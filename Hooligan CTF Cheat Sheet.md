# Hooligan CTF Cheat Sheet

This is a list of all the commands you'll need to use throughout the Hooligan CTF.

## Useful directories and files

``/bin`` is where most commands live. if you do ``cd`` you're taking a shortcut to doing ``\bin\cd``

``/etc`` is where a lot of program files live, sometimes some useful stuff can be found here

``/tmp`` is a temporary directory. Everything here gets removed on startup

## ssh - Connect to a remote server

ssh is used to connect to a remote server

``ssh hooligan@hooligan.com -p 1234`` will connect to the server at hooligan.com with the user hooligan on port 1234

``ssh -i <key> hooligan@hooligan.com -p 1234`` will connect to a remote server using an ssh keypair called <key>

## cd - Change Directory

cd changes the directory

`` cd folder1`` will take you to folder 1

## ls - List directory

ls will list all of the directories and files in a directory.

### Arguments:

``-a`` will list all of the files, including hidden ones

``-l`` will list more information about the files, including size, owner, and permissions

## cat - Read a file

cat will read a speified file

``cat password.txt``

## grep - Find something in a file

Grep can be used to find something in a file. you have to pipe a source into grep to be able to use it.

Something like

``cat file.txt | grep "asdf"``

will return lines which contain ``asdf`` in the ``file.txt``

## wc - Count the words in a file

the first number is number of lines

the second number is number of words

the third number is number of characters

## find - Find a file

To use find you first give a directory to look at and then some options so

``find . -name text.txt`` will look for a file in the current directory called text.txt

``-user`` will show with a certain owner

``-size`` will show of a certain size. But there is a caveat here, it needs a suffix. if you did ``find -size 123M``, ``M`` is the suffix.

* ``b`` is for 512-byte blocks
* ``c`` is for bytes
* ``w`` is for 2-byte words
* ``k`` is for kilobytes
* ``M`` is for megabytes
* ``G`` is for gigabytes

## getent - read databases

this will read certain databases in a readble way

``getent [database]`` where database is the one you want to read

Some databases you might be intersted in:

* passwd: stores user information
* group: stores group information

## lscpu - show some info

this command will list information about the systems processor

## lspci - show even more info

this command will list information about the connected devices

## lsusb - show different info

this command will lsit information about the connected usb devices

## which - show where the command you're using is

giving it a command will show you where the command actually is on the system

``which cd`` will return where the ``cd``executable is on the system. 

## file - tells you what kind of file it is

in linux file extensions don't mean as much as they do in windows. ``file`` will tell you what kind of file a file is. 

## base32

decodes/encodes using base32

by default it will encode, give ``-d`` to decode. Base64 and 32 encoded files end with one or multiple ``=``

## base64

decodes/encodes using base64

by default it will encode, give ``-d`` to decode. Base64 and 32 encoded files end with one or multiple ``=``

## rot13

encodes/decodes using ROT13, a rotational cipher

## strings

will find whole words in a file

## ltrace

ltrace shows the system calls being made by a program. you have to execute the program in the argument for ltrace

to ltrace a exectuable called ``password`` you would do ``ltrace ./password``

Run the executable through once to see what's happneing before using ltrace. 

## vim - a handy editor

Vim is a file editor, however it can be a little difficult to use at first

There are a few different modes in vim, the two we really care about are ``insert`` and ``normal``

Insert mode allows you to edit the file you have open, normal mode allows you to pass commands to vim

Some handy vim commands

``:w`` write the file

``:u`` undos 

``:q`` quit

``:wq`` writes and quits

``q!`` quit discarding changes

## bzip2 - file compression

bzip is a file compression tool.

you can compress something with bzip2 by doing ``bzip2 <file>`` or decompress by doing ``bzip2 -d <file>``

## gzip - file compression

gzip is another file compress tool that will compress or decompress ``.gz`` file

you can compress something with gzip by doing ``gzip <file> `` and decompress with ``gzip -d <file>``

## xz - file compression

xz is _another_ file compression tool that will compress or decompress ``.xz`` files

you can compress something with xz by doing ``xz <file>`` and decompress by doing ``xz -d <file>``

