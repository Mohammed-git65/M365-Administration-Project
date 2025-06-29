I had a Microsoft 365 Office case and it was good to share.

A user said: *My Office apps keep asking me to sign in every day*. 

They were using Office 365 apps on Windows 10. 

They had a valid Microsoft 365 Business license. 

We checked: 
 - License was assigned 
 - Device was Azure AD joined 
 - No policy blocking sign-in 
 - No network issues 
 - Activation was OK

Still, the user had to sign in every day. Outlook and Word showed "Sign in required" often. 

So I checked Office identity settings using PowerShell: 
Get-ItemProperty -Path "HKCU:\Software\Microsoft\Office\16.0\Common\Identity" | fl 

And I found this: 
EnableADAL : 0 Version : 1 
This means Modern Authentication was off on the device. Office was falling back to basic auth, so it couldn’t keep the session. 
To fix it, I enabled Modern Authentication with this command: 
Set-ItemProperty -Path "HKCU:\Software\Microsoft\Office\16.0\Common\Identity" -Name EnableADAL -Value 1 
After restarting Office, the sign-in stayed active. No more daily prompts. 
