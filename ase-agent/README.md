# Azure Pipelines Agent in Private Virtual Network for ASE

The Azure [App Service Environment (ASE)](https://docs.microsoft.com/en-us/azure/app-service/environment/intro) allows you to deploy Azure Web Apps into a private environment for enhanced security and access control. One challenge with this configuration is how to orchestrate Continuous Integration and Continuous Deployment (CI/CD) with [Azure DevOps Services](https://azure.microsoft.com/en-us/services/devops/) or [Azure DevOps Server](https://azure.microsoft.com/en-us/services/devops/server/) into such environments.

This template deploys an Azure Pipelines [self-hosted agent](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/v2-windows?view=azure-devops) into the Virtual Network where the ASE is deployed and connects this agent to an Azure DevOps instance. It also adds appropriate `hosts` file entries to the agent to allow it to deploy to a specific Web App in an ASE.

To ensure that the configuration of the agen is correct, you need to supply:

* `TSServerUrl`: Url of your Azure DevOps instance
* `AgentPool`: Name of the agent pool in the Azure DevOps instance (needs to be created in advance)
* `PAToken`: Personal Access Token for agent to register with the Azure DevOps instance
* `AseIp`: The IP address of the ASE environment.
* `AppDns`: The DNS name of the app, e.g. myapp.contoso-internal.us

<a href="https://transmogrify.azurewebsites.net/ase-agent/azuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
