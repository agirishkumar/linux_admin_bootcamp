A *Command Line* is a text based interface which can be used to input instruction to computer system. 
The Linux Command Line is provided by a program called *Shell*.*Bourne Again Shell (bash)* is the default shell program of RHEL/Centos.
When a shell is used interactively,it displays a string when its waiting for a command from the user.This is called *Shell prompt*.
It looks like this:
```
[user@host ~]$
```
if the user is root '$' is replaced by '#'
```
[root@host ~]#
```

Commands entered in shell prompt have three basic parts:

* Command, to run
* Options, to adjust the behaviour of the command
* Argumnets, which are targets of the Command

## Logging in over the network
```
[user@host ~]$ ssh remoteruser@remotehost
remoteruser@remotehost's password: password
[remoteruser@remotehost ~]$
```
The **SSH** Command encrypts the connection to secure the connection to remote host
For tighter security authentication to remote machine is done through **public key authentication** without entering the password

With this Public Key Authentication method , users have special identity file containing **Private key** which is equivalent to password and this
is kept secret.
