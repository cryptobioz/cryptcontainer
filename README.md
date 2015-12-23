Cryptcontainer
==============

What is it ?
------------

Cryptcontainer is a tool created to manage easily your encrypted containers. It work with **cryptsetup** and **LUKS**.

How it work ?
-------------

It very easy.

### Create a container #

To create a container named *MyFile* and with *1000* Mo (1 Go) of free space, run the command : `# cryptcontainer -n MyFile 1000`.

### Open a container #

To open a container named *MyFile*, run : `# cryptcontainer -o MyFile`.

### Close a container #

To close a container with the ID *dKte5gsCaN*, run : `# cryptcontainer -d dKte5gsCaN`.

### List opened containers #

To list opened containers, run : `# cryptcontainer -l`

### Advanced features #

You can choose which cipher you want by using the argument **-c** : `# cryptcontainer -c twofish-cbc -n MyFile 1000`

*In this case, your container will be encrypted with the TwoFish algorithm and use the default hash size, 512.*

However, you can also choose the size of the hash by using the argument **-s** : `# cryptcontainer -s 256 -n MyFile 1000`

*In this case, your container will be encrypted with the default cipher, aes-xts-plain64, and use a hash size equal to 256 bits.*
