---

copyright:
  years: 2023, 2023
lastupdated: "2023-12-13"

keywords: best practices, technical principles

subcollection: confidential-computing

---

{{site.data.keyword.attribute-definition-list}}

# Best practices for confidential computing
{: #best-practices}


These best practices summarize some of the most important technical principles for application providers based on the controls and implementation guidance of the confidential computing. 
{: shortdesc}


## Technical Assurance

Utilize hardware and firmware-based protection mechanisms to ensure the security of the system and the data it processes. This includes utilizing Trusted Execution Environments (TEEs) for creating secure enclaves that isolate sensitive data and computations from the rest of the system.

## Trusted Execution Environment (TEE) Deployment

Implement TEEs to establish isolated execution boundaries around applications and data, protecting them against unauthorized external access, while still allowing for necessary interactions across these boundaries.

## Reduced Trust Boundary

Minimize the trusted computing base to limit the system components that need to be trusted to maintain the overall security posture. This principle helps in reducing the attack surface of the application.

## Separation of Duty

Design and control applications by ensuring that roles and responsibilities are divided among different entities to prevent unauthorized access and reduce the risk of insider threats. This also involves restricting access to cryptographic keys to maintain data confidentiality.

## Exclusive Control Over Cryptographic Keys

Maintain full and exclusive control over cryptographic keys to ensure that sensitive data remains encrypted and only accessible to authorized entities. This is critical in establishing trust in a multi-tenant cloud environment.

## Support for OCI Images

Ensure that the confidential computing solution supports Open Container Initiative (OCI) images, which standardize container runtime and image format, making it easier for applications to run across different cloud environments.

## Scalability

Design applications to be scalable in conjunction with the infrastructure, ensuring that security does not become a bottleneck as performance and memory requirements increase.

## Zero Trust Architecture Integration

Keep in mind of developing and deploying applications with zero trust security models, continuously verifying and never assuming trust, even within the hybrid cloud infrastructure.

## Data Protection Throughout Lifecycle

Extend data protection principles to cover data in use, not just data at rest and data in transit, to ensure comprehensive security across the entire data lifecycle.

## Regular Awareness and Training

Stay informed about the latest threats and development of confidential computing technologies. Ensure that the team is knowledgeable and trained in implementing and leveraging these technologies effectively.


