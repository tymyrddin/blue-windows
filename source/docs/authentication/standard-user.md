# Use a standard user account

Users with administrator privileges have complete control over the OS and their apps have unrestricted access to the 
computer. Even when keeping up with system and antivirus updates, following the best security practices, and being 
careful using the internet and checking email attachments, there is still a chance that malware could gain access to 
your device.

Running as administrator, an exploit can more easily gain control of your system. It can install rootkits, keyloggers, 
and other suspect services without you knowing. A malicious program can also modify and delete files, and even prevent 
devices from booting. 

Consider setting up a separate standard user account with fewer privileges for day-to-day use. This can block some 
attacks and make others much harder.

## Create a new administrator account

* Settings -> Accounts -> Family & other people.
* Under Other People, click the Add someone else to this PC option.
* Click the "I don't have this person's sign-in information" link. 
* Click the "Add a user without a Microsoft account link": Because the account will only be used for administrative tasks you do not need to create a new Windows 10 account using a Microsoft account.
* Type the username and password you want to use for the admin account. Next
* Select the newly created account, and click Change account type.
* In the "Account type" drop-down menu, select Administrator. OK.

## Change your user account type

An Administrator account is a member of the Administrators and Users groups, which means that to make the account a 
Standard User, you only need to remove your account from the Administrators group. Sign-in to the newly created admin 
account to change your user account type to Standard User using the Settings app.

* Type Computer Management in search box and click the result to open the console.
* Go to System Tools -> Local Users and Groups -> Users
* Double-click your user account — the one you want to switch to remove the privileges from.
* Click on Member Of tab.
* Select Administrators from the list.
* Click the Remove button.
* Apply and OK.
* Sign out and sign back in to apply the changes.

You have turned your account into a standard user account with fewer privileges and apps will not be allowed to make 
system changes, making your system more secure against malware. When you need to perform a task that requires 
administrator rights, you can right-click the app and use the Run as Administrator option with the credentials of the 
administrator account you just created.


