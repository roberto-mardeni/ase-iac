# Integrate your ILB App Service Environment with the Azure Application Gateway

This template illustrates how to deploy an [Azure Application Gateway](https://docs.microsoft.com/en-us/azure/app-service/environment/integrate-with-application-gateway) to integrate with an [Azure App Service Environment](https://docs.microsoft.com/en-us/azure/app-service/environment/intro) a.k.a. ASEv2 with ILB configuration.

The template allows you to supply an existing Subnet for ASE deployment (there should be no resources in this Subnet). If you do not supply a Subnet, i.e. leave that parameter as `null`, a new Virtual Network will be created and the ASE deployed in it.

<a href="https://transmogrify.azurewebsites.net/ase-gateway/azuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
