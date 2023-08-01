# AZ-140T00 All Module Errata

# Active Directory Domain Services (AD DS)

# Learning Path 1 – Plan an Azure Virtual Desktop Implementation

# AZ-140T00 Learning Path 1 – Plan an Azure Virtual Desktop Implementation

## Lab - Prepare for deployment of Azure Virtual Desktop (AD DS) ~75 Minutes

### Exercise 0:  Increase the number of vCPU quota

Task 1:  Identify current vCPU usage <br>
Step 6:  Copy and paste each line induviually, replace '<Azure_region>' with 'eastus', copy and paste the other 2 cmdlets <br>

Task 2:  Request vCPU quota increase <br>
Step 6:  If prompted for MFA, follow the promtps to authenticate with MFA - Use dropdown box to select phone number - -  redo steps 3 - 5 <br>

## Do not close the quota request window until the request has been approved.

### Exercise 1:  Deploy an Active Directory Domain Services (AD DS) domain

Task 2:  Deploy an Azure VM running an AD DS domain controller by using an Azure Resource Manager QuickStart template <br>
Step 1:  Copy and paste each line induviually, replace '<Azure_region>' with 'eastus', copy and paste the other 2 cmdlets <br>
Step 6:  you can also browse to the file, it is located on the F drive in Allfiles>Labs>01 folder <br>

Task 4: Deploy Azure Bastion <br>\
2 Options <br>

Open another browser window <br>

### Option 1 - alternate way to deply Bastion

Navigate to Virtual networks > az140-adds-vnet11 > Settings > Bastion <br>
Click Deploy Bastion <br>

### Option 2 - Bastion work around - Connect to DC11 directly with RDP instead of Bastion (My preferred way for the lab)
1.  In the Azure portal, Search for Public Ip <br>
2.  Select Publi IP Address
3.  Select Create
4.  Select az140-11-RG resource group <br>
5.  Select region used in previous steps <br>
6.  Give it a name <br>
7.  Choose no Zone redundancy <br>
8.  Use (initials)Adatum for DNS name <br>
9.  Select Review + create then Create <br>
10. In the Azure Portal Browse to Virtual Machines > az140-dc-vm11 > Settings > Networking <br>
11.  Select the Network Interface <br>
12.  Browse to Settings > Network Security Group - Select the az140-cl-vm11-ngs in the dropdown box <br>
13.  Select Save <br>
14.  Browse to Settings > IP configuration > Ipconfig <br>
15.  Check Associate public IP address > Choose in dropdown box the name you created above <br>
16.  Select Save <br>

In the overview pane of the VM select Connect then RDP . Download the file then open it <br>
Credentials are Studnet   Pa55w.rd  <br>

### Exercise 2: Integrate an AD DS forest with an Azure AD tenant

While in the PowerShell ISE delete each entry form the previous step from the pane before pasting the nest step <br>

Task 4: Install Azure AD Connect <br>
Step 3:  after installing Edge, select the prompts to not sync account data <br>
Step 13: you can copy the UPN from the Azure AAD portal <br>

# AZ-140T00 Learning Path 2 – Implement an Azure Virtual Desktop Infrastructure Errata

# Active Directory Domain Services (AD DS)

## Lab - Deploy host pools and session hosts by using the Azure portal (AD DS) ~60 Minutes

### Exercise 1: Implement an Azure Virtual Desktop environment in an AD DS domain

Task 2: Deploy an Azure Virtual Desktop host pool <br>
Manually create a Resouce Group named az140-21-RG before starting the exercise <br>
Step 2: select the az140-21-RG Resource Group <br>

### Exercise 2: Validate Azure Virtual Desktop environment

Task 1: Install Microsoft Remote Desktop client (MSRDC) on a Windows 10 computer <br>
Step 8:  Step 8:  after launching Edge, select the prompts to not sync account data - My have to click on Open file to run <br>

## Lab - Implement and manage storage for AVD (AD DS) ~30 Minutes

### Exercise 1: Configure Azure Files to store profile containers for Azure Virtual Desktop <br>

Task 3: Enable AD DS authentication for the Azure Storage account <br>
Step 2: Expand v0.2.5 by clicking on Assets > click on AZFilesHybrid.zip to download the latest version <br>
Step 6:  When prompted select "Yes to All" <br>
Step 8:  Run the single cmdlet that starts with $storageaccount.  Verify the output looks like what is in the grey box <br>

Task 4: Configure the Azure Files RBAC-based permissions <br>
Step 3:  you may have to exit back to Home then back to the file Share <br>
Step 5:  Paste the role in the search box, then select the role <br>
Step 7:  Paste the role in the search box, then select the role <br>

## Lab - Deploy  host pools and hosts by using Azure Resource Manager templates ~30 Minutes

### Exercise 1: Deploy Azure Virtual Desktop host pools and hosts by using Azure Resource Manager templates

Before beginning exercise manually create a Resourse Group named az140-23-RG in the region you have been uysing in previou labs <br>

Open notepad, copy and paste the items that you will be asked to take note <br>

Task 2: Deploy an Azure Virtual Desktop host pool and hosts by using an Azure Resource Manager template <br>

Step 6:  Use the az140-23-RG resource group you created <br>

## Lab - Deploy and manage host pools and hosts by using PowerShell ~60 Minutes

No errata <br>

## Lab - Create and manage session host images (AD DS) ~60 minutes 

### Exercise 1: Create and manage session host images

Task 3: Configure a Azure Virtual Desktop host image <br>
Step 10: Move the downloaded file from the downloads folder to the desired path <br>
Step 12: Move the downloaded file from the downloads folder to the desired path

Task 5: Provision a Azure Virtual Desktop host pool by using a custom image <br>
Step 5:  Disregard selectign Image Type as the setting has been removed <br>

# Learning Path 3 – Manage access and security for Azure Virtual Desktops Errata

## Lab - Configure Conditional Access policies for WVD (AD DS)

Before starting the lab you will need to configure a Premium P2 license.  Use the following steps if needed. <br>

From your lab computer, start a web browser, navigate to the https://portal.azure.com, and sign in by providing credentials of a user account with the Owner role in the subscription you will be using in this lab and the Global Administrator role in the Azure AD tenant associated with that subscription.<br>

In the Azure portal, search for and select Azure Active Directory to navigate to the Azure AD tenant associated with the Azure subscription you are using for this lab.<br>

In the Azure portal, navigate back to the Overview blade of the Azure AD tenant and, in the vertical menu bar on the left side, in the Manage section, click Licenses.<br>

On the Licenses | Overview blade, in the vertical menu bar on the left side, in the Manage section, click All products.<br>

On the Licenses | All products blade, in the toolbar, click + Try/Buy.<br>

On the Activate blade, click Free trial in the Azure Premium P2 section and then click Activate.<br>

While on the Licenses | Overview blade, refresh the browser window to verify that the activation was successful.<br>

### Exercise 1: Prepare for Azure AD-based Conditional Access for Azure Virtual Desktop

Task 3: Register a user for Azure AD MFA<br>
Step 3:  Select "I want to set up a different method".  In the choose method drop down box choose Phone, click Confirm<br>

### Exercise 2: Implement Azure AD-based Conditional Access for Azure Virtual Desktop

Task 1: Create an Azure AD-based Conditional Access policy for all Azure Virtual Desktop connections<br>
Step 4:  May have to search for Microsoft Remote Desktop instead of the GUID<br>




