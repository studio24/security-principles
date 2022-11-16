# Asset protection and resilience

## Physical location

Studio 24 manages client hosting via AWS (Amazon Web Services) in regions eu-west-1 (Ireland) or eu-west-2 (London). We can manage hosting in other regions on request.

Other services we use for client hosting includes:

* [Cloudflare](https://www.cloudflare.com/) - security and performance, [hosted globally](https://www.cloudflare.com/network/)
* [Postmark](https://postmarkapp.com/) - reliable email delivery, hosted at [ServerCentral's](https://www.servercentral.com/data-centers) data center (located outside of Chicago, USA) and AWS (USA)

If sensitive information is being delivered via email we can use [AWS Simple Email Service (SES)](https://aws.amazon.com/ses/) hosted in your local country, though additional setup costs will apply.

For further information please see:
* [AWS data center controls](https://aws.amazon.com/compliance/data-center/controls/)
* [Cloudflare security](https://www.cloudflare.com/security/)
* [Postmark security and privacy](https://postmarkapp.com/eu-privacy#security-and-privacy)

## Data centre security

Physical data centre security controls at AWS are comprehensive and are detailed on https://aws.amazon.com/compliance/data-center/controls/

AWS meets ISAE 3402 standards. See https://docs.aws.amazon.com/whitepapers/latest/introduction-aws-security/compliance.html

## Data encryption

We take an approach where we encrypt all user data, with encryption at rest as our default approach using AES-256 data encryption. Where there is a need to store sensitve data we encrypt this at the application layer (in addition to encryption at rest).

Database content is encrypted at rest both in the database storage and in backups.

We use Elastic Block Storage (EBS) to store persistent data which is encrypted at rest.

## Data sanitisation and equipment disposal

* When decommissioning via AWS all servers, storage blocks and S3 buckets are permanently deleted.
* Local devices are accessible via an individual staff member only. 
* Any data is removed from the device when it is decomissioned. 
* All hard drives are encrypted and if a computer is to be used by a new staff member or decommissions they are securely wiped and the OS reinstalled.

## Physical resilience and availability

We offer four levels of web hosting for clients designed to support different SLAs:

* Standard Cloud, single cloud server with shared database service, 99.5% SLA
* Single Cloud, single cloud service, 99.9% SLA
* Scalable Cloud, auto scaling service with a minimum of 2 instances for critical services, 99.95% SLA
* High Availability Cloud, auto-scaling service hosted in 2 availability zones for redundancy, 99.99% SLA

For all services:

* Database(s) and file structure are backed up to a secure (non-public) S3 bucket daily and are encrypted at rest. These are stored for 35 days and then automatically deleted.
* Data may be used on Development machines as required, all these devices meet Cyber Essentials accreditation. Where sensitive data is stored in databases we develop scripts to download safe versions of the database with sensitive data removed for development work.
* We use [Cloudflare](https://www.cloudflare.com/application-security/) to help protect against DDoS and other security attacks.

For Standard and Single Cloud:

* Single webserver instance. On Standard Cloud a shared database service, on Single Cloud a dedicated database service.
* Configuration and data for the web server are stored on Elastic Block Storage (EBS) to help ensure availability and easy re-attachment to an alternative server if required.
* Auto scaling groups are used to manage restoring servers quickly.
* Restoring servers will have some short downtime (normally a few minutes).

For Scalable Cloud and High Availability Cloud:

* A minimum of two instances for critical services such as web server and database service.
* Auto scaling to increase hosting resources at times of high traffic and decrease resources when they are not needed. 
* We use CodeBuild and CodePipeline to manage restoring servers and deploying code changes.
* Restoring servers will have no downtime.

For High Availability Cloud:

* Scalable cloud hosting service is replicated across two availability zones (AZ) for redundancy

See [AWS Service Level Agreements](https://aws.amazon.com/legal/service-level-agreements/?aws-sla-cards.sort-by=item.additionalFields.serviceNameLower&aws-sla-cards.sort-order=asc&awsf.tech-category-filter=*all)
