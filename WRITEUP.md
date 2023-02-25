# Write-up Template
[My app service](https://quyetnt7.azurewebsites.net/)
### Analyze, choose, and justify the appropriate resource option for deploying the app.
- **Cost**: Use VM because it provides enough free plan for me to use in this project. But in terms of cost, up to now, App Service is cheaper than VM, in the picture below, I'm trying to estimate between the two sides.
![compare-cost](https://github.com/ntrongquyet/Deploy-An-Article-CMS-To-Azure/blob/main/example_images/compare-cost.png?raw=true)
- **Scalability**: We can easily scale our application horizontally or vertically.
    - **Vertically**: scaling increases or decreases resources allocated to our App Service, such as the amount of vCPUs or RAM, by changing the App Service pricing tier.
    - **Horizontal**: scaling increases or decreases the number of Virtual Machine instances our App Service is running.
- **Availability**: Locations of Azure data centers of Microsoft around the world so I can host my app service everywhere with high availability. But as me know, free tier no provide SLA.
- **Workflow**: We can do continuous deployment using GitHub, Azure DevOps or any Git repo.

#### The reason why I choose App Service
- ***Azure App Service*** can support Python as well as many other languages such as ASP.NET, ASP.NET Core, Java, Ruby, Node.js and PHP.
-  App Service which help us deploy application quickly and just take care of our applications and data. The rest is already handled by cloud provider because ***Azure App Service*** is a **PaaS**.
### Assess app changes that would change your decision.
-  ***Azure App Service*** is a Pass, so it will be limited to operating system management. So if I need intervention to change, I will use VM.
-  ***Azure App Service***  limit of up to 14 GB or 4 CPU cores on the highest tier, so if my application has a large number of users in the future and many function will added. I will choice Virtual Machine.