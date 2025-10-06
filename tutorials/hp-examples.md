---

copyright:
  years: 2025
lastupdated: "2025-10-06"

keywords: 

subcollection: confidential-computing

---

{{site.data.keyword.attribute-definition-list}}

# Tutorials and examples
{: #tutorial-example}

You can refer to this page for all the available tutorials or code examples for Hyper Protect products.


## Tutorials
{: #tutorial}

The following list gives you an overview of the available tutorials when using Hyper Protect products.

- [Run multiple OCI container workloads on IBM Hyper Protect Virtual Servers for VPC](https://developer.ibm.com/tutorials/awb-run-multiple-oci-container-workloads-on-hpvs-for-vpc/){: external}

- [Deploying the PayNow application on Hyper Protect Virtual Server for VPC](/docs/vpc?topic=vpc-financial-transaction-confidential-computing-on-hyper-protect-virtual-server-for-vpc)

- [Use Terraform to automate deployment of IBM Cloud Hyper Protect Services](https://developer.ibm.com/tutorials/use-terraform-to-automate-deployment-of-ibm-cloud-hyper-protect-services/){: external}.

- [Use IBM Cloud Hyper Protect Crypto Services to Encrypt VMware Disks](https://developer.ibm.com/tutorials/use-hyper-protect-crypto-services-to-encrypt-vmware-disks/){: external}.

- [Using Hyper Protect Crypto Services PKCS #11 for IBM Db2 native encryption](/docs/hs-crypto?topic=hs-crypto-tutorial-db2-pkcs11)

- [Using Hyper Protect Crypto Services PKCS #11 for Oracle Transparent Database Encryption](/docs/hs-crypto?topic=hs-crypto-tutorial-tde-pkcs11)

- [Integrate Enterprise HashiCorp Vault with IBM Cloud Hyper Protect Crypto Services](https://developer.ibm.com/tutorials/integrate-enterprise-vault-ibm-cloud-hyper-protect-crypto-services/){: external}.


## Code examples
{: #examples}

Confidential Services Platform provides a list of scripts to help you speed up your deloyment. To explore those code samples, go to the [repository](https://github.com/ibm-hyper-protect){: external}. For more information about Terraform, see [About Terraform on IBM Cloud](/docs/ibm-cloud-provider-for-terraform?topic=ibm-cloud-provider-for-terraform-about).


The following list gives you an overview of the available samples. See the repo for the latest samples and the readme file of each sample for detailed instructions. 

- `linuxone-vsi-automation-samples` - Ansible and Terraform examples for IBM Cloud LinuxONE and z/OS virtual server instances. The examples are:   
    - `create-contract` - creates an encrypted and signed contract.
    - `create-contract-dynamic-registry` - creates an encrypted and signed contract with a dynamic registry reference.
    - `hello-world` - deploys the hello-world example as a Hyper Protect Virtual Server for VPC.
    - `nginx-hello` - deploys the nginx-hello example as a Hyper Protect Virtual Server for VPC.
    - `mongodb` - deploys three MongoDB instances on Hyper Protect Virtual Servers for VPC in three availability zones.
    - `postgresql` - deploys a PostgreSQL instance on a Hyper Protect Virtual Server for VPC in a region.
    - `postgresql-cluster` - deploys a PostgreSQL cluster on Hyper Protect Virtual Servers for VPC in given regions.
    - `log-encryption` - encrypts selected log messages.
- `paynow-website` - A node.js Express app serving the PayNow website, and the deployment instructions as a Hyper Protect Virtual Server.
- `k8s-operator-hpcr` - Custom resources for managing Hyper Protect Virtual Servers in Kubernetes clusters.
- `terraform-provider-hpcr` -  A terraform provider to support working with IBM Cloud Hyper Protect Virtual Server for IBM Cloud VPC.
- `contract-go` - A go-based utility to encrypt and decrypt the contract for Confidential Services Platform.
- `secure-build-cli` - The scripts and intructions on how to use Hyper Protect Secure build CLI.
- `hpcs-automation-samples` - Automation examples for Hyper Protect Crypto Services.
