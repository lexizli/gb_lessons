# It's the first homework for Git seminar

What is a Git?
> Git is a free and open source distributed version control system
---

![Common Git commands](https://res.cloudinary.com/practicaldev/image/fetch/s--ShHSfi-a--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://cl.ly/1N2U2i2Z2C16/Image%25202018-04-11%2520at%252012.47.23%2520PM.png)

<a id="top"></a>

---
## Let's try to describe some commands that we have learned  
* [git config](#config)
* [git init](#init)
* [git add](#add)
* [git commit](#commit)
* [git status](#status)
* [git log](#log)
* [Branches](#branch)
* [git checkout](#checkout)
* [Merging](#merge)
* [Conflictes](#conflict)

<a id="config"></a>

---
## git config

Set the name _John Doe_ and email _john_d_email@mail.com_ that will be attached to commits and tags.
```
git config --global user.name "John Doe"
git config --global user.email "john_d_email@mail.com"
```
[top](#top)

<a id="init"></a>

---
## git init

Create a local repo in _directory_.
If omit _directory_ current directory will be initialised as repo.
```
git init <directory>
```
[top](#top)

<a id="add"></a>

---
## git add

Add _file_ content to the index. 

Add all files in directory if used the dot .

```
git add <file>
git add .
```
[top](#top)

<a id="commit"></a>

---
## git commit

Commit all added files to index with _comment_.

```
git commit -m <comment>
```
[top](#top)

<a id="status"></a>

---
## git status

Show working tree status — differences between the index file and the current HEAD
 commit. 

```
git status 
```
[top](#top)

<a id="log"></a>

---
## git log

Show the commit logs.

```
git log
```
[top](#top)

<a id="branch"></a>

---

## Branches, git branch and other ways for branch creating and swiching

```
git branch [options]
```
Create, list or delete branches. WIth _branch_name_ create this branch. Full optoins list is [here](https://git-scm.com/docs/git-branch).

Create branch _branch_name_

```
git branch <branch_name>
```
Alternate ways:

Fast creation and checkout
```
git checkout -b <newbranchname>
```
New (from Git 2.23)

Now, from Git version 2.23, we have a new command for branch changing and creating.

Changing branch to _some_branch_:
```
git switch <some_branch>
```

Creating and changing to _new_branch_:
```
git switch -c <new_branch>
```

[top](#top)

<a id="checkout"></a>

---
## git checkout

Switch to a branch _branch_name_ and update the working directory

```
git checkout <branch_name>
```

Or create a new branch _branch_name_ and switch to it.

```
git checkout -b <branch_name>
```

[top](#top)

<a id="merge"></a>

---
## Merging

You or somebody else made work on some part of project and now it's need to add this part in our project. For this you have to use something like this (merge _added_branch_ to current:

```
git merge <added_branch>
```
[top](#top)

<a id="conflict"></a>

---
## Conflicts in merging

Sometimes merging has problems. 

![add some humor about merging](https://devhumor.com/content/uploads/images/July2020/merge.jpg)

[top](#top)
