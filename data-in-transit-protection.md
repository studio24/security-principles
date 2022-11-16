# Data in transit protection

We implement as many of the suggested best practice methods as possible to ensure data security.

## Encryption

We use HTTPS to encrypt all network traffic for websites and web applications using TLS version 1.2 and TLS 1.3.

We use [Lets Encrypt](https://letsencrypt.org/) and [AWS Certificate Manager](https://aws.amazon.com/certificate-manager/) for automated, free SSL certificates. We can also use commercial SSL certificates if required (though these do not offer more security).

We test SSL setup on websites using [Qualys SSL Server Test](https://www.ssllabs.com/ssltest/).

## Network protection

Network access to cloud services by Studio 24 staff is via encrypted Virtual Private Network (VPN) and we use authorised SSH keys for authentication.

_TODO: "Cloud platforms usually allow you to create virtual networks, which use dynamic routing rules on the underlying network to ensure that packets can only flow between your hosted resources." Suggested text:_

We host clients on AWS cloud hosting, we create a [Virtual Private Cloud (VPC)](https://aws.amazon.com/vpc/) for each client to isolate their cloud environment.

## Authentication

Accessing the AWS control panel requires username, password and two-factor authentication.

Accessing cloud services requires secure connection to VPN and authentication via SSH key.

_Is this accurate:_

Cloud database services are locked down so they can only be accessed via cloud web servers. Authentication is via a password. 

API services are locked down by IP address and authentication key if they are private.

Also see [identity and authentication](identity-and-authentication.md).