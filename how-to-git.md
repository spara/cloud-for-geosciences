# Git for Geosciences

Git is a version-control system for tracking changes in computer files and coordinating work on those files among multiple people. Git is a Distributed Version Control System. So Git does not necessarily rely on a central server to store all the versions of a project’s files. Instead, every user “clones” a copy of a repository (a collection of files) and has the full history of the project on their own hard drive. This clone has all of the metadata of the original while the original itself is stored on a self-hosted server or a third party hosting service like GitHub.

Git helps you keep track of the changes you make to your code. It is basically the history tab for your code editor(With no incognito mode ?). If at any point while coding you hit a fatal error and don’t know what’s causing it you can always revert back to the stable state. So it is very helpful for debugging. Or you can simply see what changes you made to your code over time.

## History

Torvalds: I really never wanted to do source control management at all and felt that it was just about the least interesting thing in the computing world (with the possible exception of databases ;^), and I hated all SCM’s with a passion. But then BitKeeper came along and really changed the way I viewed source control. BK got most things right and having a local copy of the repository and distributed merging was a big deal. The big thing about distributed source control is that it makes one of the main issues with SCM’s go away – the politics around “who can make changes.” BK showed that you can avoid that by just giving everybody their own source repository. But BK had its own problems, too; there were a few technical choices that caused problems (renames were painful), but the biggest downside was the fact that since it wasn’t open source, there was a lot of people who didn’t want to use it. So while we ended up having several core maintainers use BK – it was free to use for open source projects – it never got ubiquitous. So it helped kernel development, but there were still pain points.

That then came to a head when Tridge (Andrew Tridgell) started reverse-engineering the (fairly simply) BK protocol, which was against the usage rules for BK. I spent a few weeks (months? It felt that way) trying to mediate between Tridge and Larry McVoy, but in the end it clearly wasn’t working. So at some point I decided that I can’t continue using BK, but that I really didn’t want to go back to the bad old pre-BK days. Sadly, at the time, while there were some other SCM’s that kind of tried to get the whole distributed thing, none of them did it remotely well.  I had performance requirements that were not even remotely satisfied by what was available, and I also worried about integrity of the code and the whole workflow, so I ended up just deciding to write my own.

How did you approach it? Did you stay up all weekend to write it or was it just during regular hours?

Torvalds: Heh. You can actually see how it all took shape in the git source code repository, except for the very first day or so. It took about a day to get to be “self-hosting” so that I could start committing things into git using git itself, so the first day or so is hidden, but everything else is there. The work was clearly mostly during the day, but there’s a few midnight entries and a couple of 2 a.m. ones. The most interesting part is how quickly it took shape ; the very first commit in the git tree is not a lot of code, but it already did the basics – enough to commit itself. The trick wasn’t really so much the coding but coming up with how it organizes the data.

So I’d like to stress that while it really came together in just about ten days or so (at which point I did my first *kernel* commit using git), it wasn’t like it was some kind of mad dash of coding. The actual amount of that early code is actually fairly small, it all depended on getting the basic ideas right. And that I had been mulling over for a while before the whole project started. I’d seen the problems others had. I’d seen what I wanted to avoid doing. 

## Getting Started: Creating and Setting Up an Account

https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github



#### Generate a key









```python
$ git config --global user.name "YOUR_USERNAME"

$ git config --global user.email "im_satoshi@musk.com"

$ git config --global --list # To check the info you just provided
```

### Authentication

#### Generate a key


```python

```

#### Add a key


```python

```

## First Repository


```python
mkdir mycode
cd mycode
touch README.md
git init
git remote set-url origin https://github.com/spara/git-for-geosciences.git
git push -u orgin main

```


```python

```
