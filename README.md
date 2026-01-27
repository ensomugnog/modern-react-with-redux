# MRWR - Modern React with Redux (Stephen Grider)
Master React and Redux. Apply modern design patterns to build apps with React Router, TailwindCSS, Context, and Hooks!

**Course**: [https://www.udemy.com/course/react-redux](https://www.udemy.com/course/react-redux)

## Course content

- [x] 01 - Let's Dive In!

  - [x] 01 - How to Get Help

  - [x] 02 - Join Our Community!

  - [x] 03 - Course Resources

  - [x] 04 - Let's Build an App! [ [mrwr-language-translation](https://github.com/ensomugnog/mrwr-language-translation) -> [74c697dfaab4edee3e80e10076e7d0356bcc9557](https://github.com/ensomugnog/mrwr-language-translation/commit/74c697dfaab4edee3e80e10076e7d0356bcc9557) ]

  - [x] 05 - Critical Questions

## Repository configuration
Each submodule in this repository contains the code examples of the original course.

### Create new submodules
Create a new repository on Github, then execute the following commands to link the new repository as a submodule of the main repository:

```
$ cd modern-react-with-redux
$ git submodule add -b main git@github.com:ensomugnog/mrwr-language-translation.git mrwr-language-translation
```

Using the **-b** argument means we want to follow the main branch of the new repository, and after running this command we’ll have a new directory named `mrwr-submodule/`, this directory will automaticaly checkout the main branch for you to be ready to make changes.

### Update main repository with latest submodule changes
First make sure the submodule changes have been commited and pushed to the orign repository, then run the following commands:

```
$ git status
$ git stage .
$ git commit -m 'mrwr-submodule'
$ git push
```

### Clone Repository with submodules
If you want to clone a repository including its submodules you can use the --recursive parameter, use the --jobs parameter to fetch multiple submodules at the same time, download up to 8 submodules at once use --jobs 8

```
$ git clone --recursive --jobs 8 git@github.com:ensomugnog/modern-react-with-redux.git
```

### Delete a submodule from a repository
Currently Git provides no standard interface to delete a submodule. To remove a submodule `mrwr-submodule` you need to:

```
$ git submodule deinit -f mrwr-submodule
$ rm -rf .git/modules/mrwr-submodule
$ git rm -f mrwr-submodule
```

### Checkout a commit
To checkout a Git commit, you will need the commit hash.

```
$ git checkout 4aa03973d004286558465a8d86bcccfdc7b46505
$ git reset --hard
$ git checkout main
```