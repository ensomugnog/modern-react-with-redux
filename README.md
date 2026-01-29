# MRWR - Modern React with Redux (Stephen Grider)
Master React and Redux. Apply modern design patterns to build apps with React Router, TailwindCSS, Context, and Hooks!

**Course**: [https://www.udemy.com/course/react-redux](https://www.udemy.com/course/react-redux)

## Course Content Completion (3.7%)

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

  - [x] 06 - Exercise Solution [ [mrwr-quick-practice-with-jsx](https://github.com/ensomugnog/mrwr-quick-practice-with-jsx) -> [a893bdeb8231662074d4127fbf36103d3d487e52](https://github.com/ensomugnog/mrwr-quick-practice-with-jsx/commit/a893bdeb8231662074d4127fbf36103d3d487e52) ]

  - [x] 07 - Typical Component Layouts [ [mrwr-jsx](https://github.com/ensomugnog/mrwr-jsx) -> [1d0e679edf90ef3de9f269b970c85bca28d3656e](https://github.com/ensomugnog/mrwr-jsx/commit/1d0e679edf90ef3de9f269b970c85bca28d3656e) ]

  - [x] 08 - Customizing Elements with Props [ [mrwr-jsx](https://github.com/ensomugnog/mrwr-jsx) -> [1012516dd6776864a8f969ab14c6daedb52cc9dd](https://github.com/ensomugnog/mrwr-jsx/commit/1012516dd6776864a8f969ab14c6daedb52cc9dd) ]

  - [x] 09 - Converting HTML to JSX [ [mrwr-jsx](https://github.com/ensomugnog/mrwr-jsx) -> [daef59cc400854dabb2bc72241024f19bb643f95](https://github.com/ensomugnog/mrwr-jsx/commit/daef59cc400854dabb2bc72241024f19bb643f95) ]

  - [x] 10 - Applying Styling in JSX [ [mrwr-jsx](https://github.com/ensomugnog/mrwr-jsx) -> [4a797c13f1cbc897984dfe513ecd905090819734](https://github.com/ensomugnog/mrwr-jsx/commit/4a797c13f1cbc897984dfe513ecd905090819734) ]

  - [x] 11 - Exercise Solution [ [mrwr-practice-jsx-conversion](https://github.com/ensomugnog/mrwr-practice-jsx-conversion) -> [233085727063ab9b4b1caebbbec171583003351a](https://github.com/ensomugnog/mrwr-practice-jsx-conversion/commit/233085727063ab9b4b1caebbbec171583003351a) ]

## Repository Configuration
Each submodule in this repository contains the code examples of the original course.

### Create New Submodules
Create a new repository on Github, then execute the following commands to link the new repository as a submodule of the main repository:

```
$ cd modern-react-with-redux
$ git submodule add -b main git@github.com:ensomugnog/mrwr-practice-jsx-conversion.git
```

Using the **-b** argument means we want to follow the main branch of the new repository, and after running this command we’ll have a new directory named `mrwr-submodule/`, this directory will automaticaly checkout the main branch for you to be ready to make changes.

### Update Main Repository with Latest Submodule Changes
First make sure the submodule changes have been commited and pushed to the orign repository, then run the following commands:

```
$ git status
$ git stage .
$ git commit -m 'mrwr-submodule'
$ git push
```

### Clone Repository with Submodules
If you want to clone a repository including its submodules you can use the --recursive parameter, use the --jobs parameter to fetch multiple submodules at the same time, download up to 8 submodules at once use --jobs 8

```
$ git clone --recursive --jobs 8 git@github.com:ensomugnog/modern-react-with-redux.git
```

### Delete a Submodule from a Repository
Currently Git provides no standard interface to delete a submodule. To remove a submodule `mrwr-submodule` you need to:

```
$ git submodule deinit -f mrwr-submodule
$ rm -rf .git/modules/mrwr-submodule
$ git rm -f mrwr-submodule
```

### Checkout a Commit
To checkout a Git commit, you will need the commit hash.

```
$ git checkout 4aa03973d004286558465a8d86bcccfdc7b46505
$ git reset --hard
$ git checkout main
```