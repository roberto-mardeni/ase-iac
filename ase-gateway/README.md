# Integrate your ILB App Service Environment with the Azure Application Gateway

This template illustrates how to deploy an [Azure Application Gateway](https://docs.microsoft.com/en-us/azure/app-service/environment/integrate-with-application-gateway) to integrate with an [Azure App Service Environment](https://docs.microsoft.com/en-us/azure/app-service/environment/intro) a.k.a. ASEv2 with ILB configuration.

## Prerequisites

You will need certificates for this to successfully deploy. These can be valid certificates, or self-signed certificates (for demo and testing purposes). Specifically, you will need the following certs:

- **Front End Certificate**: This is the certificate that will terminate SSL on the Application Gateway for traffic coming from the internet. This will need to be in .pfx format, and will need to be encoded in base-64 in order to include in the template deployment.
- **Back End Certificate**: This is the certificate that will be installed on the IIS servers to encrypt traffic between the Application Gateway and the IIS servers. This could be the same as the front end certificate or could be a different certificate. This will need to be in .pfx format, and will need to be encoded in base-64 in order to include in the template deployment.
- **Back End Public Key**: This is the public key from the back end certificate that will be used by the Application Gateway to whitelist the back end servers. This will need to be in .cer format, and will need to be encoded in base-64 in order to include in the template deployment.

The script [PrepareAseDeployment.ps1](../scripts/PrepareAseDeployment.ps1) helps you to get the values to provide for the template.

<a href="https://transmogrify.azurewebsites.net/ase-gateway/azuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
