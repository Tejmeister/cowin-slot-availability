# cowin-slot-availability

## Description
This Azure Logic App template regularly polls the public API of cowin for specified pincodes and sends an SMS to the registered mobile number whenver a vaccination slot is available.

## Technologies used:
1. Microsoft Azure Logic App
2. Twilio to send SMS

## Usage
You can override the parameters of the logic app in the parameters.json and use Azure Powershell Command to deploy the logic app to your azure account.

The command to be used is:
```
New-AzResourceGroupDeployment `
	-Name <DEPLOYMENT_NAME> `
	-ResourceGroup <RESOURCE_GROUP> `
	-TemplateFile <TEMPLATE_FILE_PATH> `
	-TemplateParameterFile <PARAMETERS_FILE_PATH>
	
```
