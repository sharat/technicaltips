# How to setup Kdiff with git as mergetool?

Kdiff is one my favorite merge tools around. But how to set this up with git?

- Download kdiff OS X package from their website(sourceforge)
- Install the app in application folder
- Fire up your terminal

# Simple setup

- Add a symbolic link in the path `$ ln -s /Applications/kdiff3.app/Contents/MacOS/kdiff3 /usr/local/bin/kdiff3`. Note that kdiff3 is name is important because that's the name idenitified by Git as one of the supported known tools. If you're choosing a different name or not wanted to add kdiff in the path, choose the alternative method

- Enter `$ git config --global merge.tool kdiff3`

- Now simply start merging

# Manual setup
Fire up `~/.gitconfig` in your favorite editor and put the following there. (This also put KDiff as diff tool)

```
[difftool "kdiff3"]
    path = /Applications/kdiff3.app/Contents/MacOS/kdiff3
    trustExitCode = false
[difftool]
    prompt = false
[diff]
    tool = kdiff3
[mergetool "kdiff3"]
    path = /Applications/kdiff3.app/Contents/MacOS/kdiff3
    trustExitCode = false
[mergetool]
    keepBackup = false
[merge]
    tool = kdiff3
```
