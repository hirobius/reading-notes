# day_2

###### [day_1](day_1.md)
###### [day_2](day_2.md)
###### [day_3](day_3.md)
###### [day_4](day_4.md)
###### [day_5](day_5.md)
###### [day_6a](day_6a.md)
###### [day_6b](day_6b.md)
###### [day_7](day_7.md)
###### [day_8](day_8.md)

###### [MASTER_NOTES.md](MASTER_NOTES.md)


## VS seems legit. 

It's a full-on IDE. When selecting a Text Editor you need to weigh a couple factors that feel the best for the experiene you want when working in it while still remaining efficient for the job at hand.

One feature may be code completion, which is when your text editor will display possible suggestions based on what you have begun to type.
Emmet is a form of shorthand language that will speed up your code writing faster than you can imagine. You can have emmet built in or add it with an extension.

Syntax highlighting is another feature which provides individually different colors for attributes, elements and copy respectively so it's easier to parse the info you're reading.

The ability to add can provide you with dark backgrounds and brighter colored text, which can reduce eye strain. Or you can add other extensions to improve the functionality of your editor.
Brackets has “Live Preview” built in (which is a plus), but only supports HTML, CSS & JavaScript out of the box, meaning you will need an extension to write in further languages.


## The Command Line *(Also known as a Terminal)*

I think of the Command line as an extension of the Finder on my Mac. It is a text-based interface that you can navigate and interact with and add/subtract to and from. Apparently you can have multiple different command lines running different tasks at once while also jumping between the Finder or other GUI on your computer. 

You interact with the command line by entering certain commands which will return different outputs that cover the information you have requested or committed such as confirmations of changes you have made, your current position in a directory, warnings, current software versions or other relevant metadata 

Within a terminal is the shell which is a user interface that provides access to an operating system's services
A shell is a user interface for access to an operating system's services.


## More About Files
Linux is smart enough to look past the file extension and determine what the file actually is regardless.

Linux is also case sensitive, capitals and lowercase deliver different results.

You have to be strategic when working with spaces... you can use quotes to encapsulate the name of something to make it read as a single item. You can also use a "backslash" (\) to nullify the next character making it readable

ls -a will List the contents of a directory, including hidden files.


## Basic Navigation 
Beginning commands:

pwd — Print Working Directory

ls — This shows us what is in our current location

ls -a — This will List the contents of a directory, including hidden files. (there are multiple ways to run ls which I'm assuming I'll pick up later)

[] square brackets mean that an item is optional


## Paths
There are 2 types of paths we can use, absolute and relative.

The file system under Linux is a hierarchical structure. It begins with the ROOT and is denoted by a / followed by subdirectories then another / and more subdir and so on. There can be files in any of these directories.

You can either call on a directory relatively or using an absolute(exact) path... absolute pretty much means you will be "spelling it out" using a series of slashes and completely accurately spelled and case sensitive subdirectories down the line including their respective slashes from the root to the desired directory

There are also a few ways to bounce around paths: 


**cd** followed by the following will bring you up in the directory:

~ (tilde) — This is a reference to your home directory.

. (dot) — This is a reference to your current directory.

.. (dotdot)- This is a reference to the parent directory. 

***cd is the golden ticket to go places and actually navigate***


mkdir — make directory

rm -rf — big kid version of delete (be very careful)

rmdir — Remove directory

ls -a look for 


## Key takeaways to practice:

pwd — Print Working Directory - ie. Where are we currently.

ls — List the contents of a directory.

cd — Change Directories - ie. move to another directory.

ALWAYS MAKE A README for every repo you ever create. Best Practice.