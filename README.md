SQL Insights ARM Template
-

This is a collection of ARM templates used to automate the deployment of Solutions, Extensions, Agents, and Workbooks.


### Deploy Solutions

##### Parameters required:
| Parameter      | Type   |
|----------------|--------|
| workspace name | String |

##### Solutions Installed in this template:
* SQLAdvancedThreatProtection
* SQLAssessment (SQL Health Check)
* SQLVulnerabilityAssessment
* AzureActivity

### Deploy Extensions

##### Parameters required:
| Parameter             | Type   | Description                                                      |
|-----------------------|--------|------------------------------------------------------------------|
| Mma Extension Version | String | MMA/OMS Extension Version. Currently: Windows - 1.0, Linux - 1.4 |
| Da Extension Version  | String | Dependency Agent Extension Version.                              |
| Vm Type               | String | VM type: 1. virtualMachines, 2 virtualMachineScaleSets.          |
| Workspace Name        | String |                                                                  |
| Vm Name               | String |                                                                  |
| Os Type               | String | Operating System. Example Windows or Linux                       |

##### Agents Installed in this template:
* Mma Extension - This extension installs the OMS Agent on the VM
* Da Extension - This extension installs the Dependency Agent on the VM


----
##### Coming Soon
* Install pre-made workbooks along with the solutions with this template
* Connect Agent on VMs with this template
* Connect VM to Workspace with this template