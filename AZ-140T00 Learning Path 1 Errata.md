# AZ-140T00 Learning Path 1 – Plan an Azure Virtual Desktop Implementation

# Active Directory Domain Services (AD DS)

## Lab - Prepare for deployment of Azure Virtual Desktop (AD DS) ~75 Minutes

### Exercise 0:  Increase the number of vCPU quota

Task 1:  Identify current vCPU usage <br>
Step 6:  Open Notepad on Lab Computer.  Paste Cmdlets into notepad, replace '<Azure_region>' with 'eastus', copy and paste into Cloud Shell <br>

Task 2:  Request vCPU quota increase <br>
Step 6:  If prompted for MFA, follow the promtps to authenticate with MFA - Use dropdown box to select phone number - -  redo steps 3 - 5 <br>

## Do not close the quota request window until the request has been approved.

### Exercise 1:  Deploy an Active Directory Domain Services (AD DS) domain

Task 2:  Deploy an Azure VM running an AD DS domain controller by using an Azure Resource Manager QuickStart template <br>
Step 1:  Copy and paste each line induviually, replace '<Azure_region>' with 'eastus', copy and paste the other 2 cmdlets <br>
Step 6:  you can also browse to the file, it is located on the F drive in Allfiles>Labs>01 folder <br>

Task 4: Deploy Azure Bastion <br>\
2 Options <br>

### Option 1 Connecting through the Bastion Host as written in the lab <br>

### Option 2 - Bastion work around - Connect to DC11 directly with RDP instead of Bastion (My preferred way for the lab)

##  *** Using this method will expose your Domain Controller directly to the Internet.  There is a risk your DC could be compromised and your labs will no longer work ***

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
Credentials are Student   Pa55w.rd1234  <br>

### Exercise 2: Integrate an AD DS forest with an Azure AD tenant

While in the PowerShell ISE delete each entry form the previous step from the pane before pasting the nest step <br>

Task 4: Install Azure AD Connect <br>
Step 3:  after installing Edge, select the prompts to not sync account data <br>
Step 13: you can copy the UPN from the Azure AAD portal <br>
