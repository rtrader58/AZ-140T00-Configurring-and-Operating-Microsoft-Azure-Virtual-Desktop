# AZ-140T00 Learning Path 1 – Plan an Azure Virtual Desktop Implementation

# Active Directory Domain Services (AD DS)

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

Task 4: Deploy Azure Bastion
Open another browser window and connect to the Azure Portal

### Exercise 2: Integrate an AD DS forest with an Azure AD tenant

While in the PowerShell ISE delete each entry form the previous step from the pane before pasting the nest step

Task 4: Install Azure AD Connect
Step 3:  after installing Edge, select the prompts to not sync account data
Step 13: you can copy the UPN from the Azure AAD portal
