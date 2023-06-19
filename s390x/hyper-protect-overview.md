---

copyright:
  years: 2023, 2023
lastupdated: "2023-06-19"

keywords: 

subcollection: confidential-computing

---

{{site.data.keyword.attribute-definition-list}}

# Hyper Protect Platform
{: #hyper-protect-s390x}


The IBM Hyper Protect Platform in its first generation leverages the [Secure Service Container technology](){: external}. This technology already maintains the confidentiality and integrity of hosted client data. It provides the support for enterprise DevSecOps solutions like the IBM Hyper Protect Secure Build or the simplified approach to industry and regulatory challenges, which technical assurance provides.

In its second generation, the IBM Hyper Protect Platform leverages [IBM Secure Execution for Linux technololgy](https://www.ibm.com/docs/en/linux-on-systems?topic=virtualization-introducing-secure-execution-linux){: external},. This is a hardware-based security technology, which was introduced with the IBM z15® and IBM® LinuxONE III generation systems for Kernel Virtual Machines (KVM). It is designed to provide scalable isolation for individual workloads to help protect them from not only external attacks, but also insider threats. Secure Execution can help protect and isolate workloads on-premises, or on IBM Z and IBM® LinuxONE hybrid cloud environments.

![Hyper Protect Platfrom Generation 1 and 2](../images/hps_gen1_2.png){: caption="Figure 1. Hyper Protect Platfrom Generation 1 and 2" caption-side="bottom"}

 By reducing the size of the protected environment with Hyper protect Platfrom generation 2, it is possible to enhance data protection from potential attacks on the system from inside and outside. By the ability to protect data-in-use by individual KVMs it is possible to increase flexibility and scalability of the solution, which also becomes independent of underlaying software stack.

## About Secure Execution for Linux

The Secure Execution for Linux is available as part of the following hardwares:
   * IBM z15 and z16
   * IBM LinuxONE III and LinuxONE 4


Secure Execution for Linux is built to apply Zero Trust policies. Encryption combined with architectural, development and manufactural processes can establish technical assurance. Regulation and Audition require proof that the assumed environment and workload is present as well as appropriate personalisation of instances has happened. A common way to provide such proof are attestation methods or through an attestation record. 

To achieve this, the zSystem firmware contains a so-called Ultravisor, a trusted firmware component, which enforces memory protection and offers the owner of a given KVM guest to securely pass secret information to the Ultravisor by using the public host key.

![Secure Exuection for Linux](../images/lxse_uv.jpg){: caption="Figure 2. IBM Secure Execution for Linux" caption-side="bottom"}}


To process the secret information, the Ultravisor uses the matching private host key. The private host key is specific to an IBM z or LinuxONE server and is hardware protected.

![Securing the workload](../images/lxse_flowkeys_otherway.jpg){: caption="Figure 3. Securing the workload" caption-side="bottom"}}

