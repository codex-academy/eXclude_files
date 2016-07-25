---
layout : default
title : Create the .gitignore file
---

# How to create the .gitignore file

Here we are going to use the terminal in order to create it just to make things easy for us.

notice. We will do the exact thing that would've been done on any of our favorite text editor program *eg.Atom*
but for now we are going to create this file by using our terminal with commands.

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`nano .gitignore`

or

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`touch .gitignore`


The only difference between these commands it's that the first command opens a file *it is as if we are already having this file existing within our project folder* then the second command creates file *The file doesn't not exist* We just want to create a new file instance.

# What should lie inside this file ?

We should reference our file directories or a specific file by specifying proper file path line on this file.

# Daigram.1 Project files

![image-title-here](/img/filesEx.png){:class="img-responsive"}

An example of project files and with a file list output when executed `ls -al`command its easy to see which files to exclude


Check you local file changes by executing the following git command:

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`git status`

This should be the output before adding the files to git and if it happens that you havent yet uploaded  your files to git it will be advantageous to create the gitignore to ignore all the files of your choice before adding other file changes to git.

![image-title-here](/img/untrackedFileEx.png){:class="img-responsive"}

now from above example you don't want to upload the bower_components directory and your node_modules so you will have to reference these two directories by typing the following to your .gitignore file:

<pre><code>/node_modules
/bower_components
</code></pre>

The next thing to do is to check if your file are still showing up as untracked files which you would then think that it would be nice to upload them to git.

Then you will have to check if the .gitignore file works exactly like the way you want by executing the following git command:

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`git status`

then you should get the next output as the result of that gitignore file which you will then add it to git.

![image-title-here](/img/statusExample.png){:class="img-responsive"}

Untracked files should no longer show excluded files or directories which you already referenced in the `.gitignore` file .
