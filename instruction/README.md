:point_right: **Task 1**: Fork this repository  

:point_right: **Task 2**: Clone your forked repository to your local  

:point_right: **Task 3**: Create a new branch named `devel`  

:point_right: **Task 4**: Checkout the `devel` branch  

:point_right: **Task 5**: Open a text editor (I you don't have one download vs code https://code.visualstudio.com/download)  

:point_right: **Task 6**: Change the README file in the top folder, by adding the followings   
```
# Header 1
## Header 2
### Header 3
#### Header 4
```

:point_right: **Task 7**: run the following command to see if git can see your changes
```
$ git status
```

:point_right: **Task 8**: Stage your changes by running the following command:
```
$ git add README.md
```

:point_right: **Task 9**: Commit your changes to your local repo
```
$ git commit -m 'your-github-id: task 1 to 9 done'
```

:point_right: **Task 10**: run the following command to see if your commit is recorded in local git
```
$ git log
```

:point_right: **Task 11**: Push your changes to remote repo
```
$ git push origin devel
```

:point_right: **Task 12**: Go to your remote and check if your changes are there

:point_right: **Task 13**: Creaet a pull request from your `devel` branch to your `master` branch.
Note: the pull should be to **your** master branch not the upstream forked branch

:point_right: **Task 14**: Check the changes and merge the pull request to master branch.

:point_right: **Task 15**: On your local repo checkout the `master` branch by running the following command:
```
$ git checkout master
```
Observe your local README file is reverted back to its original

:point_right: **Task 16**: Merge your local devel branch into you master branch
```
$ git merge devel
```
Observe your local README file now has your changes

:point_right: **Task 17**: See list of all your local branches by running:
```
$ git branch -a
```

:point_right: **Task 18**: Delete the old `devel` branch by running the following command:
```
$ git branch -D devel
```

:point_right: **Task 19**: See if devel branch is deleted from your local
```
$ git branch -a
```

:point_right: **Task 20**: Delete your remote devel branch as well by going to `branches` tab in the repo's GitHub page


## This part will create a merge conflict

:point_right: **Task 21**: Make the following change in the remote repo by editing the file in the browser.
```
This keyword is **bold**
```

:point_right: **Task 22**: Create a new branch named `content_update`
```
$ git branch content_update
```

:point_right: **Task 23**: checkout `content_update` branch
```
$ git checkout content_update
```

:point_right: **Task 24**: Add the followin to the README
```
This is a link to [google](https://www.google.com)
```

:point_right: **Task 24**: Add and commit your changes
```
$ git add .
$ git commit -m 'your-github-id: updated README file'
```

:point_right: **Task 25**: Push your changes to remote
```
$ git push origin content_update
```

:point_right: **Task 26**: Try to create a pull request and observe there is merge conflict

:point_right: **Task 27**: On your local checkout master branch
```
$ git checkout master
```

:point_right: **Task 28**: On your local pull the latest remote update from master branch to your local
```
$ git pull
```

:point_right: **Task 29**: Checkout the content_update branch
```
$ git checkout content_update
```

:point_right: **Task 29**: Merge master branch to your content_update branch
```
$ git merge master
```
Observer there is merge conflict

:point_right: **Task 30**: Open a code editor and accept both changes

:point_right: **Task 31**: add and commit and push your changes

```
$ git add .
$ git commit -m 'your-github-id: fixed merge conflict'
$ git push origin content_update
```

:point_right: **Task 32**: From the remote repo create a pull request. Check the changes and merge to your remote master branch.
