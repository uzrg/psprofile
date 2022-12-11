# psprofile
This project is a bundle of PowerShell Profiles customized to add several systems administration functions
The intent is to simplify my systems administration tasks with PowerShell by turning frequently used scripts into functions that are automatically loaded each time I launch PowerShell, thus I can call the functions as needed.
Depending on version of PowerShell, the following profiles must be placed at the proper locations such as:
($profile | select *)
PowerShell 5.1:
AllUsersAllHosts       : C:\Windows\System32\WindowsPowerShell\v1.0\profile.ps1
AllUsersCurrentHost    : C:\Windows\System32\WindowsPowerShell\v1.0\Microsoft.PowerShell_profile.ps1
CurrentUserAllHosts    : C:\Users\roger\Documents\WindowsPowerShell\profile.ps1
CurrentUserCurrentHost : C:\Users\roger\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1

ISE:
AllUsersAllHosts       : C:\Windows\System32\WindowsPowerShell\v1.0\profile.ps1
AllUsersCurrentHost    : C:\Windows\System32\WindowsPowerShell\v1.0\Microsoft.PowerShellISE_profile.ps1
CurrentUserAllHosts    : C:\Users\roger\Documents\WindowsPowerShell\profile.ps1
CurrentUserCurrentHost : C:\Users\roger\Documents\WindowsPowerShell\Microsoft.PowerShellISE_profile.ps1

PowerShell 7:

AllUsersAllHosts       : C:\Program Files\PowerShell\7-preview\profile.ps1
AllUsersCurrentHost    : C:\Program Files\PowerShell\7-preview\Microsoft.PowerShell_profile.ps1
CurrentUserAllHosts    : C:\Users\roger\Documents\PowerShell\profile.ps1
CurrentUserCurrentHost : C:\Users\roger\Documents\PowerShell\Microsoft.PowerShell_profile.ps1

VSCode:
AllUsersAllHosts       : C:\Program Files\PowerShell\7-preview\profile.ps1
AllUsersCurrentHost    : C:\Program Files\PowerShell\7-preview\Microsoft.VSCode_profile.ps1
CurrentUserAllHosts    : C:\Users\roger\Documents\PowerShell\profile.ps1
CurrentUserCurrentHost : C:\Users\roger\Documents\PowerShell\Microsoft.VSCode_profile.ps1

Also, there will be some minor environment specific customization/adjustments required to make the profile work in your environment.
Currently they are tailored to my homelab where everything is joined to the "myhomelab.lab" domain,should be simple to search and replace all myhomelab specific by your ouwn domain or environment to make the profiles work for you

Do not hesitate to make improvenents, suggestions, report issues etc ...


