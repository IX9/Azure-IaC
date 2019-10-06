# ST81-IaC


### Azure CLI
    azure login
    azure group deployment create -g RG-ARMTEST-AuEast --template-file webserver.json --parameters-file parameters/webserver-parameters.json


### Powershell

    Connect-AzureRmAccount

    New-azurermresourcegroupdeployment -resourcegroupname RG-ARMTEST-AuEast -Name WebDeployment -DeploymentDebugLogLevel All -TemplateFile .\webservers\webserver.json -TemplateParameterFile .\webservers\parameters\webserver-parameters.json

