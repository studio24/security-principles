# Asset protection and resilience
Hosting is via AWS (Amazon Web Services), in region eu-west-1 (Ireland) or eu-west-2 (London).   

For further information please view 
* [AWS data center controls](https://aws.amazon.com/compliance/data-center/controls/)  
* [AWS Service Level Agreements](https://aws.amazon.com/legal/service-level-agreements/?aws-sla-cards.sort-by=item.additionalFields.serviceNameLower&aws-sla-cards.sort-order=asc&awsf.tech-category-filter=*all)
## Resilience
* Configuration and Data for the web server are stored on (EBS) Elastic Block Storage to help ensure availability and easy re-attachment to an alternative server if required.
* Configuration (without sensitive data) is backed up to a private GitHub repository for further redundancy.
* Auto Scaling Groups are used to manage the availability of servers.
* Database(s) and file structure are backed up to a secure (non-public) S3 bucket daily, these are stored for 35 days and then automatically deleted.
* Data may be used on Development machines as required, all these devices meet Cyber Essentials accreditation. Where sensitive data is stored in databases we develop scripts to download safe versions of the database with sensitive data removed for development work.

## Data at rest protection
* We allow minimal access to the servers and database content is encrypted at rest.


## Data sanitization
* When decommissioning via AWS all servers, storage blocks and S3 buckets are permanently deleted.
* Local devices are accessible via an individual staff member only. 
* Any data is removed from the device. 
* All hard drives are encrypted and if a computer is to be used by a new staff member or decommissions they are securely wiped and the OS reinstalled.
