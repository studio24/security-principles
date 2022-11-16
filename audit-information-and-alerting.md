# Audit information and alerting

All changes to the codebase can be audited and reviewed via GitHub pull requests and commit histories.  

Server logs are stored on EBS storage so that they persist even if a server is terminated. These are also accessible via the AWS Cloudwatch service and are kept for a default retention period of 35 days.

Email logs are stored on [Postmark](https://postmarkapp.com/) and are kept for 45 days.

We keep a record of any critical support incidents for at least 7 years. 
