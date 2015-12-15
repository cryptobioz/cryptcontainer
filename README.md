Cryptcontainer
==============

What is it ?
------------

Cryptcontainer is a tool that was create to manage easily your encrypted containers. It work with **cryptsetup** and **LUKS**.

How it work ?
-------------

It very easy.

### Create a container #

To create a container named *MyFile* and with *1000* Mo (1 Go) of free space, run the command : `# cryptcontainer -c MyFile 1000`.

### Open a container #

To open a container named *MyFile*, run : `# cryptcontainer -o MyFile`.

### Close a container #

To close a container named *MyFile*, run : `# cryptcontainer -d MyFile`.

### List opened containers #

To list opened containers, run : `# cryptcontainer -l`


/!\ CAUTION /!\
---------------

**Do not use this program in production or to protect really important data. This script is still in developement, there are bugs !**
