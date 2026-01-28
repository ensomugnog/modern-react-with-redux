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

  - [x] 06 - A Few More Critical Questions

  - [x] 07 - Node Setup

  - [x] 08 - Generating a React Project with Vite

  - [x] 09 - Generating a React Project with Create React App [ [mrwr-jsx](https://github.com/ensomugnog/mrwr-jsx) -> [6c16eb50dc50c4d1b2623314f8caaf6ee513d007](https://github.com/ensomugnog/mrwr-jsx/commit/6c16eb50dc50c4d1b2623314f8caaf6ee513d007) ]

  - [x] 10 - What is Create React App

  - [x] 006 - Core Concepts

  - [x] assets

  - [x] external-links

- [x] 02 - Creating Content with JSX

  - [x] 01 - Showing Basic Content [ [mrwr-jsx](https://github.com/ensomugnog/mrwr-jsx) -> [c97934dcb1baea6b89384649fbbb52bfb3693723](https://github.com/ensomugnog/mrwr-jsx/commit/c97934dcb1baea6b89384649fbbb52bfb3693723) ]

  - [x] 02 - What is JSX

  - [x] 03 - Printing JavaScript Variables in JSX [ [mrwr-jsx](https://github.com/ensomugnog/mrwr-jsx) -> [f23a5d5cfaf951b2ec2bd8686f13b2cbe901b3a0](https://github.com/ensomugnog/mrwr-jsx/commit/f23a5d5cfaf951b2ec2bd8686f13b2cbe901b3a0) ]

  - [x] 04 - Shorthand JS Expressions [ [mrwr-jsx](https://github.com/ensomugnog/mrwr-jsx) -> [418aba4827155750cd78065ffec4314788b5510a](https://github.com/ensomugnog/mrwr-jsx/commit/418aba4827155750cd78065ffec4314788b5510a) ]

  - [x] 05 - Exercise Overview

## Repository configuration
Each submodule in this repository contains the code examples of the original course.

### Create new submodules
Create a new repository on Github, then execute the following commands to link the new repository as a submodule of the main repository:

```
$ cd modern-react-with-redux
$ git submodule add -b main git@github.com:ensomugnog/mrwr-jsx.git
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