# Secure development

We develop web applications to be secure by design. Our high-level secure development principles appear below.

## Design

When planning web development projects we aim to create secure systems. 

We review the following, and peer review it, to help design a secure solution. We review security on an ongoing basis throughout the project.

* User authentication 
* Access control (authorisation)
* How we are processing personal data
* Whether we are dealing with sensitive personal data (e.g. health data)
* How might malicious users try to exploit the feature? What can we do about it? How can we test this?
* What 3rd party software or packages do we need to use for this project and is there a supported, stable version we can use?
* What 3rd party systems do we need to interact with and what security implications does this have?

## Development 

### Project code

* Studio 24 stores the codebase within private GitHub repositories (unless the client decides to make the repo public). We are happy to use client GitHub organisations.
* No sensitive data such as passwords or security keys are stored within these repositories.
* Sensitive data such as passwords or security keys are stored within secure vaults or data management tools with access limited as required.
* We store application and config files outside of the website document root.

### Security considerations

We take care to be aware of common security considerations:

* Cross-site scripting (XSS).
* Cross-site Request Forgery (CSRF).
* SQL injection (use prepared statements).
* Filter incoming data and sanitize data when it is outputted.
* Validate incoming data before it is used.
* If something fails, throw an exception. You can catch these effeciently in your code.
* If cryptography is used rely on well supported packages rather than roll it ourselves.
* Separate the view layer (front-end templates) by using a proper templating system that is not just PHP (we use Twig).

[PHP: The Right Way](https://phptherightway.com/#security) and [OWASP Cheat Sheet](https://cheatsheetseries.owasp.org/) are good resources for web development security.

### External packages

* We use the current latest stable version of [PHP](https://www.php.net/supported-versions).
* We use the current Long Term Support version of [NodeJS](https://nodejs.org/en/) for JavaScript libraries.
* We use supported versions of any packages and libraries our code relies on. 
* Where legacy software versions are in use we discuss these with the client and put a plan in place to upgrade these or migrate away to a newer system.
* We manage PHP packages via Composer and JavaScript packages via Node.
* We audit CMS plugins for how well used they are in the community and how well they are maintained.

## Testing

* Where appropriate, we work with independant security professionals to perform penetration security testing on websites before launch. We partner with Zoonou for CREST accredited [penetration testing](https://zoonou.com/our-services/penetration-testing/).
* We use [Roave Security Advisories](https://github.com/Roave/SecurityAdvisories) to test for any vulnerabilites in PHP packages.
* We create automated tests for custom web applications, focussing on unit tests for component functionality and end to end tests for critical end user functioanlity (e.g. submitting a form).
* Where automated tests exist we integrate continuous integration (using GitHub Actions) so tests are run before code is merged into the main branch (and therefore deployed).
* Where critical functionality needs to be manually tested we create test plans to run through before any deployment.

## Deployment

* All code changes and updates are tested in a local development environment prior to deployment to the hosting environment. 
* We deploy and test to a staging environment for further testing and approval as required. 
* Once this has been sufficiently tested and peer reviewed/approved then the production environment is updated.
* We use automated deployments methods to deploy project code from GitHub.
* We develop code on branches and merge these into the main branch via pull requests. 
* Pull requests undergo peer review and automated code checks, where appropriate (e.g. code linting, automated tests).
* We use branch protection rules at GitHub to enforce this process.
* Deployment systems either automatically deploy code from the main branch (when new code is merged into the main branch), or deploy on manual request. 
* Where deployment is manually requested, this can only be done if you are connected via secure VPN and have SSH key access to the server you are deploying to. 
