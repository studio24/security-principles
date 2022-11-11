# Separation between customers
* All customers have their own VPC (Virtual Private Cloud) for containing their hosting environment.
* Each VPC has its own set of security keys and credentials which isolates each environment to that individual client only.
* Depending on the hosting package, the client will either have their own database instance or use a shared database server with unique connection credentials.
