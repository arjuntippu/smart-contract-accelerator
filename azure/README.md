# To deploy on Azure

Prerequisites
=============
Azure cloud account is mandatory to deploy this smart contract accelerator. Following the below link to create an azure account 

https://azure.microsoft.com/en-us/free/


Steps to deploy smart contract accelerator
==========================================

1. Click the below button, it will open "Deploy to Azure" screen to initiate the deployment

    [![Deploy to Azure](https://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/) 

2. Provide values for the following highligted mandatory fields and press "Next" to proceed further.
   
    "Admin Username / Admin Password" - Credentials to access virtual machine.
    
    "Dns Name for Public IP" - Unique name to access the admin panel 
    (ex http://testbcnw.eastus.cloudapp.azure.com:8090/login) 

3. "Preview" screen will show the list of azure resources will be created during the deployment. For this accelerator the following resources will be created. Press "Deploy" to start the deployment process.
    a. Microsoft.Network
    b. Microsoft.Compute

4. The following componenets will be deployed on azure and link will be provided to access the azure portal. This step will take 5 to 8 minutes to complete.
    a. Updating Microsoft.Network/publicIPAddresses
    b. Updating Microsoft.Network/virtualNetworks
    c. Updating Microsoft.Network/networkInterfaces
    d. Updating Microsoft.Compute/virtualMachines
    e. Updating Microsoft.Compute/virtualMachines/extensions 

5. Click "manage" link to access deployed resources from azure portal.

6. In azure portal, under "Settings", select "Deployments" then select the name under the column header "DEPLOYMENT NAME". This will open deployment overview screen.

7. In deployment overview screen, select "Output" and copy the URL from "ApplicationURL" field. Paste the URL on browser address bar to access admin panel.









