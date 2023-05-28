# os161
"Programmazione di Sistema" Labs @PoliTo - Computer Engineering Master Degree

This repo are my personal solutions for "Programmazione di Sistema" Labs.
I struggled with create several version of os161 because several reason (versioning it's not so easy "The upstream version control for OS/161 is a nightmare. Each solution set or solution fragment needs to be a branch, which is bad enough; 
plus when things are under active development it is essential that each changeset be merged from one branch to the next in the right order, never skipping any or going in the wrong order at the risk of creating potentially unfixable problems." [1](http://www.os161.org/resources/versioncontrol.html)).

I solved in this way:
1) cloning the clean version of os161
2) change the variable at this path
```c
/home/os161user/<clonedfolder>/src/defs.mk
```
```c
OSTREE=/home/os161user/os161/root
```
in
```c
OSTREE=/home/os161user/<clonedfolder>/root
```
