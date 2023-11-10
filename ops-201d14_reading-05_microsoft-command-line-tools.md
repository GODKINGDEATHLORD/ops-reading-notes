# Reading 05- Microsoft Command Line Tools- CompTIA A+ 220-1002-1.4

## How can you list the files in the current directory using the command prompt?
dir- list files and directories
cd- change directory  cd \ specifys volume or series
.. go back a folder


## How might the “sfc” command and the “gpupdate” command help in troubleshooting on Windows?
system file checker, scans the integrity of all protected system files ,and will identify, and repair files, 
managing group policy- will allow the system administrator to update all the computers at once , which will force an update to a computer
-gpupdate /target: {computer|user} /force
-gpupdate /target:professor /force
gpresult
-gpresult /r
gpresult /user sgc/professsor /v 
## What advantages does the “robocopy” command offer over the “xcopy” command, and why is it useful for file transfers in certain situations?
xcopy will copy multiple files or folders , robocopy is a more reliable copy application , and you can see the results, and how long it took
## Think about any real-life scenarios from your cultural context where the use of command line tools could be beneficial. Describe one such scenario and explain how a specific command line tool would help address the situation.
We would actually run group updates to all computers , I didnt know it was GP update, but we would constantly have to make sure all the computers were updated with certain secure files that would change from time to time





### Other Helpful Commands

Help- will tell you information about those commands
shutdown /s  /t nn(wait seconds then shutdown)-shutdown
shutdown /r  /t nn(wait seconds then shutdown)-shutdown and restart
shutdown /a                                   -abort
Deployment image servicing and management- dism 

chkdsk /f check disk only on file system 

chkdsk /r locates baad sectors and recovers readable information 

DiskPart - check disk partitions ( type diskpart,)If you need any more information type help in diskpart 

tasklist- check task currently running 

taskkill- terminate task  (taskkill /im notepad.exe  or taskkill /pid 1234 /t)

format: formats a disk for use with windows, - BE CAREFUL!!!! CAN DELETE DATA

copy( /v /y)- copy /v will verify that new files are written correctly, /y will suppresses prompting to confirm you want ot overwrite the dsestingation file .

