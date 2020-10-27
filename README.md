(Deprecated) Stop / Start all Azure classic VMs in parallel
===========================================================

            

**Updated at 05/17/2019 : This runbook is deprecated. You should use the new Az Powershell module by using [this runbook to stop / start VMs in parallel](https://gallery.technet.microsoft.com/scriptcenter/Stop-Start-all-or-only-8a7e11a2?redir=0) or [this runbook to stop /start VMs in sequence](https://gallery.technet.microsoft.com/scriptcenter/Az-Stop-Start-all-or-only-8a8fcab4?redir=0). **


**[See more about the new **Az PowerShell module for Azure**](https://docs.microsoft.com/en-us/powershell/azure/new-azureps-module-az?view=azps-2.0.0)**


**DESCRIPTION**


This PowerShell Workflow Runbook connects to Azure using an Automation Classic Run As account, retrieves the power status of Azure V1 VMs and turns off / on  in parallel those that are turned on / off. You can attach a recurring schedule to this
 runbook to run it at a specific time.


**REQUIRED**


1. An Automation connection asset called AzureClassicRunAsConnection that contains the information for connecting with Azure using a service principal.  To use an asset with a different name you can pass the asset name as a input parameter to this runbook.


2. An Action input parameter value that allows runbook to handle Azure V2 power state. The parameter must be set to 'Stop' or 'Start'.


**AUTHOR**


Farouk FRIHA


**LAST EDIT**


2016-12-03


**RELEASE NOTES**


2016-11-30 First release


2016-12-03 Handle changes to output


**RUNBOOK CONTENT**

** **




 


 


 


 


 


 



        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
