# Separation principle

Windows was designed as a single-user desktop system and has had various functionality added to it over time to address 
the weaknesses of the original design. A major weakness is that a desktop Windows user is also an admin-level user. 

[User Account Control (UAC)](../services/max-uac) was introduced 
in Windows Vista to create more of a barrier to installation and requires users to specifically authorise certain 
actions by clicking an OK button when prompted. By requiring administrator privileges to install programs, it is harder 
to deploy malware. And, the weakest link in any security chain is people. While these privilege escalation tools are 
fully functional, many people will simply type in their administrator password, or click the OK button to allow highly 
privileged activities to occur whenever the prompt comes up, without further thought.

In fact, this opens up another attack route for privilege escalation by an adversary. Presenting people with a spoofed 
pop-up box asking for the password, will usually work.

For better separation, you can 
[create a standard Windows account](standard-user) yourself. Now the user 
account has fewer privileges, but when you need to perform a task that requires administrator rights, you 
can right-click an app and use the Run as Administrator option with the credentials of the administrator account you 
just created. Stay aware, awake and alert!