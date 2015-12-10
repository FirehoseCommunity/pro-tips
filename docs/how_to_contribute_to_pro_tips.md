# How to Contribute to Pro-Tips

1. Create a local directory where you want to clone the repo.
For example, create a folder called `vagrant/src/fhp`

2. Go to our repo:
https://github.com/FirehoseCommunity/pro-tips

3. Click 'Fork' button on the top right side.
It might ask you "Where should we fork this repository?".  If so, pick the correct account.  For example, I have one for an organization and another for my personal account.  I picked my personal account.

4. You will see .git file name next to SSH.  Click the button right next to it.  It should say, "copy to clipboard". 
Name of the .git file is something like git@github.com:[your account name]/pro-tips.git, where [your account name] is the name of your GitHub account.

5. Go back to your local directory.  For example, using the example above, go to vagrant/src/fhp by typing `cd vagrant/src/fhp`

6. In the local directory, create a clone.  Type `git clone git@github.com:[your account name]/pro-tips.git` (the same one you copied to clipboard) Now you creatted a clone repo!

7. Go to pro-tips/ directory by typing `cd pro-tips`

8. Double check you are in your correct directory (should be in pro-tips/) and create a branch.  To create a branch, type `git checkout -b my-tips`.  Make sure NOT to forget to type `-b` this is a flag to create a branch.  `my-tips` is a branch name.  You can change to whatever the branch name you choose.

9. Type `git branch` to make sure you are in the correct branch.  For this example, the asterick is next to my-tips (instead of master) to indicate I am in the correct branch.  

10. From here, you can open, edit or add file(s) in pro-tips/ directory using your choice of text editor.  If you are creating a new documentation, our current recommentions are:
  * Create *.md file and put it under docs/ directory.
  * Make a link to this newly created documentation from README.md
  * Add your name in README.md and put a link to your GitHub account.

11. After editing, do a git add and make a git commit (don't "git push" yet!)
`git add --all`
`git commit -am "[write a comment here]"`

12. Now, instead of a standard `git push` command with master branch, you need to push from your branch.  For this exmaple, I created `my-tips` branch, so type:
`git push origin my-tips`

13. Go back to your GitHub account: https://github.com/ [your account name] /pro-tips.  You should see a message said "Your recently pushed branches:" and the name of your branch under that message. 

14. Click "Compare & Pull Request" (the green button on the right).  You should see the page saying "Open a pull request".  The comment you entered when you did `git commit` should also show here.  Write some comments in "Write" tab.  

15. Click "Create pull request" (the green button). 

You now created a pull request!

To learn more about creating a pull request, see the following links.



[How to Fork a Repo and Contribute](http://community.thefirehoseproject.com/2015/08/19/How-To-Fork-A-Repo-And-Contribute.html)


[Pull Request Lesson](http://www.thefirehoseproject.com/advanced-git-topics/4)

### Syncing a Fork

Let's say you create a pull request, and your document is merged, and you are very happy.  But what if you want to create another document one week later?  Here's how to sync your fork.


1. Go to your local diretory, and type:  `git remote -v`

   You will see: 

   origin https://github.com/ [your account name] / pro-tips.git (fetch)

   origin https://github.com/ [your account name] / pro-tips.git (push)

2. Set a new upstream repo to FirehoseCommunity/pro-tips repo by typing:

   `git remote add upstream https://github.com/FirehoseCommunity/pro-tips.git`

3. Type  `git remote -v` to see if a new upstream repo is specified.  Along with origin, you should see:

   upstream https://github.com/FirehoseCommunity/pro-tips.git (fetch)

   upstream  https://github.com/FirehoseCommunity/pro-tips.git (push)

4. Make sure you are on master branch by typing `git checkout master`  (also verify by typing `git branch`)

5. Fetch the upstream repo by typing, `git fetch upstream`

6. Merge the change from upstream/master to your local master branch by typing `git merge upstream/master`

7. When you open the files, you should see all the files are up to date.  From here, you can go back to Step 8 above, create a branch and follow the subsequent steps to create a pull request again.

For more information about syncing a fork, see:

https://help.github.com/articles/syncing-a-fork/

https://help.github.com/articles/configuring-a-remote-for-a-fork/