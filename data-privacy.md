# Data privacy

As an ethical agency we take data privacy seriously and advise clients on how to best process data online to comply with GPDR. 

The GDPR principles include:

* **Inform users** – Tell users why you are collecting data and who this is shared with.
* **Limit what you collect** – Limit data collection to what is necessary.
* **Accuracy** – Take reasonable steps to keep user data accurate.
* **Limit data retention** – Limit how long you keep data for.
* **Security** – Process user data in a secure way and protect user data from unlawful processing.

We wrote a series of [blog posts to advise clients about GDPR](https://www.studio24.net/blog/practical-approach-to-gdpr/).

## Personal data

Personal data is information about an individual, which can be used to identify that individual (either directly or by
combining with other information). It only applies to living people.

Examples of personal data:

- people’s names and addresses
- photographs
- customer reference numbers
- medical information
- school reports
- customer reviews

See [Personal information - what is it?](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/personal-information-what-is-it/).

### Special category data

If we are collecting sensitive personal data, this needs to be treated with a higher level of protection. The UK GDPR
refers to the processing of these data as [special category data](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/lawful-basis/special-category-data/):

- race
- ethnic origin
- political opinions
- religious or philosophical beliefs
- trade union membership
- genetic data
- biometric data (where this is used for identification purposes)
- health data
- sex life
- sexual orientation

Personal information relating to criminal convictions and offences is classifed as [criminal offence data](https://ico.org.uk/for-organisations/guide-to-the-general-data-protection-regulation-gdpr/lawful-basis-for-processing/criminal-offence-data/).

## Consent for data collection

Collection of personal data must meet a [lawful basis for processing](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/lawful-basis-for-processing/), the most common of which for websites are:

* **Consent** – You need to offer users an informed choice and ask for opt-in consent. For example, opting into a marketing newsletter.
* **Contract** – You need to process user data to fulfil a contractual obligation to that user. For example, processing an order on an E-Commerce site. Your website terms and conditions would normally cover this use case so is more straightforward.
* **Legitimate interests** – You have a legitimate reason for processing user data (which can be commercial) that passes the legitimate interests test.

## Reviewing data privacy

We review data privacy requirements in every project, since each project has individual requirements. The specifics of data privacy for your website will be discussed in your project. 

Areas we review include:

* What personal data is collected (any data that directly or indirectly identifies a person)?
* Are you collecting [special category data](#special-category-data) (e.g. health data)?
* Are you collecting personal data for children?
* Why do we need this data, can we limit data collection?
* How long do we need to retain personal data for?
* Can we support data portability (allow users to export their data)?
* Is there any automated decision making in this project and how can we ensure this is fair?

Common techniques we use to protect personal data:

* Use positive opt-in for any consent to data collection, don't use conditional consent for data collection.
* Use clear language to ensure data collection is understood.
* Storing personal data encrypted at rest.
* Using application encryption to store special category data.
* Automate data deletion if we have fixed data retention times.
* Where 3rd party cookies are used, implement a cookie manager tool, ideally not setting 3rd party cookies without consent. Inform users how cookies are used on the website, including 3rd party cookies.
* Ensure there is a data privacy web page detailing how personal data is processed and detailing how users can request data or request data deletion. We can assist with managing these requests via our support service.
* We recommend [Matomo analytics](https://matomo.org/gdpr-analytics/) as an alternative to Google Analytics, since it has better data privacy.

## Data processor

Studio 24 acts as a data processor under GDPR for any personal data your website processes. We only process this data in the management and support of your website and we do not use this for any other purpose.

You, as the client, are the data controller under GDPR.

## External services

We manage our hosting at AWS either in regions eu-west-1 (Ireland) or eu-west-2 (London). We use external services to help power websites:

* [Cloudflare](https://www.cloudflare.com/gdpr/introduction/) - security and performance
* [Postmark](https://postmarkapp.com/eu-privacy#gdpr) - email delivery
 
Both Cloudflare and Postmark meet GDPR and Privacy Shield frameworks. 

If other external services are used for your project, we'll document these and investigate data privacy risks.

### Emails

Email may be used in your application to send personal data, for example an address. We recommend not sending sensitive personal data via email. 

Postmark does not encrypt email messages since they must be decrypted in the admin interface. Postmark stores all sent emails for 45 days, while bounces and spam complaints are stored indefinitely in a Streams Suppression list for reporting and list hygiene.  

If Postmark is not acceptable to use for your project, we can use [AWS Simple Email Service (SES)](https://aws.amazon.com/ses/) hosted in your local country, though additional setup costs will apply.

## Data breaches

See [data breaches](data-breaches.md).
