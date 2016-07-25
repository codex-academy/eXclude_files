---
layout : default
title : All about the .gitignore
---

# What is the .gitignore file?

It is a file that you create to avoid other files being pushed to git.
It easily disallows you to upload other project files to Github automatically by its existence into your local project folder.


# Why is it useful to have one ?

You will need it because git will not be able to determine which files are most significant for your project needs, that's when it comes to your file `commits`. So it helps you to reduce data consumption and share your repository with others without them having struggles to know which binary files were required by your application as external sources such that it could be an easy project to work with.


# What happens if I don't have one ?

All your project files would then be STORED, committed with a their messages and pushed.Then when would push your repository it could event take more than a minute which it is not normal process when git cloning a repository. All the non essentials('files') are going to exist on your repository.

<h3>One example. It could be the following:</h3>

` npm.log`

Why whould you commit this file ?... :thought_balloon:
