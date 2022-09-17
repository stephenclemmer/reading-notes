# Practice in the Terminal

### The Command Line - What is it, how does it work and how do I get to one.

The Command Line is another way to navigate one's computer. As opposed to a Graphical User Interface, the Command Line uses a text-based interface. Commands are entered in using text, and text is returned. As a MAc user, I use Terminal for my Command Line. My shell is ZSH. PROTIP: Use the arrow keys to navigate through previosly entered commands.

### Basic Navigation - An introduction to the Linux directory system and how to get around it.

#### Common commands to be used in the Command Line include

- **pwd** (print working directory): The “Where am i?” command
- **ls** (list): lists all of the items that are in the directory the user is currently in
- **cd** (change directory): ex: 'cd directoryname' The command cd may be run without a location as we saw in the shortcut above but usually will be run with a single command line argument which is the location we would like to change into. The location is specified as a path and as such may be specified as either an absolute or relative path and using any of the path building blocks. If a user ran 'cd' without also including an argument, then the user will always be taken back to the home directory.  
- **mkdir** (make directory)
- **cd..** (change directory and go back one): However many levels you want to go back, indicate one dot, and then add one.
- **touch** (make a file): ex '~ touch hiclass.md' would create a new markdown file called hiclass.
- **code .** (opens a new window with everything in the folder)
- **tree** (shows the tree of files. Similar to ls). It shows everything that is also inside of other directories.
- **-a** (i.e., 'tree -a'): If one were to hide files, adding this to the end of a command may reveal the hidden files.
- **-la** Similar to '-a', but it will display the results in list form, which is more digestable.

#### Types of Information entered and received from the Command Line

1. The first command line argument (i.e., '-l') is also referred to as an option. Options are typically used to modify the behaviour of the command. Options are usually listed before other arguments and typically start with a dash ( - ).
2. Most commands produce output and it will be listed straight under the issuing of the command. Other commands just perform their task and don't display any information unless there was an error.
3. After the command has run and the terminal is ready for you to enter another command the prompt will be displayed. If no prompt is displayed then the command may still be running

#### The Shell

The shell is part of the operating system that defines how the terminal will behave and how it will look after executing commands. BASH is a commonly used shell.

## PRO TIP 1

_Commands within the Terminal are stored in a history that can be accessed via the arrow keys. Rather than retyping familiar commands, simply scroll through the recently used commands to fly more easily through coding._

#### Paths: Absolute vs. Relative

Linux is a hierarchal structure. At the top is the **Root Directory**. The Root is denoted by a single slash ( / ). **Directories** and **Subdirectories** may be built off of the root, and files may be organized within them.

A path is a means to get to a particular file or directory on the system. There are 2 types of paths we can use, **absolute** and **relative**.

An **Absolute Path** specifies a location (file or directory) in relation to the root directory. You can identify Absolute Paths easily as they _always_ begin with a forward slash ( / ).

Relative paths specify a location (file or directory) in relation to where a user currently is in the system. Relative Paths _will not_ begin with a forward slash.

#### Common Building Blocks Used to Build Paths

~ (tilde): This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
. (dot): This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
.. (dotdot): This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory.

## PRO TIP 2

_When you start typing a path you may hit the Tab key on your keyboard at any time which will invoke an auto complete action. If nothing happens then that means there are several possibilities. If you hit Tab again it will show you those possibilities._



## More About Files - Find out some interesting characteristics of files and directories in a Linux environment.

### In Linux, Everything is a File

Unlike other systems, Linux does not use file extensions, i.e. .exe, .txt, .png, .jpg, .gif, etc. Instead, Linux looks inside the file to determine what it is. This is why on a mac, one can simply change a file extension to create a file with a different extension for use elsewhere, i.e., changing the extension of a picture from .jpg to .png. When no extension is present, the file type can be determined by using the command 'file', i.e. 'file [path]'.

### Linux is Case Sensitive

It is possible to have two files with the same name, but different choices of capitalization of the letters in the name. Similarly, 'ls' vs. 'lS' will render two different outputs because the commands are different.

### Spaces in Names

While spaces can be used within names, they will run the risk of being misunderstood as two distinct command line arguments. To ensure that naes containing words separated by spaces are understood as a single command line argument, use one of two conventions:

1. Use quotes around the entire item. i.e., cd 'Holiday Photos'
2. Use an escape character (\) before the space to nullify its meaning, i.e., cd Holiday\ Photos

## PRO TIP 3

Use Tab Completion to fill in the name and Linux will automatically escape any spaces for you.

### Hidden Files

Hidden files are created when a file or directory begins with a period (.) by adding '-a' to a command, hidden files may be revealed. i.e., 'ls -a'.

## Manual Pages - Learn how to make the most of the Linux commands you are learning.

The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept. You invoke the manual pages with the following command:

**man (command to look up)**

To exit the man pages press '**q**' for quit.

keyword search on the Manual pages:

**man -k** (search term)

## File Manipulation - How to make, remove, rename, copy and move files and directories.

**mkdir**: Makes a directory.

**rmdir**: Removes a directory.

**touch**: Creates a blank file.

**cp**: Copies a file or directory. This has many different options the syntax is:

**cp Options Source Destination**

**mv**: Moves a file or directory. mv can be used to rename a file or directory. This has many different options the syntax is:

**mv Options Source Destination**

**rm**: Removes a file or empty directory. The syntax is:

**rm Options File**

**rm -r**: To remove a directory and all files contained within.

## Cheat Sheet - A quick reference for the main points covered in this tutorial.

[CLI Cheatsheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)

This cheat sheet is intended to be a quick reminder for the main concepts involved in using the command line and assumes you already understand their usage
