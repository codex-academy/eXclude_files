---
layout : default
title : How do you cleanup
---


# How do you cleanup if you didn't have one

If you already pushed unnecessary files you can easily clean your repository just with a few use of the git commands.

Lets make an example from the following git repository below:

# Diagram .1 Git resitory with Commits

![image-title-here](/img/gitRepoWithUnecessaryFilesExample.png){:class="img-responsive"}

Now lets say we mistakenly added node_modules folder to our repository now we to get rid of it without removing it from our local disk files.


Firstly we are going to execute the following git command:

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`git rm node_modules -r`

and without `-r` flag which it's stands for recursive - we won't be able to remove it.

Then Lets have a commit message by execute the following git command:

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`git commit -m "removed the node_modules folder"`

Then push all these cahnges to github:

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`git push origin master` *depending on the branch that you switched to when you made your changes*


You will follow this Procedure whenever you are thinking of to remove something:

You have to 1stly remove your [files/directory] with the following git command:
`git rm [FILE OR DIRECTORY] -r`;

Then you should commit by writing your commit message with following git command:
`git commit -m "[YOUR COMMIT MESSAGE]"`;

3rdly you should push with following git command:
`git push origin [CURRENT_BRANCH]`;

`NB`This is not a completely different process from the one of adding your files to git, as you will notice that after the `rm` command, you would then do the same as you usually do to upload/Add your local changes to your github.

When we run the following command would then get our git status result showing that we deleted node_modules directory.
