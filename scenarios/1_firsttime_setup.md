# GitHub for open source collaboration on parsons.nyc

### Scenario: Forking the repository for the first time

This document describes a common scenario in the [MSDV GitHub Workflow](https://github.com/visualizedata/github-workflow): forking the [visualizedata.github.io repository](https://github.com/visualizedata/visualizedata.github.io). You only need to do this once in preparation for making contributions to [https://parsons.nyc/](https://parsons.nyc/) 

This documentation is adapted from: [https://help.github.com/articles/fork-a-repo/](https://help.github.com/articles/fork-a-repo/)

#### 1. Fork

First, go to: [https://github.com/visualizedata/visualizedata.github.io](https://github.com/visualizedata/visualizedata.github.io)

In the top-right corner of the page, click the "Fork" button: 

![](https://github-images.s3.amazonaws.com/help/bootcamp/Bootcamp-Fork.png)

#### 2. Create a local clone of your fork

In the terminal, navigate to the subdirectory on your computer where you want to save this repository. Then run this command after changing `YOUR-USERNAME` to your GitHub username: 

`git clone https://github.com/YOUR-USERNAME/visualizedata.github.io.git`

#### 3. Configure Git to sync your fork with the Parsons visualizedata.github.io repository

On your GitHub page, navigate to the forked repository you created in step 1. Under the repository name, click **Clone or Download**. Click the "copy" icon to copy the clone URL for the repository. 

Back in the terminal, in the directory where you saved the `visualizedata.github.io` clone, type `git remote -v` and press Enter. You should see: 

```
$ git remote -v
origin  https://github.com/YOUR_USERNAME/visualizedata.github.io.git (fetch)
origin  https://github.com/YOUR_USERNAME/visualizedata.github.io.git (push)
```

Type and run this command:  
`git remote add upstream https://github.com/visualizedata/visualizedata.github.io.git`

Type `git remote -v` again and you should see something like:  
```
$ git remote -v
origin    https://github.com/YOUR_USERNAME/visualizedata.github.io.git (fetch)
origin    https://github.com/YOUR_USERNAME/visualizedata.github.io.git (push)
upstream  https://github.com/visualizedata/visualizedata.github.io.git (fetch)
upstream  https://github.com/visualizedata/visualizedata.github.io.git (push)
```

#### Done!

You're now ready to move to Step 2 in the [MSDV GitHub workflow](https://github.com/visualizedata/github-workflow). 