# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- VMs are more costly than web apps (although web apps can overcome VMs in cost in limited situations as web apps are not pay-as-you-go). Pricings can be calculated through the pricing calculator that is provided by azure. In our situation I don't think cost matter that much with the current scale of the project, but anyhow, that is a point for web apps.
- Since we are using python, it is more reasonable to work on app service as it already support this language. 
- VM gives you more control over the operating system. However, in this project, there is no need for this much control.
- The project is about deploying articles, and looking at the current scope, it is not expected to get expanded in the future. It is a small-scale project that requires a short duration of development and a small team (in my case it's just me :)). Given these factors, and as web apps gives us minimal managerial responsibilities (which is a good thing in terms of abstraction), web apps would be a good choice. 
- Both VMs and Web apps gives you access to multiple regions (even in the middle east), so they are both equal in terms of availability.

Given the points above, choosing web apps would be a good decision given the reasons that:
1- We do not need that much of control over OS
2- It is a small-scale project that does not require heavy resources
3- Availability is a non-issue
4- Project language is already supported by app service
5- Cost is estimated to be less using app service


### Assess app changes that would change your decision.

- If we were to use another programming language, then we would reside to VM.
- If we need more control over the operating system, then we would choose VM.
- If the project were to be scaled up and we needed to use higher amount of CPU, RAM, and storage, then we would choose VM
