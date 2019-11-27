SQL Insights ARM Template
-

This is a collection of ARM templates used to automate the deployment of Solutions, Extensions, Agents, and Workbooks.


### Deploy Solutions

##### Parameters required:
* workspace name

##### Solutions Installed in this template:
* SQLAdvancedThreatProtection
* SQLAssessment (SQL Health Check)
* SQLVulnerabilityAssessment
* AzureActivity

### Deploy Extensions

##### Parameters required:
* Mma Extension Version
* Da Extension Version
* Vm Type
* Vm Name
* Os Type
* Workspace Name

##### Agents Installed in this template:
* Mma Extension - This extension installs the OMS Agent on the VM
* Da Extension - This extension installs the Dependency Agent on the VM


##### Coming Soon
* Install pre-made workbooks along with the solutions with this template
* Connect Agent on VMs with this template
* Connect VM to Workspace with this template