# How to Contribute to Pro-Tips

* Create a local directory where you want to clone the repo.
For example, create a folder called `vagrant/src/fhp`

* Go to our repo:
https://github.com/FirehoseCommunity/pro-tips

* Click 'Fork' button on the top right side.
It might ask you "Where should we fork this repository?".  If so, pick the correct account.  For example, I have one for an organization and another for my personal account.  I picked my personal account.

* You will see .git file name next to SSH.  Click the button right next to it.  It should say, "copy to clipboard". 
Name of the .git file is something like git@github.com:[your account name]/pro-tips.git, where [your account name] is the name of your GitHub account.

* Go back to your local directory.  For example, using the example above, go to vagrant/src/fhp by typing `cd vagrant/src/fhp`

* In the local directory, create a clone.  Type `git clone git@github.com:[your account name]/pro-tips.git` (the same one you copied to clipboard) Now you creatted a clone repo!

* Go to pro-tips/ directory by typing `cd pro-tips`

* Double check you are in your correct directory (should be in pro-tips/) and create a branch.  To create a branch, type `git checkout -b my-tips`.  Make sure NOT to forget to type `-b` this is a flag to create a branch.  `my-tips` is a branch name.  You can change to whatever the branch name you choose.

* Type `get branch` to make sure you are in the correct branch.  For this example, the asterick is next to my-tips (instead of master) to indicate I am in the correct branch.  

* From here, you can open, edit or add file(s) in pro-tips/ directory using your choice of text editor.

* After editing, do a git add and make a git commit (don't "git push" yet!)
`git add --all`
`git commit -am "[write a comment here]"`

* Now, instead of a standard `git push` command with master branch, you need to push from your branch.  For this exmaple, I created `my-tips` branch, so type:
`git push origin my-tips`

* Go back to your GitHub account: https://github.com/[your account name]/pro-tips.  You should see a message said "Your recently pushed branches:" and the name of your branch under that message. 

* Click "Compare & Pull Request" (the green button on the right).  You should see the page saying "Open a pull request".  The comment you entered when you did `git commit` should also show here.  Write some comments in "Write" tab.  

* Click "Create pull request" (the green button). 

You now created a pull request!




 




