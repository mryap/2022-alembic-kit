---
title: The Business of Container
date: 2017-11-15 14:23:09 +00:00
description: Say “Docker”, and you quite possibly mean lightweight virtual machine 
  using Linux technology.
template: post
---

When you mention Excel, you mean spreadsheet. Say “Docker”, and you quite possibly mean lightweight virtual machine using Linux technology.

You can run Skype, Firefox browser, office suite, database etc in a Container. This Container can run on every Operating System from your desktop PC, Server or in the Cloud.

The best definition of Docker is from  Hackterms 

> Docker is a tool that bundles all of the files, programs, libraries, and configuration needed by a program into a single unit (called an image) and then to run that program in an isolated manner (called a contained) with controllable access to your local files and network.

>
> This make it simpler and safer (but nothing is 100% safe) to run things on systems. The simplicity that this offers enables docker containers to be moved around easily and quickly.
>
>
Bundling all of the files, programs, libraries, and configuration into one unit helps ensure that a program is running with the exact same way as it was tested since development, testing, and production can use the same image.

For enduser, Docker offers software on demand without messing up their PC system. Once done with, you delete the Container.

**Analogies**
Docker has being refer to as apartment building. Various apartment unit share the plumbing, heating, electrical all under one roof. It has its own door. The roof is your own PC consider as the host*

With Docker, you can keep a copy of your WordPress site just like the actual one running by your hosting provider.

**Container in the data science domain**

Think of Docker container as a zip file. A zip file that also includes a full-fledged software application that runs the data analysis code.

If you need to handover the data analysis in the exact computer set-up so your client or project stakeholder can run at their end and keep it on-premise, Docker Container is the way. Container is one of the end product of a data analysis.

[Fighting with dependencies](https://en.wikipedia.org/wiki/Dependency_hell) is can be difficult; nobody wants to sink hours  into sorting out which version of which package is needed to reproduce the data analytics results.  Like version control for code, a Docker image allows you to go back - allowing you to experiment fearlessly without messing up your PC .

With Docker, Data analyst/Data Scientist can make their [work immediately useful to software developers](http://blog.ibmjstart.net/2016/01/28/jupyter-notebooks-as-restful-microservices/) to turn into products and services.

**Training**

In terms of learning, setting up a data science environment is difficult. For instructor/lecturer, even though you told the students what they needed well in advance of the class, you still had a lot of problems configuring students’ systems. Docker container is the solution for you.

**Let Get Down to Business**

You can start using Docker with a tool called [Kitematic](https://kitematic.com/). It is a

* simple Graphical User Interface for launching and managing containers. Point and click without typing command.
* great place to start for less technical people



**Docker for Data Science**

Here is a Docker container that lets you run Jupyter notebook <https://github.com/mryap/docker-ds>

**Conclusion**

You can think of Docker as providing you a laptop

* without an operating system
* pre-installed with all the software you need for a particular task and
* built for a single purpose — running your program or application.

You can “ship” this container to any OS as well as in the Cloud and it will just work.

Docker helps you resolve the "works on my machine, but doesn't work on my boss or client machine" conundrum.

All these without the overhead of a Virtual Machine.

```
* https://blog.docker.com/2016/03/containers-are-not-vms/

^ If you are on Windows, run the installer and make sure the checkbox to install Virtualbox 
is checked if you don't already have Virtualbox or another virtualization platform 
(like VMWare Workstation) installed
```

https://containerjournal.com/2017/09/22/microsoft-embrace-containers-face-extinction/
