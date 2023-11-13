---

copyright:
  years: 2023, 2023
lastupdated: "2023-11-13"

keywords: 

subcollection: confidential-computing

---

{{site.data.keyword.attribute-definition-list}}

# Secure multi-party computation and collaboration
{: #smpc}

As various entities collaborate towards a common goal: the need for the individual data privacy as well as correct computation output. With confidential computing, it is possible to enable distributed multi-party computation and collaboration, where participants are ensured that their data or insights are protected even when being calculated outside their direct control.
{: shortdesc}

In multi-party collaborations (MPC), the biggest concern is how can the confidentiality and integrity of the data be preserved? For example, secure federated learning can be applied to cases in which multiple parties have private data that needs to be combined and analyzed without exposing the underlying data or machine learning models to any of the other parties. This technology can be applied to preventing fraud in financial services, detecting or developing cures for diseases in the healthcare industry, or gaining business insight. As the following diagram shows, multiple hospitals could combine data to train a machine learning model to clinically analyze medical images.

![Secure multi-party computation - healthcare](../images/smpc-hospitals.png){: caption="Figure 1. Hospitals share data to help drug development and disease diagnostics" caption-side="bottom"}

As another example, banks can collaborate to find patterns of anti-money laundering. Each bank brings encrypted financial-transactions data to a confidential computing enclave (like a Hyper Protect Virtual Server) where data can be safely un-encrypted. The MPC application runs fraud-detection algorithms in the confidential computing enclave. Malicious administrators or operators will not be able to see financial transaction data from any banks collaborating on the MPC platform.

![Secure multi-party computation - banks](../images/smpc-banks.png){: caption="Figure 2. Banks collaborate to find patterns of anti-money laundering" caption-side="bottom"}

Using the Hyper Protect Platform and confidential computing, organizations can now ensure that data is protected against tampering and compromise, and data sovereignty and privacy regulations can be fulfilled. This includes threats within the partnering organizations and validating the integrity of the code processing that data.
The data can be combined and analyzed and the results can be sent in an encrypted format back to each party. Data remains protected throughout the entire process: while in transit, in use and at rest. The following diagram illustrates the general SMPC implementation architecture with the Hyper Protect Platform:

![Hyper Protect implementation](../images/smpc-hp.png){: caption="Figure 2. Hyper Protect implementation" caption-side="bottom"}
