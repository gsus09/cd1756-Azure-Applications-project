# Write-up
App Deployement using Microsoft Azure

## Analyze, choose, and justify the appropriate resource option for deploying the app.

### Feature comparison
 **Criteria**           | **Azure Virtual Machine (VM)**                                 | **Azure App Service**                                           |
|------------------------|----------------------------------------------------------------|------------------------------------------------------------------|
| **Cost**               | Higher: Pay for compute, storage, network, and licenses        | Lower: Pay-as-you-go, includes auto-scaling                     |
| **Scalability**        | Manual or via VM Scale Sets                                    | Automatic horizontal scaling with minimal setup                 |
| **Availability**       | High, but requires configuration (e.g., Availability Sets)     | High, built-in SLA (99.95%)                                     |
| **Workflow**       | - Offers flexibility in deployment workflows. <br>- Requires manual setup for CI/CD pipelines.     | - Provides built-in deployment options like GitHub, Azure DevOps, FTP, and ZIP deploy.<br>- Supports automated CI/CD with minimal configuration.                                     |

### Appropriate solution
The appropriate solution for deploying this web application is App Service.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.*

- if I got special requirements to install a special set of software what is not covered in the options of Azure App Service --> than I need to switch to a VM service
- if I need full control over the os
- if I need full control over the network configuration