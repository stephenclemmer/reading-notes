# Read 2: The Coder's Computer

## Text Editor vs. Code Editor vs. IDE

A **text editor** is a tool that allows one to organize and format text. Eamples include MS Word and Google Docs. These examples are "What you see is what you get" (WYSIWYG) because the final product will look identical to the text that has been inputted/formatted.

A **code editor** is a type of text editor that helps is designed to help coders write code. Unlike WYSIWYG applications, the inputted code's format will not resemble the text that is output. Unlike word processing text editors, code editors contain additional features that assist in formatting, editing, and proofing code such as syntax highlighting. Features of text editors may include:

- **Code Completion**: Suggests possible code to increase efficiency and reduce typos
- **Syntax Highlighting**: Colorizes text to make it more readable, and easier to discern between the different parts of code, i.e., elements and attributes.
- **Themes**: A variety of formats to choose from that make code easier to read and reduce eye strain
- **Extensions**: Plug-ins that increase the utility of the application

An **Integrated Development Environment, (IDE)** combines many tools all in one place such as a text editor, a code editor, termnal, and database. This allows a coder to stay within the same platform when writing, rather than needed to more between applications.

Whichever of these a person chooses depends on their own preferences, needs, and workflow. This can be subjective  Ultimately, whichever tools gets the job done best for a prticular person or team is the best one to use.  In the same way that a hammer, sledgehammer, and ball peen hammer all serve specific purposes, **it is important that developers understand the needs of their projects, teams, and organizaitions so they can choose the right tool for the coding task that helps them code efficiently and effectively.**

### Best Practices to Bear in Mind When Coding with Text Editors

- Make sure to code in plain text
- Create folders and subfolders to store files in an organized fashion
- Make sure that files contain the appropriate extension, i.e.:
  - style._**css**_
  - index._**html**_

### The Command Line

Most computer users interact with their machines by using a **Graphical User Interface (GUI)**, where they can command their machines to run applications and store files by interacting with icons and other visual elements. A **Command Line**, (i.e. Terminal), is a text-based interface that can provide additional functionality for computer users. Commands are entered as text, and feedback is delivered back to the user in text.

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

### The Shell

The shell is part of the operating system that defines how the terminal will behave and how it will look after executing commands. BASH is a commonly used shell.

## PRO TIP 1

_Commands within the Terminal are stored in a history that can be accessed via the arrow keys. Rather than retyping familiar commands, simply scroll through the recently used commands to fly more easily through coding._

### Paths: Absolute vs. Relative

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
