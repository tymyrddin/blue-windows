# Maximise user account control (UAC)

Windows was designed as a single-user desktop system and has had various functionality added to it over time to address 
the weaknesses of the original design. A major weakness is that a desktop Windows user is also an admin-level user. 

User Account Control (UAC) was introduced in Windows Vista to create more of a barrier to installation and requires 
users to specifically authorise certain actions by clicking an OK button when prompted. By requiring administrator privileges to install programs, it is harder 
to deploy malware.

* In the search box type "Change user account control" and select the first result
* Move slider to Always notify me up top and click on OK

Now the machine always asks for the user’s permission before making any changes. And, the weakest link in any security chain is people. 

While these privilege escalation tools are fully functional, many people will simply type in their administrator 
password, or click the OK button to allow highly privileged activities to occur whenever the prompt comes up, without 
further thought.

In fact, this opens up another attack route for privilege escalation by an adversary. Presenting people with a spoofed 
pop-up box asking for the password, will usually work.

For better separation, you can [create a standard Windows account](../authentication/standard-user.md) yourself. 