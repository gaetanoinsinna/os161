# os161
"Programmazione di Sistema" Labs @PoliTo - Computer Engineering Master Degree

This repo are my personal solutions for "Programmazione di Sistema" Labs.
I struggled with create several version of os161 because several reason (versioning it's not so easy [1](http://www.os161.org/resources/versioncontrol.html)).

I solved in this way:
1) cloning the clean version of os161
2) go to ```defs.mk``` in ```<clonedfolder>/src```
```c
<clonedfolder>/src/defs.mk
```
3) change ```OSTREE```
```c
OSTREE=/home/os161user/os161/root
```
in
```c
OSTREE=/home/os161user/<clonedfolder>/root
```

# docker-container
Some useful commands:

```
docker cp <SOURCE-PATH> <DEST-PATH>
```
In order to access to the path you have to prepend the name of the container

```
<CONTAINER-NAME>:/home/os161user

```
To copy the folder from os161 to our filesys, we could use:
```
docker cp polito-os161:/home/os161user/os161 /Users
```
