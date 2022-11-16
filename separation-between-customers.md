# Separation between customers

On the Standard Cloud hosting service we use a shared environment for hosting simple websites. This service includes one webserver per client and access to a shared database service with unique connection credentials. 

For Single Cloud and above our hosting service offers:

* All customers have their own Virtual Private Cloud (VPC) for containing their hosting environment.
* Each VPC has its own set of security keys and credentials which isolates each environment to that individual client only.
* Each client has their own cloud services (webserver, database service, S3 for static file storage)

For larger client accounts we setup dedicated AWS accounts for the highest level of isolation.
