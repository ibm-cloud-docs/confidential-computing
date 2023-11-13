---

copyright:
  years: 2023, 2023
lastupdated: "2023-11-13"

keywords: 

subcollection: confidential-computing

---

{{site.data.keyword.attribute-definition-list}}

# Getting started with Confidential Computing
{: #about}

Confidential computing (CC) protects applications and data while in use by keeping them encrypted all the time, even in memory, and only decrypting inside the processor, which is also known as Truested Execution Environment (TEE). The decryption keys are known only to the application/data owner and the processor. This way, even a compromised operating system or hypervisor can’t peek into the application or steal any sensitive data. Confidential computing is critical for cloud deployments, but also for edge deployments where such devices can be easily compromised or stolen. It’s also important for AI data processing where data needs to be shared (such as federated learning) but the data owners don’t trust the infrastructure where data needs to be jointly processed.

![Confidential Computing](images/what-is-cc.jpg){: caption="Figure 1. Confidential Computing" caption-side="bottom"}

As defined by the [Confidential Computing Consortium](https://confidentialcomputing.io/wp-content/uploads/sites/85/2021/03/confidentialcomputing_outreach_whitepaper-8-5x11-1.pdf), Confidential Computing has the following key characteristics: 

* **Data confidentiality**: Unauthorized entities cannot view data while it is in use within the TEE.
* **Data integrity**: Unauthorized entities cannot add, remove, or alter data while it is in use within the TEE.
* **Code integrity**: Unauthorized entities cannot add, remove, or alter code executing in the TEE.


## IBM confidential computing strategy
{: #cc-ibm}


IBM confidential computing strategy focuses on providing secure and trusted computing environments that protect sensitive data and workloads throughout their lifecycle. It aims to address concerns related to data privacy, security, and compliance in cloud, hybrid cloud, and edge computing environments with technical assurance rather than operation assurance. IBM's confidential computing strategy encompasses the following key elements:

- **Hardware-Based Security**
   IBM leverages hardware and firmware security features to establish trusted execution environments (TEEs). These TEEs create isolated enclaves where sensitive data and computations can be securely processed, ensuring confidentiality and integrity.

- **Secure Enclaves and Isolation**
   IBM employs secure enclaves to isolate sensitive workloads, applications, and data from the underlying infrastructure and other untrusted components. This isolation prevents unauthorized access and tampering, even by privileged users or compromised systems.

- **Data Encryption and Protection**
   IBM incorporates strong encryption mechanisms to safeguard data in transit and at rest. It includes solutions such as Hyper Protect platforms, which provide encryption and key management capabilities to protect data in cloud environments.

- **Confidential Containers**
   IBM offers technologies such as Hyper Protect Container Runtime to enable the secure execution of containerized applications. By leveraging hardware-based security features, confidential containers protect sensitive workloads and data within containers, even in shared or untrusted environments.

- **Trusted Execution and Attestation**
  IBM incorporates mechanisms for attestation and verification of trusted execution environments. This ensures the integrity of the enclave and verifies that it hasn't been compromised, establishing trust between different components in the system.

- **Compliance and Standards**
  IBM's confidential computing strategy takes into account various regulatory and compliance requirements. IBM aims to provide solutions that help organizations meet industry-specific regulations and standards while maintaining data privacy and security.

- **Cloud-Based Confidential Computing**
   IBM provides confidential computing capabilities in its Hyper Protect services. These services enable organizations to leverage secure enclaves and confidential computing technologies in the cloud, providing a secure and compliant platform for sensitive workloads.

In a nut shell, IBM confidential computing strategy emphasizes the use of hardware-based security, secure enclaves, encryption, and isolation mechanisms to protect sensitive data and workloads with zero-trust and technical assurance. By incorporating these elements into their offerings, IBM aims to provide organizations with secure and trusted environments that safeguard their data and maintain compliance in various computing scenarios.



## Personas in the confidential computing
{: #cc-personas}

When considering personas, we start with the view that the responsibility for defining the workload to be deployed is separate from control over how it gets deployed. And that there is no “assumed” trust that what is expected to be deployed is in fact what gets deployed.

- **Container Image Provider**
  A workload can consist of one or more container images which in combination deliver an expected solution. To ensure the integrity of the solution we must be able to verify the individual container images which deliver the solution, and ensure supply chain integrity through this.
  All container images used are expected to be built in a secure manner that reassures the Workload Provider of their supply chain integrity and provides a way to verify the appropriate container images are being deployed. This means a signature is securely established over the generated container image and the signature provides a means for a Workload Deployer Persona to establish trust in the container image being deployed.

- **Workload Provider Persona**
  This may be the same persona as the Container Image Provider, but the workload may also combine container images from different sources. The workload provider persona defines the container(s) and environment requirements for the solution to be deployed. There is no trust given to allow any other persona to change the container images being used to provide the workload or to redefine the environment requirements specified by the workload provider.

- **Workload Deployer Persona**
  This persona is responsible for deploying the workload using the (cloud) infrastructure available. The Workload Provider provides the encrypted workload contract section and identifies and communicates to the Workload Deployer the environment required to provide the workload to an end user. This allows the Workload Deployer to supplement the definition provided by the workload provider with instance/environment specific information (logging, storage etc). 
  The workload deployer is responsible for the service availability. They
    * can control the networking, compute and storage resources made available to instance - can influence network traffic in and out of a provided workload
    * cannot change the workload to be deployed
    * cannot change the Workload Provider’ environment expectations.

  If they do change the environment expectations, either the workload will not start, or the Auditor will not verify the environment when the workload is deployed.

- **Auditor**
  Since there is no “assumed” trust between the Workload Provider and other personas we must ensure at runtime that the workload is not deployed in a manner which breaks the Workload Provider’s or the Workload Deployer’s expectations.
  The Auditor is the persona with responsibility for verifying that a deployed workload is both the workload expected and deployed to the expected environment. They do this by obtaining and verifying a trusted attestation record at runtime. The contents of this record can be verified against workload and environment expectations and details are covered in future section of this document.

- **Infrastructure/System Admin Persona**
  This role includes the system (cloud) administrator of a compute, storage, and network or support persona of the infrastructure like a Site Reliability Engineer (SRE). They will have responsibility for the underlying hardware but must not be able to use the capabilities this role offers to access confidential data or subvert the workload providers definition of the workload and expected environment. The use of Secure Execution achieves this through protecting the memory used by the workload from all external access at runtime, and the use of an encrypted Contract protects the intended workload and environment definitions at deployment time.
 


