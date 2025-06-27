# Outlook desktop prompts for credentials after 20 seconds.
* It’s *only affecting one user, **webmail (OWA) works fine*.
* You’ve already tried:

  * Creating a new Outlook profile
  * New data file
  * Added EnableADAL registry keys
  * Reinstalling Outlook

---

## 🎯 Most Likely Causes (Single User, Desktop-Only Issue)

### ✅ 1. *Corrupt Windows Credentials for Outlook*

* Open *Credential Manager* > Windows Credentials
* Remove *all* entries related to:

  * MicrosoftOffice16
  * Outlook
  * autodiscover
  * mail.avwequipment.com

💡 This is the #1 fix in many similar cases.

---

### ✅ 2. *Corrupt Autodiscover Cache*

Even though you created a new profile, sometimes the autodiscover.xml cache remains:

* Navigate to:

  
  C:\Users\<username>\AppData\Local\Microsoft\Outlook\
  

  Delete the *.xml files or rename the folder.

* Also delete:

  
  C:\Users\<username>\AppData\Local\Microsoft\Outlook\RoamCache
  

Then relaunch Outlook.

---

### ✅ 3. *Wrong Primary SMTP or Legacy DN Mapping*

If the user's mailbox was *recently migrated, renamed, or has a **new alias*, Outlook might be trying to connect with outdated data.

* Open *Outlook Profile* settings > Email Accounts > Repair
* Or recreate profile and double-check Set as default is pointing to correct SMTP address.

You can also run:

powershell
Get-Mailbox shipping | fl EmailAddresses


Ensure the *primary SMTP* (SMTP:) matches what Outlook is using.

---

### ✅ 4. *MAPI/HTTP Authentication Token Issue (Stuck Token)*

Try *forcing Basic Auth* for the user's profile to isolate the issue:

* In registry:

  
  HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Outlook\RPC
  

  Create or set:

  * EnableRPCEncryption = 1 (DWORD)
  * ProxyServerFlags = 3 (DWORD)

Also try starting Outlook with:

cmd
outlook.exe /safe


If Safe Mode works — it's likely an *add-in* or *stuck credential token* issue.

---

### ✅ 5. *Try Outlook Profile on Another PC*

If you haven’t yet:

> *Try logging into the same user's account on a different workstation.*

* If it works there → issue is *local to original machine*
* If not → issue is *server-side or user mailbox–specific*

---

### ✅ 6. *Reset Autodiscover SCP Redirection*

Sometimes a bad redirect causes loops. You can test this:

* Hold Ctrl + Right Click on Outlook icon in tray > *Test E-mail AutoConfiguration*
* Uncheck "Use Guesssmart" and "Secure Guessmart"
* Click *Test*

See if the autodiscover URL is correct and consistent. If it fails or loops to external sources, it needs a fix on the Exchange SCP side:

powershell
Get-ClientAccessService | fl AutoDiscoverServiceInternalUri


---

## ✅ Final Option: Recreate Windows User Profile

If *all else fails*, and only one user on one machine is affected:

> Try logging in with a *new Windows user account* (not just Outlook profile).

Corruption in the user's *Windows profile* can cause persistent auth issues in Outlook.

---

Let me know what happens after trying:

* Deleting credentials
* Clearing RoamCache
* Testing on a second machine

I can guide further based on the result.
