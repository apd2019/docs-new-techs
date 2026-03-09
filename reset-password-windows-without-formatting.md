What is this tutorial about?
* if you forgot your password and are not able to remember it and wish to reset the whole system or format it.

WorkFlow-
* press shift while restarting the system and hold until the booting menu loads
* go to the Troubleshoot option
* Go to Advanced option
* Go to command prompt

It will show something like-
X:\Windows\System32 (it's temporary RAM drive OR the recovery drive and not the real system drive)

You will need to type in some commands.

* change the directory to the system directory/drive - C:\ OR whatever is your system drive or the OS partition drive
* Type in - cd Windows > Press Enter
* Type in - System32 > press Enter
* Type in - dir /p and scroll to see if these files appear- cmd.exe, utilman.exe

Now the flow will be like this-
* rename the utilman.exe to something like utilman.old
* copy the cmd.exe as utilman.exe
* so that the accessibility icon is replaced with the cmd on the sign in screen
* click the accessibility icon > cmd appears > type in some commands to reset your password

Actions-

* **Rename the utilman.exe to something like utilman.old**
* type in - ren utilman.exe utilman.old
* **copy the cmd.exe as utilman.exe**
* type in - copy cmd.exe utilman.exe
* type in - exit > press Enter
* click Continue to restart the system
* click the accessbility button on the windows sign in screen > cmd appears
* type in - net user (to see the users on the computer)
* type in - net user your-username new-password
* it would ask to confirm the password
* Exit
* That's it:)

Blocker

Sometimes, cmd.exe can't be found in System32 and would be present in the SysWoW folder instead as 32bit version.
On 64 bits system, 32bit cmd can be run as well.

Workflow-
* You will need to copy that cmd.exe from the sysWoW folder to the System32 folder
* Rename the utilman.exe to something like utilman.old
* copy the cmd.exe as utilman.exe so the accessibility icon can run cmd on the start up screen

Actions-
* **You will need to copy that cmd.exe from the sysWoW folder to the System32 folder**
* copy e:\Windows\SysWOW\cmd.exe e:\Windows\System32
* **copy the rename the utilman.exe to something like utilman.old**
* 
