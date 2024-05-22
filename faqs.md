---

copyright:
  years: 2024
lastupdated: "2024-05-22"

keywords: faq, confidential computings

subcollection: framework-financial-services

---

{{site.data.keyword.attribute-definition-list}}


# FAQs for Confidential Computing in IBM
{: #cc}

Answers to common questions about Confidential Computing on IBM Cloud.
{: shortdesc}

## What is IBM Confidential Services Platform?
{: #cc-hps}
    
IBM Confidential Services Platform is a suite of services designed to provide a highly secure environment for sensitive data and applications in hybrid cloud deployments, leveraging Confidential Computing capabilities on IBM Z or LinuxONE.

## What is Confidential Computing, and how does it relate to Confidential Services Platform?
{: #cc-hpp}

Confidential Computing refers to the protection of data in use by performing computation in a hardware-based Trusted Execution Environment (TEE), ensuring data is encrypted and isolated during processing. IBM Confidential Services Platform utilize this concept to protect mission-critical workloads and sensitive data.

## What is Zero-Trust?
{: #cc-zero-trust}

Zero-trust is a security model that never assumes trust and always verifies access. The zero-trust model assumes that threats exist both inside and outside traditional network boundaries, and therefore, every connection, endpoint, and domain are considered a potential threat. 

## What is the difference between Operation Assurance and Technical Assurance?
{: #cc-operation-technical}

Operation assurance ensures that the operations conducted by service providers and others are compliant and do not intentionally or unintentionally compromise security.

Technical assurance ensures that the security features are ingrained in the technology. And it is technically impossible for unauthorized access or changes to occur.


## What kind of technology underlies the Confidential Services Platform?
{: #tech}
    
The Confidential Services Platform is based on technology that includes hardware and firmware features such as memory encryption and an Ultravisor to create isolated, secure environments for workloads.

## How does Hyper Protect Crypto Service enhance security?
{: #hpcs}

 Hyper Protect Crypto Service provides exclusive and full control over cryptographic keys, ensuring that only authorized users can access and manage them. This is critical for maintaining the confidentiality and integrity of sensitive data [3].

## Can Hyper Protect Services be integrated with a hybrid cloud strategy?
{: #hb}

Yes, Hyper Protect Services are designed to support hybrid cloud strategies, allowing for secure workload deployment both on-premises and in the cloud.

## What is the Hyper Protect Virtual Server, and what does it offer?
{: #hpvs}
    
The Hyper Protect Virtual Server (HPVS) is a service that offers virtual server instances designed to protect sensitive workloads with built-in encryption and secure execution capabilities on IBM Z and IBM LinuxONE.

## How does the Hyper Protect Secure Build process work?
{: #hpsb}

The Secure Build process involves creating a secure pipeline for workload images, protecting them from unauthorized access or tampering throughout their lifecycle, from build to deployment.

## What is cryptographic agility, and why is it important in Hyper Protect Services?
{: #ca}
    
Cryptographic agility refers to the ability to quickly and easily adapt to new cryptographic standards and algorithms. This is important for Hyper Protect Services to ensure that security measures remain robust against evolving threats.

## Is there support for custom application OCI images within Hyper Protect Services?
{: #oci}    
    
Yes, Hyper Protect Services support custom application Open Container Initiative (OCI) images, which can be securely built and run within the protected service environment.

## What considerations should be taken when deploying workloads in HPVS instances?
{: #consideration}

When deploying workloads in HPVS instances, considerations should include regulatory compliance, the sensitivity of data, the required level of isolation, and the specifics of the workload's architecture to ensure optimal security and performance.

