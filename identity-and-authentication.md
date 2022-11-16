# Identity and authentication

Access to services is managed via the following methods.

## Hosting infrastructure

* The AWS hosting environment is secured via [Identity and Access Management (IAM)](https://aws.amazon.com/iam/) policies and two-factor authentication, with limited access to the Support team only.
* All connections to the service are controlled by VPN connectivity and SSH keys.
* We have policies in place for the addition or removal of team members and access, when the team changes.
* Accessing the AWS control panel requires username, password and two-factor authentication.

## Website applications / CMS

* We use [one-way hashing](https://www.php.net/password_hash) to secure passwords for web applications using the Bcrypt algorithm.
* We recommend a minimum password length for strong passwords and two-factor authentication to secure logins to admin systems.
* Studio 24 use a single shared login to client admin systems for support purposes with a strong password (we manage team passwords in [1Password](https://1password.com/)).
