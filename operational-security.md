# Operational security

## Vulnerability management

We have a range of techniques to monitor and address vulnerabilities:

* [GitHub Dependabot](https://docs.github.com/en/code-security/dependabot/working-with-dependabot) alerts to monitor package vulnerabilities
* [Roave security advisories](https://github.com/Roave/SecurityAdvisories) to monitor Composer package vulnerabilities (PHP packages)
* Any known vulnerabilities that are being exploited in the wild are addressed as a matter of urgency, via whatever the recommended solution is (eg: installing a patch or removing a package).
* Regular patching and updating of the operating system, CMS software and PHP packages are part of our support service.

## Protective monitoring

We monitor for attacks and misuse to help identify possible attacks:

* We have performance alerts in place that notify us when system resources are escalated to an extreme level ([AWS Cloudwatch](https://aws.amazon.com/cloudwatch/)).
* We use monitoring and alerting packages that check the availability and response at 5 minute intervals ([Pingdom](https://www.pingdom.com/)).
* We use automated alerting tools to help alert us to critical website issues out-of-hours ([iLert](https://www.ilert.com/)).

## Incident management

We have a technical support service where clients can report issues. We also proactively monitor websites and web services to help detect issues.

After being alerted/notified of an incident the Support Team will review the issue. If it is a critical issue (e.g. a service is down) then we prioritise this. Where additional help is required we escalate this to second line support and get experts within the agency to help address the problem.

We have an out-of-hours support line available for clients to use for critical issues outside of working hours (additional fees apply for this service).

Studio 24 produces an incident report for events such as site outages to notify the client of key information including but not limited to:

* Summary of the incident 
* Duration of incident
* Root cause of incident 
* How the incident was resolved 
* Any steps taken to mitigate a repetition of the incident 
* Suggested/further actions (as required) to mitigate a repetition of the incident

## Configuration and change management

Cloud hosting services are managed via:

* Hosting service configuration is managed via [Terraform](https://www.terraform.io/) and [Ansible](https://www.ansible.com/). 
* Hosting configuration (without sensitive data) is backed up to a private GitHub repository.
* The hosting environment and updates are tested within a sandbox environment and peer reviewed prior going live. 
* Studio 24 uses software autonomy to manage the hosting environment and all changes can be audited.
