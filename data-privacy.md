# Data privacy

As an ethical agency we take data privacy seriously and advise clients on how to best process data online to comply with GPDR. 

The GDPR principles include:

* **Inform users** – Tell users why you are collecting data and who this is shared with.
* **Limit what you collect** – Limit data collection to what is necessary.
* **Accuracy** – Take reasonable steps to keep user data accurate.
* **Limit data retention** – Limit how long you keep data for.
* **Security** – Process user data in a secure way and protect user data from unlawful processing.

We wrote a series of [blog posts to advise clients about GDPR](https://www.studio24.net/blog/practical-approach-to-gdpr/).

## Consent for data collection

Collection of personal data must meet a [lawful basis for processing](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/lawful-basis-for-processing/), the most common of which for websites are:

* **Consent** – You need to offer users an informed choice and ask for opt-in consent. For example, opting into a marketing newsletter.
* **Contract** – You need to process user data to fulfil a contractual obligation to that user. For example, processing an order on an E-Commerce site. Your website terms and conditions would normally cover this use case so is more straightforward.
* **Legitimate interests** – You have a legitimate reason for processing user data (which can be commercial) that passes the legitimate interests test.

## Reviewing data privacy

We review data privacy requirements in every project, since each project has individual requirements. The specifics of data privacy for your website will be discussed in your project. 

Areas we review include:

* What personal data is collected (any data that directly or indirectly identifies a person)?
* Are you collecting [special category](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/lawful-basis/special-category-data/what-is-special-category-data/) of personal data (e.g. protected characteristic, health data)?
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

Under GDPR a serious data breach that results in a risk to people’s rights and freedoms must be [reported to the Information Commissioner’s Office (ICO)](https://ico.org.uk/for-organisations/report-a-breach/). ICO gives the example of a customer database being stolen could enable identity theft, so needs to be reported. Whereas a staff telephone list is not a serious risk and would not be.

In the context of a website managed by Studio 24, if Studio 24 (the processor) is made aware of a data breach we will make the client (the data controller) aware as soon as possible. We will report this to ICO within 72 hours, or we will request the client (data controller) does this. 

We keep a record of contacts our Support team can contact in the case of any data breach or critical issue on your website. 

You can find out more about what constitutes a serious data breach and how to report it on [ICO’s guide to Personal data breaches](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/personal-data-breaches/). 
 