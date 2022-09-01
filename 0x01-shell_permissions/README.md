## Project 0x01. Shell, Permissions

0-iam_betty : Switches current user to betty using *su betty *.
1-who_am_i : Shows effective username of the current user using *whoami* .
2-groups : Shows all the groups the current user is part of using *id -Gn* -Gn show all groups by name only
3-new_owner : Changes the owner of the file using *sudo chown"
4-empty : Creates empty file using *touch*
5-execute : adds execute (x) permission to owner of the file using * chmod u+x"
6-multiple_permissions : Adds execute permission to the owner and the group owner, and read permission to other users, using *chmod ug+x,o+r* 
7-everybody : Adds execute permission to all users using *chmod a+x* 
8-James_Bond :Sets the permission of a file with user and group no permission and other users with full permission using *chmod 007*
9-John_Doe : Sets mod of file to user=read,write,excute and group=read and excute only, other users=write and execute only using *chmod 753*  
10-mirror_permissions:  Sets the mode of the file same as another file's mode using * chmod --reference=sourceFile1 targetfile*
11-directories_permissions: Adds execute permission to all subdirectories of the current directory for all users, not affecting regular files. using *find ./ -type d -exec chmod ugo+x {} +*, this commind finds all directory in current directory *find ./ -type d * then the *-exec chmod ugo+x {}+* applies chmod command for every directory, the *{}+* runs the chmod commad on every directory by appending each selected directory name at the end, this will reduce number invocations of the command. 

12-directory_permissions :creates directory and sets permissions at the same time, using *mkdir -m*
13-change_group: changes group of a file using *chgrp* 
100-change_owner_and_group: changes owner and group of all the files and directories in the working directory using *sudo chown owner:group *
101-symbolic_link_permissions : changes owner and group of symbolic link directory using *sudo chown owner:group -h*
102-if_only :changes the owner of a file only if it is owned by specific user, using *sudo chown newOwner --from=oldOwner*
103-Star_Wars :plays the StarWars IV episode in the terminal. I was almost 😞  the task didn't provide much informatin, how to play, it a game or movies after sometime of googling, I found using *telnet" that you can watch StarWars on your terminal.

## What have I learned through these tasks

1. To be effective: since I was supposed to create around 17 files, add each one of #!/bin/bash ,change mod all of the files to u+x, add them to git and push: it was so much work, so I came with plan a. create,change mod and put #!/bin/bash files in batches. using 
I. touch file1 file2 file3....,
II. chmod u+x file1 file2 file3..,
II. echo \#\!/bin/bash | tee  file1 file2 file3..

2. It is very important to read man pages for the commands you are running if you are not sure about anything.
3. Why have I written all of this, just to reflect what I have done and gonethrough and it is a requirement in the project.





>Take Away: Always RFTM, and Read instructions carefully.



>ALWAYS DO THE HARD THINGS!






