# Quick Reference List

## Common Terminal Commands

### Git

&nbsp;&nbsp;**Create Initial Directory:** `git init .`

&nbsp;&nbsp;**Display Status:** `git status`

&nbsp;&nbsp;**Add to Directory:** `git add --all`

&nbsp;&nbsp;**Commit:** `git commit -am "Did something awesome."`

&nbsp;&nbsp;**Undo Commit:**	`git stash`

&nbsp;&nbsp;**Redo Commit:**	`git stash apply`

&nbsp;&nbsp;**Push to GitHub Master:** `git push origin master`

&nbsp;&nbsp;**Push to Heroku Master from GitHub:**	`git push heroku master`

&nbsp;&nbsp;**Clone from GitHub:** `git clone git@github.com:[your account name]/pro-tips.git`

&nbsp;&nbsp;**Pull from GitHub Master:** `git pull origin master`

&nbsp;&nbsp;**Display All Changes:** `git diff`

&nbsp;&nbsp;**Display Branches:**	`git branch`

&nbsp;&nbsp;**Create New Branch:** `git branch newbranchname`

&nbsp;&nbsp;**Change Branch:** `git checkout branchname`

&nbsp;&nbsp;**Merge Branch:**	`git merge branchname`

### Heroku

&nbsp;&nbsp;**Create New Empty Database:** `heroku run rake db:create`

&nbsp;&nbsp;**Run Migration:** `heroku run rake db:migrate`

&nbsp;&nbsp;**Drop Database:** `heroku pg:reset DATABASE`

&nbsp;&nbsp;**Run Rails Console:** `heroku run console`

&nbsp;&nbsp;**Restart Heroku:**	`heroku restart`

### Rails

&nbsp;&nbsp;**Start Server:** `rails server`

&nbsp;&nbsp;**Create New Controller:** `rails generate controller xx`

&nbsp;&nbsp;**Create New Model:**	`rails generate model xx`

&nbsp;&nbsp;**Show Routes:** `rake routes`

&nbsp;&nbsp;**Destroy Controller:**	`rails destroy controller xx`

&nbsp;&nbsp;**Destroy Model:** `rails destroy model xx`

&nbsp;&nbsp;**Create New Empty Database:** `rake db:create`

&nbsp;&nbsp;**Create Migration:**	`rails generate migration xxx`

&nbsp;&nbsp;**Run Migration:** `rake db:migrate`

&nbsp;&nbsp;**Drop Database:** `rake db:drop`

### Rails Console

&nbsp;&nbsp;**Use/Exit Rails Console:**	`rails console/exit`

&nbsp;&nbsp;**Create Record:** `Model.create(:column => 'value')`

&nbsp;&nbsp;**Display All Records:** `Model.all`

&nbsp;&nbsp;**Display All Records Formatted:** `y Model.all`

&nbsp;&nbsp;**Delete Record:** `Model.find(id).destroy`

&nbsp;&nbsp;**Delete All Records:**	`Model.delete_all`

&nbsp;&nbsp;**Show All Tables:** `ActiveRecord::Base.connection.tables`

## Naming Conventions

&nbsp;&nbsp;**Models:** singular, capital, CamelCase

&nbsp;&nbsp;**Controllers:** always plural

&nbsp;&nbsp;**Database table:** plural, lowercase, snake_case

&nbsp;&nbsp;**Association:** if you have many, it’s plural, if you have one , it’s singular
