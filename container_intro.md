# Introduction to Containers for reproducibility
_By Mark Fernandes_

In this course we will explore the use of container technology in delivering 
the goal of reproducible research.    


## Goals for reproducible computing environments   
You've just written your paper and you are required to publish details of 
your analytical pipeline. You publish your code in github so people can download
your programs, scripts and configurations. Job done?  

You then start getting e-mails and github issues from people who are having problems 
running your code - what is happening?  

### __Challenges to software reproducibility__  
1. Language versions - users may have a version of R or Python that differs from the one you 
used. This may affect default behaviour e.g. treating strings as factors   
2. Different versions of installed packages. Our software will often make use of packages. 
These, like the languages, develop and change over time and code written with one version may 
not be supported in an earlier (or later) version.   
3. Underlying Operating System - they may be running your code on a Mac when you used a Windows 
PC (or vice versa). Operating systems may have differences e.g. in how they represent times & 
dates or file paths.   

We can try to overcome these issues by publishing computational environments:-
* Virtual Machines
* Containers 
Virtual Machines (VMs) seek to emulate an entire computer and its operating system. This can be 
very faithful to the real computer and software installation and execution will occur as if on a 
'real' machine.   
The down-side that this uses a similar amount of resources (cpu, ram, disk) as a real machine. 
This can get expensive if we wisk to run more than one VM on our host machine.
