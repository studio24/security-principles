# Email security

We use a dedicated email delivery service, [Postmark](https://postmarkapp.com/), to deliver emails reliably. We believe this is more effective than rolling our own email service.

Postmark has many resources to help with [email security](https://postmarkapp.com/security). Our standard email security setup is:

* [Verify domains](https://postmarkapp.com/support/article/1046-how-do-i-verify-a-domain) for email sending via DKIM and Return-Path DNS settings. 
* Disable email tracking in Postmark (for data privacy).
* We use the REST API over HTTPS where possible to send emails, falling back to SMTP as an alternative.

If Postmark is not acceptable to use for your project, we can use [AWS Simple Email Service (SES)](https://aws.amazon.com/ses/) hosted in your local country, though additional setup costs will apply. AWS SES also supports [domain verification via DKIM](https://docs.aws.amazon.com/ses/latest/dg/send-email-authentication-dkim-easy.html).
