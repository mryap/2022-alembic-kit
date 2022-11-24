---
title: Portable Data Science Tools
date: 2017-09-21 20:59:32 +01:00
description: 'If ultimate portability is all you seek, goes for the cloud options.'
template: post
---

Toying the idea to have a portable data science tools to bring around.  Prior, I being using 
[Anacoda on a Windows PC](http://getoptimise.com/blog/tools/anaconda-vs-miniconda/)

76 days of "enforced" summer breaks without toggling along a laptop means I am away from a computer. If I am lucky, I have internet access on a mobile phone or a desktop with better connectivity but without the data science tools. Wanting to keep up leanring and developing, so my skills are no longer rusty, the idea to have a portable data science tools to bring around ever more sensible. 

Back to Dublin and in a bit of a slump, struggle to get my motivation back and not sure what to be doing with everything. Worse of all, feeling guilty at the same time. I then decide to revisit those DIY project I embark on last year without success. The success of having a SSD and its performace spurred me on https://twitter.com/mryap/status/900776007409520642

**Jupyter on the Cloud**

One option is to use cloud computing. Azure Notebooks looks like a viable options. Jupyter is used as an IDE for both Python and R. This negates the use of seperate RStudio and Python IDE.

**Jupyter in the USB drive**

I am using [Winpython](https://winpython.github.io/) with success. It works when I move WinPython in the following situations.  

* one portable drive to another (USB to portable drive), 
* one directory to another on the same machine.

Nothing breaks. In terms of performance, it bets cloud-hosted Jupyter like Axure Notebooks based on [my own test](https://notebooks.azure.com/mryap/libraries/test123/html/Performance<em>Testing</em>Azure_Local.ipynb)

With Jupyter as the IDE, I learn that:

* to use %%bash magic on Windows, you need to [install cygwin and run ipython from there](https://stackoverflow.com/questions/16281910/ipython-notebook-bash-magic-error). 
* to avoid  "Error in contrib.url(repos, "source"): trying to use CRAN without setting a mirror", you need to run this first
  ![](https://pbs.twimg.com/media/DJnBRK5WsAAWW3P.jpg:large)
* you can use Notepad++ to tinker with the user-interface, Juypton dashboard.   

(https://twitter.com/mryap/status/910825822541447169)

Cygwin gives you the advantage of being able to run linux commands on Windows, act on data and setting up data science 
environment without installing [Ubuntu](https://twitter.com/mryap/status/910275105724538880). These linux commands are useful if you are following good tutorials where linux commands is commonly use compare to Windows PC. 

**Verdict**

Being using Rstudio for sometime, I really love using Jupyter as it allows me to work with both R and Python on the same tool. Don't think I will go back but I am keeping RStudio as now you can use [R Markdown to create website](https://blog.rstudio.com/2017/09/11/announcing-blogdown/) IF you want the quickest, easiest way to get Jupyter notebook up and running, Anaconda is an excellent option. If ultimate portability is all you seek, goes for the cloud options. My favourite option is Winpython https://winpython.github.io/
