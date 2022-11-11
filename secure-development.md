# Secure development

Studio 24 stores the codebase within private GitHub repositories (unless there is a client specific reason for public access).  
* No sensitive data such as passwords or security keys are stored within these repositories.
* Sensitive data such as passwords or security keys are stored within secure Vaults or data management tools with access limited as required.

Code changes to the website/project:
* All code changes and updates are tested in a local development environment prior to deployment to the hosting environment. 
* We deploy and test to a Staging environment for further testing and approval as required. 
* Once this has been sufficiently tested and peer reviewed/approved then the Live/Production environment is updated.
* Live/Production GitHub branches are protected and require approval before they can be updated and deployed.
