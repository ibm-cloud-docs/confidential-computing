---

copyright:
  years: 2023, 2023
lastupdated: "2023-08-17"

keywords: 

subcollection: confidential-computing

---

{{site.data.keyword.attribute-definition-list}}

# Products in Hyper Protect Platform
{: #hyper-protect-products}

Understand the product portfolio in the Hyper Protect platform.


![Hyper Protect products](../images/hyper-protect-platform.png){: caption="Figure 1. Hyper Protect products" caption-side="bottom"}


## Hyper Protect Container Runtime
{: #hpcr}

**TO-DO：Add the description of HPCR**

![Hyper Protect Container Runtime on public and Hybrid cloud](../images/hpcr-hybrid.svg){: caption="Figure 2. Hyper Protect Container Runtime on public and Hybrid cloud" caption-side="bottom"}


You can deploy a workload built with SUSE Linux Enterprise Base Container Images into the Hyper Protect Container Runtime in a hybrid confidential computing environment. For more information, see [Confidential Computing with SUSE Linux Enterprise Base Container Images Using the IBM Hyper Protect Platform](https://documentation.suse.com/trd/linux/single-html/gs_sles_ibm-hpvs).


## Hyper Protect Virtual Servers
{: #hpvs}




TO-do:  need the product architecure diagram and explanation


## {{site.data.keyword.hscrypto}} with {{site.data.keyword.uko_full_notm}}
{: #hpcs}

{{site.data.keyword.cloud}} {{site.data.keyword.hscrypto}} is a dedicated key management service and Hardware Security Module (HSM) that provides you with the Keep Your Own Key capability for cloud data encryption. Built on FIPS 140-2 Level 4 certified hardware, {{site.data.keyword.hscrypto}} provides you with exclusive control of your encryption keys. You can take the ownership of the HSM through master key initialization. With {{site.data.keyword.uko_full_notm}}, you can connect your service instance to keystores in IBM Cloud and third-party cloud providers, back up and manage keys using a unified system, and orchestrate keys across multiple clouds.

The following architecture diagram shows how you interact with Hyper Protect Crypto Services components to protect your sensitive data and keys.

![HPCS architecture components](../images/hs-crypto-components-uko.svg "HPCS architecture components"){: caption="Figure 1. Interaction with {{site.data.keyword.hscrypto}} components" caption-side="bottom"}


**To-do: use a three-column table to list the major functions in HPCS and its usage links in the 3rd column**

| Feature name |  Description |  Usage and reference link |
|----|-----|------|
| Key Management Service (KMS) |     |    |
| Universal Key Orchestration (UKO)  |   Description of UKO  |   [UKO Introduction](), [UKO tutorial](https://cloud.ibm.com/docs/hs-crypto?topic=hs-crypto-tutorial-uko-satellite) |
| Hardware Security Module (HSM) |  |    |
{: caption="Table 1. Major features in Hyper Protect Crypto Service" caption-side="bottom"}}

## Hyper Protect managed Add-on for Kubernetes
{: #ikswhp}

TO-do:  need the product architecure diagram and explanation
