# DevTest_ARM

This repo is a set of Azure ARM Templates and corresponding Parameters files that will help to automate the creation and management of Azure DevTest Labs and Lab Services. Make sure to set the parameters files to contain your own specific values.

## Deployment

To leverage these templates, clone the repo into either you local folder or into your Azure Cloud Shell Storage Account and then run either the following Azure CLI or Azure PowerShell commands:

Azure CLI: az deployment group create --resource-group <group-name> --name <lab-name> --template-file azuredeploydevtest.json --parameters @azuredeploydevtest.parameters.json

Other examples can be found at the following location: [Deploy-CLI](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/deploy-cli)

---------------------------------

Azure PS: New-AzResourceGroupDeployment -ResourceGroupName <group-name> -TemplateFile azuredeploydevtest.json -TemplateParameterFile azuredeploydevtest.parameters.json

Other examples can be found at the following location: [Deploy-Powershell](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/deploy-powershell)

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.