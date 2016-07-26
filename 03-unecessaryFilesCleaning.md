---
layout : default
title : How do you cleanup
---


# How do you cleanup if you didn't have one

If you already pushed unnecessary files you can easily clean your repository just with a few use of the git commands.

Lets make an example from the following git repository below: :bulb:

# Diagram .1 Git resitory with Commits

![image-title-here](/img/gitRepoWithUnecessaryFilesExample.png){:class="img-responsive"}

Now lets say we mistakenly added node_modules folder to our repository now we to get rid of it without removing it from our local disk files.


Firstly we are going to execute the following git command to remove `1.` `node_modules`:

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`git rm node_modules -r`

and without `-r` flag which it's stands for recursive - we won't be able to remove it.

Then Lets have a commit message by execute the following git command:

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`git commit -m "removed the node_modules folder"`

Then push all these changes to github:

<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox">
`git push origin master` *depending on the branch that you switched to when you made your changes*

Then you will have to check status by executing following git command:

`git status`

You should get the following as an output:


![image-title-here](/img/gitStatusWithUntrackedUselessFiles.png){:class="img-responsive"}

Then you are on the right track the only thing that you will need to do is to create your gitignore file.

To do so you can go the following link :point_right: [create the gitignore file](/02-HowTocreateIt.html).

theeafter from above link you will then see how is it been created on the terminal. with that you accomplished the cleaning up process. :+1:

<br />

# You will follow this Procedure

1stly you have to remove your [files/directory] with the following git command:

`git rm [FILE OR DIRECTORY] -r`;

Then you should commit by writing your commit message with following git command:

`git commit -m "[YOUR COMMIT MESSAGE]"`;

Finally you will have to push with following git command:

`git push origin [CURRENT_BRANCH]`;

# :arrow_up: That's how you would clean up your.

`NB` This is not a completely different process from the one of adding your files to git, as you will notice that after the `rm` command, you would then do the same as you usually do to upload/Add your local changes to your github.

Now you shouldn't see  the `1.``node_modules` folder on your github repository unless if you haven't refreshed your browser.
