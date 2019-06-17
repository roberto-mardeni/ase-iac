# ase-iac

Azure App Service Environment - Infrastructure as Code

This repository contains templates for deploying infrastructure in Microsoft [Azure](https://azure.microsoft.com/en-us/).

* [ase](ase/) is a template to deploy Azure App Service Environment (ASE) into an existing or new Virtual Network.
* [ase-agent](ase-agent/) is a template for deploying an Azure Pipelines agent into a Virtual Network and let it deploy to a Web App in an App Service Environment (ASE).
* [ase-devops](ase-devops/) is a combination of [ase](ase/), [ase-agent](ase-agent/) and [ase-gateway](ase-gateway/) to demonstrate the complete ASE Azure DevOps experience.
* [ase-gateway](ase-gateway/) is a template for deploying an Azure Application Gateway to allow public traffic into the sites in the App Service Environment (ASE).

## Credits

This repository was created based on https://github.com/hansenms/iac
