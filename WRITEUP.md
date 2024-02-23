# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

To compare between App service and VM from azure, let make some bullet point comparison:
- Cost: Azure VM is generally more expensive than Azure App Service due to the higher resource requirements such as labour for manual management and set up. However, it can be wiser economical choice for resource-intensive application.
- Scalability: Both services offer scaling as one of their main features, but Azure App Service can automatically scale based on demand, making it easier to manage for smaller application, the real benefit from the flexibility of fully controls of VM will only become remarkable at bigger projects
- Availability: Both services offer high availability. However, the App service offer an easier to use option with redundancy storage and disaster recovery already be taken care by azure which result in slightly higher uptime compare to manual setting configuration in the case of VM
-  Azure VM requires more technical expertise which deep knowledge in server config to set up and manage, while Azure App Service's work flow is easier for user by ultilizing built-in tools.

My choice is App service for this application. In term of expenses, the fact that this project's app is small in scale and traffic make App service a more afordable options compare to fixed cost on infrastucture. With a small project like this the traffic change is small and managable with automatic scaling builtin that expand and reduce underlying resources based on the situation. The built-in backup redundancy and disaster recovery mean that the app users always get to enjoy it's high uptime and availability. The intergration with 3rd party ci/cd such as github making the deployment process effortlesss with just a few click, free me to focus on app developping. Excel in Simplicity and enable speed app-development process, the app service is my clear choice in all criterion.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

I will switch back to VM in some of these scenarios:
- When I need granular control over your environment such as installing specific software, have to sastisfy custom security requirement, or running operating systems that the App service do not offer.
- When the application is resources intensive, VM offer independent scaling for each resource such as CPU, memory, or storage. make it a better choice in this case
- Integration with On-Premises Infrastructure and legacy applications: If I have to countinue development with an app that can natively cannot be run on app service, I was left with no choice but VM. Furthermore, in case I have to integration with existing on-premises infrastructure, VMs offer higher flexibility for manage private networking and hybrid deployments.
