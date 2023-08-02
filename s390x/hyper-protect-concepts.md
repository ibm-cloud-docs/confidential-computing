---

copyright:
  years: 2023, 2023
lastupdated: "2023-08-02"

keywords: 

subcollection: confidential-computing

---

{{site.data.keyword.attribute-definition-list}}

# Concepts in Hyper Protect Platform
{: #secure-execution}

Understand the common concetps in the Hyper Protect platform.

TO-DO: Need a diagram or something to explain those key concepts and their relationships.


## Secure Execution

Understand the Secure Execution for Linux in the Hyper Protect platform.

The Secure Execution for Linux is available as part of the following hardwares:
   * IBM z15 and z16
   * IBM LinuxONE III and LinuxONE 4

Secure Execution for Linux is built to apply Zero Trust policies. Encryption combined with architectural, development and manufactural processes can establish technical assurance. Regulation and Audition require proof that the assumed environment and workload is present as well as appropriate personalisation of instances has happened. A common way to provide such proof are attestation methods or through an attestation record. 

To achieve this, the zSystem firmware contains a so-called Ultravisor, a trusted firmware component, which enforces memory protection and offers the owner of a given KVM guest to securely pass secret information to the Ultravisor by using the public host key.

![Secure Exuection for Linux](../images/lxse_uv.jpg){: caption="Figure 2. IBM Secure Execution for Linux" caption-side="bottom"}}


To process the secret information, the Ultravisor uses the matching private host key. The private host key is specific to an IBM z or LinuxONE server and is hardware protected.

![Securing the workload](../images/lxse_flowkeys_otherway.jpg){: caption="Figure 3. Securing the workload" caption-side="bottom"}}



## Contract


TO-DO: Need explanation on the concept and why it matters.


## Attestation


TO-DO: Need explanation on the concept and why it matters.



