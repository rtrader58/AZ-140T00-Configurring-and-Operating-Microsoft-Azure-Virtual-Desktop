# Learning Path 5 – Monitor and maintain an Azure Virtual Desktop infrastructure

## Lab – Implement autoscaling in host pools (AD DS) ~60 Minutes

### Exercise 3: Stop and deallocate Azure VMs provisioned in the lab


*** Note*** If you want to accomplish the alternate Azure ADDS Track you will need to remove the current Azure AD Connect Syncing.  Do the following steps before deallocating the environment.  <br>

Do the following tasks before doing Task 1 of the lab environment steps <br>

1. Use the Bastion to connect to az140-dc-vm11 <br>
2. In the Windows PowerShell console, enter the following command and press Enter to install the Microsoft Online module for Azure AD:
Install-Module -Name MSOnline <br>
3. When prompted to install the NuGet provider, enter Y, and then press Enter. <br>
4.  When prompted to install the modules from an untrusted repository, enter A, and then press Enter. <br>
5. In the Windows PowerShell console, enter the following command, and then press Enter to store Azure AD credentials in a variable:
$msolCred = Get-Credential <br>
6. In the Windows PowerShell credential request dialog box, enter the credentials of the Azure AD Global Administrator user account you created in exercise 1, and then select OK. <br>
7. In the Windows PowerShell console, enter the following command, and then press Enter to authenticate to the Azure AD tenant:
Connect-MsolService -Credential $msolCred <br>
8. Enter the following command and press Enter to disable directory synchronization:
Set-MsolDirSyncEnabled -EnableDirSync $false <br>
9. When prompted to confirm, enter Y, and then press Enter. <br>
10. On az140-dc-vm11, on the Start menu, select Control Panel. <br>
11. In the Control Panel window, under Programs, select Uninstall a program. <br>
12. In the Uninstall or change a program window, select Microsoft Azure AD Connect, and then select Uninstall. <br>
13. In the Programs and features dialog box, select Yes. <br>
14. In the Uninstall Azure AD Connect window, select Remove. <br>
15. After Azure AD Connect is uninstalled, in the Uninstall Azure AD Connect window, select Exit <br>
