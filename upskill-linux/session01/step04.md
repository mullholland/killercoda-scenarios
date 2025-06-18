### simpler times

These are some pretty detailed informations. Many times a little bit less is enough. So lets take a look the mos common basics. CPU, RAM and Discs.

#### Discs

to get an overview over your discusage there a multiple ways, the first is usually

`df -h`{{exec}}

Here you can see that the usual help parameter '-h' is used differntly. Here it means 'human readable', which translates the bytes to kilo,mega and the other bytes. so to get all the options use the '--help' parameter.

This show the filesystem this server has, how much space there is and where they are mounted.
Dont worry about the Mounted part at the moment, we will later explore what this means, concentrate on the parts Size, Uses, Avail and Use%

```bash
Filesystem  Size  Used Avail Use% Mounted on
/dev/vda1    98G   69G   25G  74% /
```

Here we can see the root filesystem is 98 Gigabyte disc. it has 69 Gigabyte used and 25 Gigabyte are free and the percentage of the used space is at 74%.

If we want to know what is using the space we can explore the filesystem with tools like

`du -h`{{exec}}

which shows you how much pace the files in certain folders take.
We will tkae a deeper look into this in a later session.
