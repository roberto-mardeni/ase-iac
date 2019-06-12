# ase-iac

Azure App Service Environment - Infrastructure as Code

This repository contains templates for deploying infrastructure in Microsoft [Azure](https://azure.microsoft.com/en-us/).

* [ase](ase/) is a template to deploy Azure App Service Environment (ASE) into an existing or new Virtual Network.
* [ase-agent](ase-agent/) is a template for deploying a VSTS/TFS build agent into a Virtual Network and let it deploy to a Web App in an App Service Environment (ASE).
* [ase-devops](ase-devops/) is a combination of [ase](ase/) and [ase-agent](ase-agent/) to demonstrate the complete ASE Azure DevOps experience.

## Credits

This repository was created based on https://github.com/hansenms/iac
