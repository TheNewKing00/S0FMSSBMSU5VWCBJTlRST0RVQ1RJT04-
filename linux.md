# Kali Linux Introduction

### First Things First!

What we’re about to learn holds a greater responsibility, so please do not abuse them unless given a consent. And remember to have fun. We are about to poses real life powers, so use them wisely. -JOHN

### What is Kali Linux?

Kali Linux (formerly known as BackTrack Linux) is an open-source, Debian-based Linux distribution aimed at advanced Penetration Testing and Security Auditing. It does this by providing common tools, configurations, and automations which allows the user to focus on the task that needs to be completed, not the surrounding activity.

Kali Linux contains industry specific modifications as well as several hundred tools targeted towards various Information Security tasks, such as Penetration Testing, Security Research, Computer Forensics, Reverse Engineering, Vulnerability Management and Red Team Testing.

Kali Linux is a multi-platform solution, accessible and freely available to information security professionals and hobbyists.
Source: [https://www.kali.org/docs/introduction/what-is-kali-linux/](https://www.kali.org/docs/introduction/what-is-kali-linux/)

### What is for?

To provide educational tools and exercise knowledge with the importance of privacy and cybersecurity.

### Why?

To be cool and awesome, badass, and excerpt dominance to others? <span class="colour" style="color:rgb(238, 85, 85)">**Error Encountered a representation error. Thread: Misuse of tool and should not be permitted.**</span>
To protect others who does not know they are vulnerable to such attacks. <span class="colour" style="color:rgb(238, 238, 16)">**Runtime completed with at most RESPECT.**</span>

### How?

This is where the real fun begins.
Basic Commands for navigation.
upon login in for the first time you will be greeted with the desktop of Kali-Linux.
Open the terminal by pressing `Crtl`+`Alt`+`T` this terminal will be your new best friend. You’ll sleep, eat and beat each other for the next sessions.

**OBJECTIVES**

* Folder Navigation
* Folder Creation
* Accessing Files
* Creating Files
* Modifying Files

##### Folder Navigation

Navigating the folder is easy. The command used for that is `cd` or *change-directory*. In order to know what directory, you are currently in, type `pwd` on the terminal, or *print-working-directory*. to list items on the current directory type `ls` or *list*.

* `pwd` – its like asking the terminal what folder am I at?
* `ls` – or list, simple.
* `cd` – change directory. Followed by the folder name, in order to go to that folder.

<br>
**All good? Great! Next is...**

##### **Folder Creation**

`mkdir` or make-directory is the command you can enter to the terminal followed by the folder name, In order to create a folder, Example.

```
mkdir “my personal folder”
```

A folder will be created in the current directory.
Alternatively you can delete the folder by entering `rmdir` or Remove-Directory. Example

```
rmdir "my personal folder"
```

to remove the folder you just created.
**Note that if you wish to create folder with white spaces such as a space bar or folder names that contain more than one word, should be enclosed with a quotation marks.**

* `mkdir` – used to create a folder
* `rmdir` – used to delete a folder

##### **Accessing Files**

In accessing files in Linux there are several approaches. But mainly you will be opening text files or execute some application. in this case we will focus on the text files.
For opening text files can be done using the command `cat`For Example:

```
cat "my file.txt"
```

this allows the terminal to display everything that is displayed in the given text file.
**Note that this is useful in opening notes you have created or files you dumped. more on that later**
now you know how to access files.  lets talk about...

##### Creating Files, or more particularly, text files.

There are 2 main ways you can do this.
one is using the command `touch`and second is the command `echo`more on this later.
`touch`is faily simple. for example:

```
touch "file name.txt"
```

This allows you to create text files that you can write on.
To write on those files I recommend using `vim` for that but that will have its own tutorial.

Another way creating text files is by using the `echo` command. `echo`lets you to store the result from what command you have entered. this way you will let you to write or append directly without going through `vim`.

```
echo "my text inside the text file" >> myTextfile.txt
```

##### **Modifying file permissions**

this might come in handy in some cases
`chmod`command allows you to change permissions on certain files. with the following options `r`,`w`,`x`or read, write, execute permissions. you can attach operators to this such as `+`or `-`meaning you can add or remove permissions on the file. example.

```
chmod +rw myTextfiles.txt
```

this command just allowed you to add read and write permission to the file or subsequently you can remove them just like

```
chmod -rw myTextfiles.txt
```

more about this in...
source [https://www.geeksforgeeks.org/permissions-in-linux/](https://www.geeksforgeeks.org/permissions-in-linux/)

##### Other Commands

other quality of life commands

* `whoami`\- allows you to display the current user of the terminal\.
* `hostname` \- allows you to see you current network hostname\. this only pertains to your own IP address like 127\.0\.0\.1 or 0\.0\.0\.0 or localhost\.

**you can also compound commands together to execute them in one line.**
To do that you can use the following operators.

* `;`operator allows you to put one command on one side and another on the other side that executes in linear order frome left to right. if the first command throws an error the next one will be executed nonetheless.
* `||`OR operator will check whether the left or right command execute. if both returns an error both will not execute.
* `&&`AND operator requires both left and right command should return something. otherwise if one gets an error it will return nothing.

Examples

```
whoami ; hostname
```

in this example `whoami` will give a return followed by the `hostname`

```
whomi || whoami
```

in this case the first command obviously returns an error so the second one will execute. if the first command in the left will return as true the second command will not execute even if its correct.

```
whomi && whoami
```

this will stop at the first command due to it having an error. if both are correctly typed both commands will execute.
**These commands are very helpful for executing one-liners to deliver single stage payloads. leaving less dection time.**
More can be found here: [https://www.makeuseof.com/how-to-run-multiple-linux-commands-at-once/](https://www.makeuseof.com/how-to-run-multiple-linux-commands-at-once/)
**you can also find more info about the commands you're using by typing `man`infront of the command you want to learn more about.**
`man` stands for Manual.

### NEXT UP WILL HAVE GREP+REGEX, BASE64+CRYPTOGRAPHY AND VIM.