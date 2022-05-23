# Shell Permissions

### [What is the Shell?](http://www.linuxcommand.org/lc3_lts0010.php)

Shell is an environment in which we can run our commands, programs, and shell scripts.

### [Shell permissions](https://www.guru99.com/file-permissions.html#linux_file_permissions)

***Every file and directory in your UNIX/Linux system has following 3 permissions defined for all the 3 owners discussed above.***

- **Read:** This permission give you the authority to open and read a file. Read permission on a directory gives you the ability to lists its content.

- **Write:** The write permission gives you the authority to modify the contents of a file. The write permission on a directory gives you the authority to add, remove and rename files stored in the directory. Consider a scenario where you have to write permission on file but do not have write permission on the directory where the file is stored. You will be able to modify the file contents. But you will not be able to rename, move or remove the file from the directory.

- **Execute:** In Windows, an executable program usually has an extension “.exe” and which you can easily run. In Unix/Linux, you cannot run a program unless the execute permission is set. If the execute permission is not set, you might still be able to see/modify the program code(provided read & write permissions are set), but not run it.

#### File permission commands:

##### 1.	[chmod](https://www.pluralsight.com/blog/it-ops/linux-file-permissions) 
##### 2.	[su](https://phoenixnap.com/kb/su-command-linux-examples)

##### 3.	[sudo](https://kb.iu.edu/d/amyi#:~:text=The%20sudo%20command%20allows%20you,which%20the%20system%20administrator%20configures.)
##### 4.	[chown](https://linuxize.com/post/linux-chown-command/)
##### 5.	[chgrp](https://www.geeksforgeeks.org/chgrp-command-in-linux-with-examples/)


