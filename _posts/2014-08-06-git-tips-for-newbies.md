---
layout: post
title: Git tips for Newbies
comments : true
tags:
- git
- webdevelopment
- sourcecontrol
- frontend
---

When I first started using [Git](http://git-scm.com/), I read as much as possible to get familiar with it, including books and online articles. There's so much good stuff out there but I'm just going to list those things I wish I had known when I started using Git.

git init
----

On a new project, I thought you always had to run <code>git init</code>. Not at all, only run it when you want to create a new repo. So when you do a <code>git clone</code> the git init part is done for you.

git checkout
------------
The <code>git checkout</code> command is done to switch branches. At first I thought running this command automatically gave you the latest commit. Not necessarily. Always run the <code>git pull</code> to get the latest changes. 

collab
------
Git is very smart. It automatically merges code for you and resolves conflicts for you. The only time Git asks you to resolve conflicts is when there has been changes to the exact same line of code. Git cannot decide which change needs to stay so you have to do it manually. I was afraid of working on same files with other devs because of this. But really as long as you don't work in the same line of code, everything will merge fine. Good communication is required with every dev working on the project so everybody knows which part of the file you're working on and vice-versa. Here's a good tip: proper use of comments to separate sections of the file are super helpful.

case sensitive
--------------
I learned this the hard way. Git branches are case sensitive. Let's say you're working on a branch called <code>new_feature</code> and a coworker checks it out and calls their branch <code>new_Feature</code>, it will probably work fine even if they do a pull. But when they do a push you will end up with two branches in origin, so always check the case!

wrong branch?
-------------
Sometimes when you're multitasking and working on different branches you might end up making changes to a file while being on the wrong branch. If you're worried that hitting undo might actually undo stuff that needs to be there just run <code>git checkout -- [file name]</code>. This command discards your changes and sets the file to how it was from last commit. This tip actually shows up when you do a <code>git status</code> command, so always make sure to run it to know the status of your working directory and helpful tips.

I think that's good enough for now. For more good git commands bookmark this [Git Cheat Sheat](http://www.git-tower.com/blog/git-cheat-sheet-detail/).