To show hidden files on Windows, you can use the following command in PowerShell:


powershell
Set-ItemProperty -Path 'HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced' -Name Hidden -Value 1

Explanation:


Set-ItemProperty: Cmdlet to set the value of a property in a specified registry key.
-Path 'HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced': Specifies the registry key path for Explorer advanced settings.
-Name Hidden -Value 1: Sets the 'Hidden' property to 1, which enables the display of hidden files.

Make sure to run PowerShell as an administrator for the changes to take effect.
