# AZ-140T00 Learning Path 2 – Implement an Azure Virtual Desktop Infrastructure Errata

# Active Directory Domain Services (AD DS)

## Lab 02 - Deploy host pools and session hosts by using the Azure portal (AD DS) ~60 Minutes

### Exercise 1: Implement an Azure Virtual Desktop environment in an AD DS domain

Task 2: Deploy an Azure Virtual Desktop host pool
Manually create a Resouce Group named az140-21-RG before starting the exercise
Step 2: select the az140-21-RG Resource Group

### Exercise 2: Validate Azure Virtual Desktop environment

Task 1: Install Microsoft Remote Desktop client (MSRDC) on a Windows 10 computer <br>
Step 8: after launching Edge, select the prompts to not sync account data - My have to click on Open file to run <br>


## Lab 03 - Implement and manage storage for AVD (AD DS) ~30 Minutes

### Exercise 1: Configure Azure Files to store profile containers for Azure Virtual Desktop <br>

Task 3:  Enable AD DS authentication for the Azure Storage account <br>
Step 2:  Expand v0.2.5 by clicking on Assets > click on AZFilesHybrid.zip to download the latest version <br>
Step 6:  When prompted select "Yes to All" <br>
Step 8:  Run the single cmdlet that starts with $storageaccount.  Verify the output looks like what is in the grey box <br>

Task 4:  Configure the Azure Files RBAC-based permissions <br>
Step 3:  you may have to exit back to Home then back to the file Share <br>
Step 5:  Paste the role in the search box, then select the role <br>
Step 7:  Paste the role in the search box, then select the role <br>

## Lab 04 - Deploy host pools and hosts by using Azure Resource Manager templates ~30 Minutes

### Exercise 1: Deploy Azure Virtual Desktop host pools and hosts by using Azure Resource Manager templates

Before beginning exercise manually create a Resourse Group named az140-23-RG in the region you have been uysing in previou labs <br>

Open notepad, copy and paste the items that you will be asked to take note <br>

Task 2:  Deploy an Azure Virtual Desktop host pool and hosts by using an Azure Resource Manager template <br>

Step 6:  Use the az140-23-RG resource group you created <br>

## Lab 05 - Deploy and manage host pools and hosts by using PowerShell ~60 Minutes

No errata

## Lab 06 - Create and manage session host images (AD DS) ~60 minutes 

### Exercise 1: Create and manage session host images

Task 2: Deploy Azure Bastion <br>
Replace steps 5 - 7 with the following <br>

In the Azure Portal - navigate to Virtual networks > az140-25-vnet > Settings > Bastion <br>
Click Deploy Bastion <br>

Task 3: Configure a Azure Virtual Desktop host image <br>
Step 10: Move the downloaded file from the downloads folder to the desired path <br>
Step 12: Move the downloaded file from the downloads folder to the desired path

Task 5:  Provision a Azure Virtual Desktop host pool by using a custom image <br>
Step 5:  Disregard selectign Image Type as the setting has been removed <br>

