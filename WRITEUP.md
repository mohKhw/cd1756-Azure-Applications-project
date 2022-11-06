# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- Web app can consume more cost than VM depending on the properties, but in general VM is more costly.
-Since we are using python, it is more reasonable to work on app service as it already contain this language. If we were to use another language that is not available on app service, then VM would be the choice.
-VM gives you more control over the operating system. However, in this project, there is no need for this much control.
-The project is considered small-scale so app services is much suitable.


### Assess app changes that would change your decision.

- If we were to use another programming language, then we would reside to VM.
- If we need more control over the operating system, then we would choose VM.
