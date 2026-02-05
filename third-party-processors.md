# Third-party processors

## Services hosted within UK or EU

| Name                      | Address | Main establishment location | Description of processing                             | Data processing location                                          | Further information                                                                      |
|---------------------------|---------|-----------------------------|-------------------------------------------------------|---------------------------------------------------------------|-------------------------------------------------------------------------------------|
| Amazon Web Services EMEA SARL | 1 Principal Place, Worship Street, London, EC2A 2FA | UK                          | Cloud web hosting (database, file storage)            | UK and Ireland                                                | [Privacy policy](https://aws.amazon.com/compliance/eu-data-protection/)             |
| Mythic Beasts             | Mythic Beasts Ltd, PO Box 1363, Cambridge, CB1 0FJ | UK                          | Cloud web hosting (database, file storage)            | UK                                                            | [Privacy policy](https://www.mythic-beasts.com/static/documents/privacy-policy.pdf) |
| Bunny | BunnyWay d.o.o., Dunajska cesta 165, 1000 Ljubljana, Slovenia | Slovenia  | CDN and DDoS mitigation services (Bunny CDN)          | Global                                                        | [GDPR policy](https://bunny.net/gdpr/)                                              |
| Google Cloud EMEA Limited | Velasco, Clanwilliam Place, Dublin 2 | Ireland                     | Studio 24 company document storage (Google Workspace) | Europe                                                        | [Privacy terms](https://cloud.google.com/terms/data-processing-addendum)            |
| Proton AG                 | Route de la Galaise 32, 1228 Plan-les-Ouates, Switzerland | UK                          | Studio 24 company email service (Proton Mail)         | Switzerland | [Privacy policy](https://proton.me/legal/privacy)                                   |

## Services hosted outside UK or EU

| Name               | Address                                                 | Main establishment location | Description of processing                                          | Data processing location | Guarantees for international transfer                                                                                                                     | Further information                                                                                                 | 
|--------------------|---------------------------------------------------------|----------|--------------------------------------------------------------------|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|
| 37signals LLC      | 137 N Oak Park Ave, Suite 208, Oak Park, IL, 60301, USA | USA | Client and supplier communications and document sharing (Basecamp) | USA                      | [Data processing addendum with Standard Contractual Clauses](https://37signals.com/policies/privacy/regulations/dpa/Data_Processing_Addendum_current.pdf) | [Privacy policy](https://37signals.com/policies/privacy) |
| ActiveCampaign LLC | 1 North Dearborn St, 5th Floor Chicago, IL 60602        | USA | Transactional email delivery (Postmark email)                      | USA                      | UK Extension to the EU-U.S. Data Privacy Framework.                                                                                                       | [EU Data Protection](https://postmarkapp.com/eu-privacy)     |                                                                                                     |
| Cloudflare, Inc.   | 101 Townsend St, San Francisco, CA 94107, USA           | USA | CDN and DDoS mitigation services (Cloudflare)                      | Global                   | UK Extension to the EU-U.S. Data Privacy Framework                                                                                                        | [Data Act Addendum (EU Data Act)](https://www.cloudflare.com/en-gb/legal/data-act-addendum/)
| Zendesk, Inc.      | 181 Fremont St., San Francisco, CA 94105, USA           | USA | Support ticketing service (Zendesk)                                | Global                   | UK Extension to the EU-U.S. Data Privacy Framework                                                                                                        | [Zendesk Trust Center](https://www.zendesk.co.uk/trust-center/)

You can verify USA-based services have agreed to the UK Extension to the EU-US Data Privacy Framework via the [Data Privacy Framework website](https://www.dataprivacyframework.gov/list).

## Additional information

### Amazon Web Services
We manage our hosting at AWS either in regions **eu-west-1** (Ireland) or **eu-west-2** (London). 

If other external services are used for your project, we'll document these and advise on any data privacy risks.

### Emails

Email may be used in your application to send personal data, for example an address. We recommend not sending sensitive personal data via email.

Postmark does not encrypt email messages since they must be decrypted in the admin interface. Postmark stores all sent emails for 45 days, while bounces and spam complaints are stored indefinitely in a Streams Suppression list for reporting and list hygiene.

If Postmark is not acceptable to use for your project, we can use [AWS Simple Email Service (SES)](https://aws.amazon.com/ses/) hosted in your local country, though additional setup costs will apply.
