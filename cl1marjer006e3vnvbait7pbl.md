## Get started with Linux.

# What is Linux?

We get many different opinions from different developers around the world on what is [Linux](https://en.wikipedia.org/wiki/Linux), some say it is a [Kernel](https://en.wikipedia.org/wiki/Kernel_(operating_system) and some say it is [Operating System(OS)](https://en.wikipedia.org/wiki/Operating_system). Linux is both a Kernel and an Operating System that directly manages a system’s hardware and resources, like CPU, memory, and storage i.e. **Linux is an operating system’s kernel**.

This amazing video by Gary Explains can easily solve the doubt of whether Linux is a Kernel or a Operating System :
<iframe width="560" height="315" src="https://www.youtube.com/embed/RNeKYjWx-s4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Linux is a free and the biggest open sources software project in the world. The most amazing fact about Linux is that anyone can run, learn, modify Linux according to your choice and even sell your version only when all the changes done are under [GNU General Public License (GPL)](https://en.wikipedia.org/wiki/GNU_General_Public_License). 

[There are several Linux Distributions](https://linuxhint.com/best-linux-distros-2022/): 

1.  **Ubuntu Linux**
2. **Zorin OS**
3. **Raspberry Pi OS**
4. **Red Hat Enterprise Linux**
5. **Fedora**

# What is a Command Line Interface(CLI)?
A [command-line interface (CLI)](https://en.wikipedia.org/wiki/Command-line_interface) is an operating system shell that uses alphanumeric characters typed on a keyboard to provide instructions and data to the operating system, interactively. 

When we talk about Command Line what we actually mean is ["Shell"](https://en.wikipedia.org/wiki/Unix_shell). It follows give and take system i.e. it takes input in the form of commands from the keyboard gives it to the operating system to process it and gives output. [Bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell) is a very famous shell program from GNU Project.

The popular shells used in Linux are:

- C Shell (csh)
- Kron Shell (ksh)
- Z Shell(zsh)

This is how a Command-Line looks:


![Screenshot 2022-04-03 at 7.17.15 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648993675577/O1Zpr0rjl.png)

# Basic Linux Commands 
As mentioned above Shell is used to communicate with the operating system and that is done through commands(reserved keywords performing a specific function). In this post, I have divided the commands on the basis of beginner and intermediate level. 

General syntax of writing a Linux Command: 

**command -(options) argument1 argument2 ...**


**🚨 Terminal is a case-sensitive platform so be careful while typing commands on command line.**


## Beginner Level Linux Commands 

**1. pwd:**

When you will open your terminal you will be in your home [directory](https://www.computerhope.com/jargon/d/director.htm) of the computer system. It is comparatively hard in Command-Line to know in which directory you are then the [Graphical User Interface(GUI)](https://en.wikipedia.org/wiki/Graphical_user_interface).
How to know when you are in which directory?  
The answer is "pwd" command which on running on the Command-Line gives you the exact location you are in with a complete path from the root directory.

```
pwd
``` 
On typing this command and pressing enter you will get an output on the console containing the result in which directory you are now, below is the example of "pwd" command :


![Screenshot 2022-04-03 at 7.18.11 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648993717709/bCmn521-X.png)
 
**2. mkdir and rmdir:**

The "mkdir" command is one of the most used command which is used to create a new directory.

```
mkdir (directory name)
``` 

![Screenshot 2022-04-04 at 3.53.01 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649067812716/vVm6czi56.png)


The "rmdir" does the opposite of "mkdir" i.e. it deletes any directory of your choice.

```
rmdir (directory name)
``` 


![Screenshot 2022-04-04 at 3.56.36 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649068022201/h9bJ5Ug7C.png)

There is more you can do with a command by using [Flags(or Options)](https://www.ibm.com/docs/en/aix/7.2?topic=names-command-flags) with the commands to get more filtered information.

**Flags(or Options):**

**· mkdir -v and rmdir -v:**


The "mkdir -v" command is used to create more than one directory in a single command.
```
mkdir -v (directory names)
``` 

![Screenshot 2022-04-05 at 3.11.44 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649108532064/18k6ozgBc.png)

The "rmdir -v" does the opposite of "mkdir -v" i.e. it deletes multiple directories in single line.

```
rmdir -v (directory names)
``` 

![Screenshot 2022-04-05 at 3.13.56 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649108685606/QMu9yq6ea.png)

**· mkdir -m:**
The "mkdir -m" command is used to set permissions on directory created.

```
mkdir -m (directory name)
``` 

![Screenshot 2022-04-05 at 3.16.55 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649109065652/KwANWohTv.png)


**3. touch:**

The "touch" command is also similar to "mkdir" command the only difference is that this command is used to create new files instead of a directory.

```
touch (file name)
``` 

![Screenshot 2022-04-04 at 4.19.00 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649069369680/elhrUKLzN.png)

**4. rm:**

The "rm" command works opposite to that of "touch" command i.e. it is used to delete the file.

```
rm (file name)
``` 

![Screenshot 2022-04-04 at 4.34.05 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649070331193/htZX8M7dt.png)
 

**Flags(or Options):**

**· rm -i:**

The "-i" here stands for interactive mode i.e. it asks the user for confirmation before removing the
file, you have to press y for confirming the deletion, and any other key leaves the file un-deleted.

```
rm -i (file name)
``` 

![Screenshot 2022-04-05 at 12.03.12 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649140415782/_J5f-8V60.png)

**· rm -f:**
The "-f" stands for force removal i.e. it forcefully removes the file is it used for even though it has some permissions or protection.


```
rm -f (file name)
``` 

![Screenshot 2022-04-05 at 12.07.32 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649140687715/QAvQaPtrt.png)
    
**5. ls:**

The "ls" command is used to list all the directories(folders) and files present in your current directory(the directory you are in)

```
ls
``` 
Below is the example of the result obtained on the console after entering "ls" command :

![Screenshot 2022-04-03 at 7.25.35 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648994169951/aVXvEhX8h.png)

**Flags(or Options):**

**· ls -a:**

The "ls -a" command will list all the files and directories of the current working directory along with the hidden files. 

```
ls -a
``` 

![Screenshot 2022-04-03 at 8.59.04 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648999772245/-cXuZThSy.png)

All the files starting with "." are hidden files.

**· ls -l:**
The "-l" flag is used to display more important information about the file in a long list format. Information such as file size, owner name, permissions, etc is displayed.

```
ls -l
``` 

![Screenshot 2022-04-05 at 12.15.29 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649141316833/yyu1bkDJ_.png)

**6. cd:**

The cd (“change directory”) command is used to change the current working directory in Linux and other Unix-like operating systems. “cd” expects the directory name or path of the new directory as input.


![Screenshot 2022-04-04 at 3.26.05 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649023018993/6K4Om-MGe.png)
       

```
cd (directory name)
``` 

There is a rule which is followed by "cd" command that is the directory you want to move in should be present in your current directory or it will throw an error. In order to move from one directory to other directories you should go to the parent directory of the directory. 

Various ways of using "cd" commands are :

![Screenshot 2022-04-04 at 3.35.24 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649023627929/lW_j8PLbD.png)

**7. clear:**

The "clear" is a very basic Linux command used to clear the command line by shifting all the current console input and output upwards and presenting an empty command line on the screen.

Before running "clear" command :

![Screenshot 2022-04-04 at 3.41.25 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649023896684/qUgpxhGdJ.png)

After running "clear" command :

![Screenshot 2022-04-04 at 3.42.53 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649023983088/4jbdTrOr9.png)

**8. man:**

The "man" command is a very useful command as it is used to get complete information of other commands and use the information to carry out your task. It shows the [manual pages](https://www.javatpoint.com/linux-man) of the commands.

```
man (command)
``` 

![Screenshot 2022-04-04 at 7.16.23 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649080012504/66MthxgZa.png)

Press "q" key to exit the information mode.

**Flags(or Options):**

**· man -a:**

The "-a" flag is used to display all the available introduction manual pages.

```
man -a (command)
``` 

![Screenshot 2022-04-05 at 12.33.52 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649142258122/Bhmw8cRPr.png)

**· man -w:**

The "-w" flag displays the location of the manual page of the entered command.


```
man -w (command)
``` 

![Screenshot 2022-04-05 at 12.38.23 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649142527534/leEyn8K4S.png)

**9. cp and mv:**

The "cp" command is used to copy files from one directory to other directories.

```
cp (file name) (destination directory)
``` 

![Screenshot 2022-04-04 at 7.28.51 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649080773466/CsjzShuCJ.png)

The "mv" command is used to move files from one directory to another directory (cut and paste).


```
mv (file name) (destination directory)
``` 

![Screenshot 2022-04-04 at 7.33.30 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649081061663/Sd_ow-6mK.png)

**Flags(or Options):**

**· cp -i and mv -i:**

The "-i" stands for interactive copying of files. It is the same as the "rm -i" which asks the user for confirmation before overwriting the file, you have to press y to confirm, and any other key leaves the file un-copied. 
 

```
cp -i (file name) (file name)
``` 


![Screenshot 2022-04-05 at 1.18.27 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649144983457/XCkJJlncK.png)

The "mv -i" is the same as that of the "cp -i" command the only difference is that it does not work if files do not exist,  it simply renames it or moves it to a new location.  

**· cp -f and mv -f:**

The "-f" stands for force, if in any case user is not able to overwrite the file, the user can use this flag along with the "cp" command in order to overwrite the file forcefully. This comes in handy when user does not have the write permission to a file.

```
cp -f (file name) (file name)
``` 

![Screenshot 2022-04-05 at 3.10.46 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649151680688/QwALLFlVG.png)

The "mv -f" command is also the same as the "cp -f" command the only difference is it overrides the minor protection and overwrites the destination file forcefully and deletes the source file. 

**10. locate:**

The "locate" command as the name suggests is used to locate a file in your local system.

```
locate (file name)
``` 

![Screenshot 2022-04-05 at 12.16.38 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649098022107/VJnLy5Tsv.png)

**Flags(or Options):**

**· locate -c:**

The "-c" flag stands for the number of counts the file with the filename has occurred.

```
locate -c (file name)
``` 

![Screenshot 2022-04-05 at 3.35.07 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649153133555/uGAq1g_u8.png)

**· locate -i:**

The "-i" command here stands for Ignore Case Sensitiveness, it is used to differentiate case sensitive locate outputs.

```
locate -i (file name)
``` 

![Screenshot 2022-04-05 at 3.39.21 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649153389962/T3iSsn1Kc.png)

## Intermediate Level Linux Commands 

**1. vim:**

The "vim" command is used to write content in the file. After typing the "vim" command followed by the file name a different window of the text editor will open. Press "i" to enter insert mode in the text editor, type the content you want to add or edit and press "esc" key to exit insert mode. The process is not yet completed you still need to save what you have changed in the file to do so you have to ":wq" to save and exit the text editor.

```
vim (file name)
``` 
After entering the command followed by the file name window like this will appear : 

![Screenshot 2022-04-05 at 12.37.56 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649099404191/29x6mQxUb.png)
Press the "i" key and you will see "INSERT" written on the bottom left of your screen :


![Screenshot 2022-04-05 at 12.53.34 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649100257162/ARnLsITO-.png)

Start writing your content press the "esc" key and you will see "INSERT" will disappear then save and exit by hitting ":wq".

![Screenshot 2022-04-05 at 12.47.21 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649099916545/MGX6zLatN.png)

There are 59 flags use can use with the "vim" command. To explore all of them you can visit [computerhope.com](https://www.computerhope.com/unix/vim.htm).

**2. cat:**

How do we know if the file we edited above has been successfully updated? The answer is "cat" command which is used to display the content of a file on the console.

```
cat (file name)
``` 

![Screenshot 2022-04-05 at 12.52.27 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649100177008/rSX6mM3Yd.png)

**3. sudo:**

The "sudo" command stands for “SuperUser Do”. If you want any command to be done with administrative or root privileges, you can use the sudo command.
Only those users can run "sudo" command who has an entry in /etc/sudoers file. A common misconception about "sudo" command is that it is used solely to provide root permissions to an ordinary user.
The "sudo" command always asks you to enter your system password to proceed because it is a very sensitive command.

```
sudo (command)
``` 


![Screenshot 2022-04-05 at 1.20.15 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649101921502/JAv6msqI-.png)

**Flags(or Options):**

**· sudo -l:**

The "-l" flag stands for list, it is used to list the user’s privileges or check a specific command.


```
sudo -l
``` 

![Screenshot 2022-04-05 at 3.51.48 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649154148881/OwNY2Aqmf.png)

**4. chmod:**

The "chmod" command is used to make a file executable and to change the permissions granted to it in Linux.

```
chmod (options) (permissions) (file name)
``` 


![Screenshot 2022-04-05 at 1.33.04 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649102612326/zQb7-oWXJ.png)

**5. df:**

The "df" command displays the size, used space, and available space on the mounted filesystems of your local system.

```
df (flag)
``` 

![Screenshot 2022-04-05 at 1.45.47 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649103389347/Dnrb3CGNc.png)

**Flags(or Options):**

**· df -a:**

The "df -a" command is used to display all file system including the files that have zero disk storage.

```
df -a
``` 

![Screenshot 2022-04-05 at 4.06.55 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649155045228/hlD3BrYkC.png)

**· df -h:**

The "-h" stands for human-readable, it is the most useful flag as it displays the sizes in Mb or Gb instead of in bytes.


```
df -h
``` 

![Screenshot 2022-04-05 at 4.08.03 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649155111883/ktAtsFc5L.png)

**6. hostname:**

The "hostname" command displays your hostname and IP address. The “hostname” command gives the output. 

```
hostname (flag)
``` 

![Screenshot 2022-04-05 at 1.49.40 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649103614427/85VwWOpvY.png)

**7. du:**

The "du" command is used to know the disk usage of a file in your local system. If you want to know the disk usage for a particular folder or file in Linux, you can type in the "df" command and the name of the folder or file.

```
du (file name)
``` 

![Screenshot 2022-04-05 at 1.55.46 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649103966826/6b8zE1Mfe.png)

**Flags(or Options):**

**· du -a:**

The "df -a" command is used to display all files along with directories.
```
du -a
``` 


![Screenshot 2022-04-05 at 4.13.50 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649155460392/N6xQALmLy.png)

**· du -h:**

The "-h" stands for human-readable, it is used to display sizes in human-readable form on console.


```
du -h
``` 

![Screenshot 2022-04-05 at 4.14.38 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649155505966/QGfVVQxjj.png)

**8. finger:**

The "finger" command gives you a short dump of information about a user, including the time of the user’s last login, the user’s home directory, and the user account’s full name.

```
finger (username)
``` 

![Screenshot 2022-04-05 at 1.58.15 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649104119508/jtMb7CRoz.png)

**9. ping:**

The "ping" command is used to check your connection to a server.

```
ping (website URL)
``` 

![Screenshot 2022-04-05 at 2.04.06 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649104470222/w4JVob97W.png)
Press "control + C" to exit from the loop.

There are various flags you can use and experiment with the ping command, visit [geeksforgeeks.com](https://www.geeksforgeeks.org/ping-command-in-linux-with-examples/) to learn more.

**10. uname:**

The "uname" command is used to display the information about your local system.

```
uname (flag)
``` 

**Flags(or Options):**

**· uname -a:**

The “uname -a” command prints most of the information about the system.


```
uname -a
``` 
![Screenshot 2022-04-05 at 2.01.46 AM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649104336233/w8Xns_guA.png)  

**· uname -r:**

The "uname -r" is used to display the kernel release date.


![Screenshot 2022-04-05 at 4.23.17 PM.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649156042043/p8ZNQ86hp.png)


# Resources 

- [What is Linux by RedHat.](https://www.redhat.com/en/topics/linux/what-is-linux#how-does-linux-work) 

- [The 50 Most Popular Linux & Terminal Commands.](https://www.youtube.com/watch?v=ZtqBQ68cfJc)

- [Introduction to Linux.](https://learning.edx.org/course/course-v1:LinuxFoundationX+LFS101x+2T2021/home)

**Watch the complete blog in the form of video:**

<iframe width="560" height="315" src="https://www.youtube.com/embed/NRzojAzA9Rg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 



# Conclusion 
In this article, we learned about Linux and various useful terminal commands. There you are at the end of this blog post, I hope this blog will help you all in understanding Linux, and Yipee!!🥳 you just started with Linux and are among 54% of developers to use Linux. I would like to thank @[Saiyam Pathak](@Saiyampathak) and @[Kunal Kushwaha](@kunalk) who encouraged me to start my technical writing journey. 

Special thanks to @[Pavan Gudiwada](@pavangudiwada) for helping me out in maintaining the proper structuring of this blog.

Don't forget to like and share this post if you liked this blog. Connect with me on [Twitter](https://twitter.com/SuperAayush14). Follow me for more such blogs.
 
**THANKS FOR READING 😄📖!!**

**#LEARNINPUBLIC**

**[Aayush Sharma 👨🏻‍💻](https://superaayush.github.io/Portfolio/)**