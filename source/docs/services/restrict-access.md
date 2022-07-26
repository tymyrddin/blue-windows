# Restricting access to applications

## Examples

### Restrict application access to email application

* Go to Settings -> Privacy
* Click on Email from the left menu
* Toggle off the app access to emails. 

This will ensure that applications have no access to your emails, unless ... Under the “Choose app that can access and 
send email” section, you can allow access to any specific applications that need email accessed.

### Any application to users using Group Policy Editor

This method is only possible if you have Windows 10 Pro or Enterprise:

* In the search box, type `gpedit.msc`, and select OK.
* Click on User Configuration on the left sidebar.
* Go to Administrative Templates folder.
* Go to the System folder.
* Locate the Don’t run specified Windows applications file on the right pane.
* Double-click on it. This will open a new window.
* On the left side of the window, check the Enabled circle.
* Under Options, go to Show.
* Type in the name of the app you want to restrict access to. Don’t forget to add the `.exe` extension after the name of the app.
* Apply.
* OK.

### Program Blocker

There are many third-party programs on the Internet that you can use to restrict applications. They will simply lock the 
applications and password-protect them. Try 
[AskAdmin](https://www.softpedia.com/get/Security/Security-Related/AppAdmin.shtml) or 
[Program Blocker](https://www.softpedia.com/get/PORTABLE-SOFTWARE/Security/d7xtech-Program-Blocker.shtml)
