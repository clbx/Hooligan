## Hooligan CTF

**Rules/Thing to know for Hooligan**

- You may not use google/stackoverflow/anything. Everything you need can either be found on this document, the cheatshee, or in a manpage. Plus you won't find the answers online. 
- you may not activley sabotage another players game. I've tried to make the game solid, but there will be things that I missed.
- Sharing passwords is strictly forbidden and will be punished by death (or disqualification) 

- Cheating (outside of the preceeding rules) is heavily encouraged. Please try and break the game (but preferably not the server it's on)
- You will want to keep a document with all the passwords you've found. It'll come in handy
- There is a logbook on every level. feel free to add your name or some trash talk, but please don't mess with it too much
- all passwords are human readable and are generally one word all lowercase and at least 5 characters long.
- you can create a folder in /tmp/ for temporary work, tmp is the only user modifiable directory, /tmp/ is not listable. 
- you can use ``su - <username>`` to switch users.

## hooligan0:

------

ssh into hooligan0 at the ip given during the CTF.

the password is hooligan

It should't be too hard to find the password for hooligan1

**Reccomended Commands**: cd, ls, cat

## hooligan1:

------

the password to hooligan2 is in a file thats 420 bytes in size

**Reccomended Commands**: cd, ls

## hooligan2:

------

the password for hooligan3, is in passwords.txt will the key being BxRufFCjEji9

if you manually look for it, you should drop out now

**Reccomended Commands**: grep

## hooligan3:

------

Inside of hooligan3 you will find the password.. somewhere.

the file is owned by "tropical" and the password is 7 bytes large.

**Reccomended Commands**: find (or grep if you're feeling dangerous) 

## hooligan4:

------

The password is in password.txt, but it looks a litle funky

**Reccomended Commands**: base32, base64

## hooligan5: 

------

The password to hooligan6 is the model name of the processor that the server is running on.

if the server was running on a "Dual-Core Intel Pentium Processor G2130" the password would be "Pentium"

## hooligan6: 

------

the password to hooligan 7, is conincidentally also the owner of hooligan7's full name. 

**Reccomended Commands**: getent, cat

## hooligan7:

------

the owner of hooligan7 made a program that spits out the password to hooligan8, though to get it you have to figure out the keyphrase for the program.

**Reccomended Commands**: ltrace

## hooligan8:

------

The password to hooligan 9 is stored in the file with the same number of bytes as there are lines in ``memior.txt``

## hooligan9:

------

There is no password for hooligan10. Instead, you must authenticate using an SSH keypair.

## hooligan10: 

------

The password to hooligan11 is in password.txt, but reading it might give you some difficulty

## hooligan11:

------

Exit vim

## hooligan12:

------

The password to hooligan13 is seems a bit _small_ don't you think?

**Reccomended Commands**: file, xz, bzip2, gz

## hooligan13:

------

The password to hooligan 14 is encrypted, figure it out. 

## hooligan14:

------

The password to hooligan15 is stuck somewhere in bliss.jpg. Go and find it!

## hooligan15:

------

Once you get unstuck you'll have to bruteforce your way to hooligan16









