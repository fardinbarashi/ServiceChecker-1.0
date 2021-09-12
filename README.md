# ServiceChecker-1.0
Servicechecker is a pscscript on how to monitor several services on different servers.

Monitoring of several different services in different servers in the same environment to reduce malfunctions when the services go down.


.Synopsis
   This script monitors services on different servers in one and the same environment.
.DESCRIPTION
   This script monitors services on different servers in one and the same environment.
   To make this script work, you need too change some strings.
    . $SmtpServer = "Your SMTP"
    . $MailFrom = "Your Mailbox" 
    . $Mailto = "TeamMailBox" 

    . $Server1 = "Server1.FQDN"
    . $Server2 = "Server2.FQDN"
    . $Server3 = "Server3.FQDN"

    . $Service1 = "ServiceName"
    . $Service2 = "ServiceName"
    . $Service3 = "ServiceName"


.EXAMPLE

   Run in shell or add to task-scheduler with elevated rights
   Start a Program : C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe
   Arguments : -File "FilePathToScript\Service-Checker 1-0.ps1" -NoLogo -NoProfile -WindowStyle Hidden
.OUTPUTS

   Script saves
   Logs : $LogPath
   Services Csv file : $PSScriptRoot\Csv\*
.NOTES

   Script uses Invoke-Command, the inviroment must allow ps-sessions. For more information
   https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/invoke-command?view=powershell-7.1

.FUNCTIONALITY

   Monitoring services

.LINKS

   Github : https://github.com/fardinbarashi
   Source Code : https://github.com/fardinbarashi/ServiceChecker-1.0 
   Linkedin : https://www.linkedin.com/in/fardin-barashi-a56310a2/
   Mail : Fardin.barashi@gmail.com

