# manifest xml files

this repository contains manifest xml files for different projects

# prerequisite

* python2.7+
* git
* [google repo command](https://source.android.com/setup/develop/repo)
* a native or virtual machine running Ubuntu (I didn't figure out how to use repo init in woindows 10 command shell)
* [allow symlink in windows 10](https://superuser.com/questions/104845/permission-to-make-symbolic-links-in-windows-7). Because repo is a native tool in linux and creates symlinks during exectuing operation, you have to enable symlinks in windows otherwisw repo commands fail.

# Fetching all repositories regarding a project

1. open a shell in Ubuntu and create a folder that acts the root folder of all projects you are about to fetching
2. enter the folder you just created and initialize repo configure by the command
```
repo init -u git@github.com:deantonccns/manifest -m kasa.xml
```
3. download all repositories
```
repo sync
```
4. please be minded that all repositories are in headless status, you need to checkout to master branch when you start to work on ertain projects
