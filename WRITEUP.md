# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

| Feature | App Service | Virtual Machine (VM) |
|---|---|---|
| Cost | Pay-per-use based on resource consumption, cost-effective for smaller projects | Fixed cost based on allocated resources, potentially higher for small projects |
| Scalability | Automatically scales up/down based on traffic | Manual scaling required, or use VM scale sets with added complexity |
| Availability | Built-in redundancy and disaster recovery for high availability | Requires configuring availability features like Azure Availability Zones |
| Workflow | Simplified configuration and built-in tools, easier to deploy and manage | Greater control over environment, but requires managing server software, runtime, and deployment |

I choosing a web app service over a virtual machine. Cost-wise, the web app wins hands down with its pay-as-you-go model, saving cash. Plus, you ditch the VM maintenance headache, freeing up your time and energy. Deployment becomes a breeze thanks to the seamless GitHub integration, getting your app live in a flash. High availability is built-in, so your users enjoy consistent uptime. And when it comes to scaling, the web app adapts to your needs effortlessly, avoiding the manual VM configuration struggles. Furthermore, the web app service excels in simplicity and speed. The seamless integration with your GitHub repository allows for effortless deployment with just a few clicks. This streamlines your workflow significantly compared to the cumbersome setup and configuration of a VM. Based on the costs, scalability, availability, and workflow analysis I chosed the web app service to deploy for my project article.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

I would choose virtual machines when security needs skyrocket and your application architecture explodes with microservices, diverse technologies and user growth, virtual machines (VMs) become attractive allies . Their inherent flexibility protects applications in isolated bubbles, enables granular resource allocation for security, and seamless integration of disparate technologies. Microservices thrive in individual VM houses, easily scaling to meet spikes in user demand. However, keep in mind the cost, management complexity when use virtual machine.