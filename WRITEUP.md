# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

ANSWER: I chose an app service to ensure our developers can focus solely on the application itself without needing to manage the infrastructure. This decision was driven by the fact that our developers don't have the time to handle infrastructure management. Additionally, using an app service will facilitate scaling up to a mobile application in the future. 
**Cost**: In the long run, the app service will be more cost-effective. 
**Scalability**: The app service will make it easier to scale our application to a mobile platform.
**Availability**: The app service offers high availability, which is crucial since this article database will be used by very critical users.
**Workflow**: We can leverage CI/CD pipelines and GitHub for our deployment workflow, streamlining the development process.

We decided against choosing a VM for several reasons, which are essentially the opposite of the benefits offered by an app service.
Cost: Using a VM would ultimately be more expensive.
Scalability: A VM wouldn't easily scale to meet our future needs for this application.
Availability: Managing a VM would require us to ensure high availability ourselves, which adds complexity.
Workflow: The workflow would be more challenging for our developers, as they would need to manage both the code and the deployment. Additionally, we would need personnel skilled in VM management.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

ANSWER: We might reconsider our decision if we had enough developers to manage the VM infrastructure. Additionally, if mobile scalability isn't required by users or if our company prioritizes cost reduction, these factors could also influence a change in our decision.
