---

copyright:
  years: 2023, 2023
lastupdated: "2023-08-17"

keywords: 

subcollection: confidential-computing

---

{{site.data.keyword.attribute-definition-list}}

# Hyper Protect Platform on IBM Z and LinuxONE
{: #hyper-protect-overview}


The IBM Hyper Protect Platform in its first generation leverages the [Secure Service Container technology](https://www.ibm.com/downloads/cas/V8XERDQO){: external}. This technology already maintains the confidentiality and integrity of hosted client data. It provides the support for enterprise DevSecOps solutions like the IBM Hyper Protect Secure Build or the simplified approach to industry and regulatory challenges, which technical assurance provides.

In its second generation, the IBM Hyper Protect Platform leverages [IBM Secure Execution for Linux technololgy](https://www.ibm.com/docs/en/linux-on-systems?topic=virtualization-introducing-secure-execution-linux){: external}. This is a hardware-based security technology, which was introduced with the IBM z15® and IBM® LinuxONE III generation systems for Kernel Virtual Machines (KVM). It is designed to provide scalable isolation for individual workloads to help protect them from not only external attacks, but also insider threats. Secure Execution can help protect and isolate workloads on-premises, or on IBM Z and IBM® LinuxONE hybrid cloud environments.

![Hyper Protect Platfrom Generation 1 and 2](../images/hps_gen1_2.png){: caption="Figure 1. Hyper Protect Platfrom Generation 1 and 2" caption-side="bottom"}

 By reducing the size of the protected environment with Hyper protect Platfrom generation 2, it is possible to enhance data protection from potential attacks on the system from inside and outside. By the ability to protect data-in-use by individual KVMs it is possible to increase flexibility and scalability of the solution, which also becomes independent of underlaying software stack.


## Protection boundary in Hyper Protect
{: #enclave-boundary}


![Protection boundary](../images/hyper-protect-boundary.png){: caption="Figure 2. Protection boundry" caption-side="bottom"}