# Write-up Template
[My app service](https://quyetnt7.azurewebsites.net/)

### Analyze, choose, and justify the appropriate resource option for deploying the app.
# The reason why I choose App Service
- ***Azure App Service*** can support Python as well as many other languages such as ASP.NET, ASP.NET Core, Java, Ruby, Node.js and PHP.
-  App Service which help us deploy application quickly and just take care of our applications and data. The rest is already handled by cloud provider because ***Azure App Service*** is a **PaaS**.

### Assess app changes that would change your decision.
-  ***Azure App Service*** is a Pass, so it will be limited to operating system management. So if I need intervention to change, I will use VM.
-  ***Azure App Service***  limit of up to 14 GB or 4 CPU cores on the highest tier, so if my application has a large number of users in the future and many function will added. I will choice Virtual Machine.