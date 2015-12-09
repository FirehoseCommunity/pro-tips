# How to Contribute to Pro-Tips

* Create a local directory where you want to clone the repo.
For example, create a folder called `vagrant/src/fhp`

* Go to our repo:
https://github.com/FirehoseCommunity/pro-tips

* Click 'Fork' button on the top right side.
It might ask you "Where should we fork this repository?".  If so, pick the correct location.  For example, I have one for an organization and another for my personal account.  I picked my personal account.

* You will see .git file name next to SSH.  Click the button right next to it.  It should say, "copy to clipboard". 
Name of the .git file is something like git@github.com:[your account name]/pro-tips.git, where [your account name] is the name of your GitHub account.

* Go back to your local directory.  For example, using the example above, go to `vagrant/src/fhp`

* In the local directory, create a clone.  Type `git clone git@github.com:[your account name]/pro-tips.git`.  Now you creatted a clone repo!

* Go to pro-tips/ directory by typing `cd pro-tips`

* Double check you are in your correct directory (should be in pro-tips/) and create a branch.  To create a branch, type `git checkout -b my-tips`.  Make sure not to forget `-b` this is a flag to create a branch.  `my-tips` is the branch name.  You can change to whatever the branch name you want.

* Type `get branch` to make sure you are in correct branch.  The * should be next to the branch you just created.  For this example, * is next to my-tips (instead of master).  

* From here, you can open, edit or add file(s) in pro-tips/ directory using your choice of text editor.

* After editing, make a git commit.
`git add --all`
`git commit -am "[write a comment here]"`



 




