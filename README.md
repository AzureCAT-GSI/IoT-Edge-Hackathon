# IoT-Edge-Hackathon

Description of hackathon to be added here...

## Deployment

Instructions to deploy the resources necessary to complete the hackathon pre-work are described below.  You can use PowerShell or Bash to deploy the resources.

The deployment will take about 40+ minutes to deploy.  The resources that are deployed are
- Azure IotHub
- Virtual machine running Debian 8 to act as an IoT edge gateway
- - Custom script extension that downloads the Azure IoT Gateway SDK and installs the Gateway.  This is where the majority of the deployment time exists.
- Virtual machine running Debian 8 to act as a ModBus Slave (device simulator)

### PowerShell

#### Requirements

Download and install the [Azure PowerShell cmdlets](https://www.microsoft.com/web/handlers/webpi.ashx/getinstaller/WindowsAzurePowershellGet.3f.3f.3fnew.appids) if you don't already have them installed.  

```PowerShell
# Sign-in to your Azure Subscription
Login-AzureRmAccount

# Deploy the resources to a resource group named 'SLB-Hackathon'.  
# - To change the resource group name, provide the -ResourceGroupName parameter.
.\Deploy-AzureResourceGroup.ps1 -ResourceGroupLocation westus
```

### Bash

Instructions to be added...

```bash
```



