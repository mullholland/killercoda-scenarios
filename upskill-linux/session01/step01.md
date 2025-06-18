### Where am i?

The first thing you see after login into a linux server with ssh is usually a blinking cursor.
The cursor is full of possibilities, some of which we are the discover here.

To better understand where we are, if we are visiting the server for the first time

### General Information

There are multiple ways to find out what linux distribution you are running

`cat /etc/os-release`{{exec}}

should always give you a first overview about the server and its os.

The Information there looks like this

```bash
NAME="Ubuntu"
VERSION="20.04.6 LTS (Focal Fossa)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 20.04.6 LTS"
VERSION_ID="20.04"
VERSION_CODENAME=focal
UBUNTU_CODENAME=focal
```

This describes the flavor of the Linux system (ID/Name) and the version (VERSION) in different ways.

we can also take a look at how the server calls himself with

`hostname`{{exec}}

this is the "shortname" of the server. The shortname on a server is only the irst part until the first dot "."
If the server has a longer name, like a domain ending, you can take a look at this with the command

`hostname -f`{{exec}}
or
`hostname --fqdn`

the "hostname" utility has some more options.

you can get a short overview over all the options with

`hostname --help`{{exec}}

### uname

To get some other basic information there is also the "uname" utility.
Take a look at the options the utility has and look at the different outputs.

`uname --help`{{exec}}

### Notes

Many of the tools we are using have a small help either with '-h' or '--help'. Sadly there is not standard for the help option and its mostly the other one ;)
