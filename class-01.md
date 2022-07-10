# Read 1 Introductory HTML and JavaScript

## Things I Want to Know More About

1. Practical uses for the Bang Operator (!)

## How the Web Works

## How the Web Works

1. **Compose a short poem describing how HTTP sends data between computers.**

***The client requests service. The server responds with service.***
**The client asks for a menu. The server responds with a menu.**
*The client orders a meal. The server puts in the order.*
The kitchen makes the order. The client picks up the meal.

2. **Describe how HTML, CSS, and JS files are “parsed” in the browser.**
The browser parses the HTML file first, and that leads to the browser recognizing any \<link>-element references to external CSS stylesheets and any \<script>-element references to scripts.
As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from \<link> elements, and any JavaScript files it has found from \<script> elements, and from those, then parses the CSS and JavaScript.
The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.
As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.


3. **How can you find images to add to a Website?**
4. **How do you create a String vs a Number in JavaScript?**
5. **What is a Variable and why are they important in JavaScript?**

## Ryan's Linux Tutorial

### Important Concepts

- Everything is a file under Linux, even directories.
- Linux is an extensionless system. Files can have any extension they like or none at all.
- Linux is case sensitive. Beware of silly typos.
- No undo. The Linux command line does not have an undo feature. Perform destructive actions carefully.
- Command line options: Most commands have many useful command line options. Make sure you skim the man page for new commands so you are familiar with what they can do and what is available.

### The Command Line

ex: 

Prompt: Command: Command-line arguments

- There must be a space between the command and the first command line argument
- The first command line argument is also referred to as an option. Options are typically used to modify the behaviour of the command. Options are usually listed before other arguments and typically start with a dash ( - ).

***Shortcut***: Use the up and down arrow keys to scroll through previously entered commands
***Shortcut***: Run cd by otself to be taken back to the home directory
***Shortcut***: **Tab Completion**: Hit the Tab key on your keyboard at any time which will invoke an auto complete action. If nothing happens then that means there are several possibilities. If you hit Tab again it will show you those possibilities. You may then continue typing and hit Tab again and it will again try to auto complete for you.
***Shortcut***: ~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /Users/Stephen then you could refer to the directory Documents with the path /Users/Stephen/Documents or ~/Documents

### Commands

**pwd**: (print working directory) Tells you what your current or present working directory is.
**ls**: (list) Lists the contents of the current directory. i.e., ls [options][location]
-- **-l**: (long listing, i.e., ls -l)
-- **/etc***: (i.e., ls /etc) Tells ls not to list our current directory but instead to list that directory's contents.
**ls -a**: will list all files, including those that are hidden.
**cd**: (change directory ex, cd [location]) Change Directories - ie. move to another directory.
**/etc**: - Stores config files for the system.
**/var/log**: - Stores log files for various system programs. 
**/bin**: - The location of several commonly used programs.
**/usr/bin**: - Another location for programs on the system.
**file [path]**: To obtain information about what type of file a file or directory is.
**man <command to look up>**: Accesses the manual for a particular command.

### Paths

Whenever we refer to either a file or directory on the command line, we are in fact referring to a path. ie. A path is a means to get to a particular file or directory on the system.

**Absolute Paths**: Absolute paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )

**Relative Paths**: Relative paths specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.

#### Path Navigation

~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /Users/Stephen then you could refer to the directory Documents with the path /Users/Stephen/Documents or ~/Documents
. (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
.. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /Users/Stephen you could run the command ls ../../ and this would do a listing of the root directory.

#### Spaces in Names

- Use quotes or an escape character before spaces ( \ ) to denote that a file name with spaces in the title is a single command line argument.
- Use Tab Completion to automatically escape spaces in a title.

#### Hidden Files

- Use a period ( . ) at the beginning of a file name to make it hidden.
- ls -a will list all files, including those that are hidden.

### Manual Pages

The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept. You invoke the manual pages with the following command:

**man [command to look up]**

To exit the manual pages, pres 'q' for quit.

Keyword search on Manual pages:

**man -k [search term]**

If you want to search within a manual page while you are in the particular manual page,  search press forward slash '/' followed by the term you would like to search for and hit 'enter' If the term appears multiple times you may cycle through them by pressing the 'n' button for next.

### File Manipulation

**mkdir**: command used to make a new directory. i.e., mkdir \[options]\<Directory>
**mk dir -p**: Tells mkdir to make parent directories as needed, i.e., mkdir -p directory/subdirectory1/subdirectory2
**mk dir -v**: The v stands for verbose. The terminal will display in detail what was done.
**rmdir**: Removes a directory. i.e., rmdir \[options]\<Directory>. Technically a directory needs to be empty before it can be removed, however there is a way around this that I will learn later. -p and -v are both available on rmdir.

#### Creating a Blank File

**touch**: Creates a blank file i.e., touch \[options]\<filename>
What is being taken advantage of is that if we touch a file and it does not exist, the command will do us a favor and automatically creating it for us. Touch is actually a command one may use to modify the access and modification times on a file (normally not needed but sometimes when you're testing a system that relies on file access or modification times it can be useful).

#### Copying a File or Directory

**cp**: Copies a file or directory, i.e., cp \[options]\<source>\<destination>

#### Moving a File or Directory

**mv**: Moves a file or directory, i.e., mv \[options]\<source>\<destination>

#### Renaming Files and Directories

Renaming can be done using mv. Were one to specify the *destination* to be the *same directory as the source, but with a different name*, then one may effectively use mv to rename a file or directory.

#### Removing a File (and Non-Empty Directories)

**rm**: Removes a file, i.e., rm \[options]\<file>
**rm -r**: Removes directories and all files contained within them.
*A good option to use in combination with r is i which stands for interactive. This option will prompt you before removing each file and directory and give you the option to cancel the command.*

