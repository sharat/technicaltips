# How to change your default X-Code version?

Once you install the beta version of X-Code, you will have change the default X-Code version for many reasons to run two versions side by side. Even after unistall, you will find lot of things got screwed up like opening certain utilities like `opendiff`

I faced the following issue when I tried to start `opendiff`

```
xcrun: Error: could not stat active Xcode path '/Applications/Xcode5-DP.app/Contents/Developer'. (No such file or directory)
```

It's quite easy to fix this with the help of `xcode-select` utility

`sudo xcode-select /Applications/XCode.app`

Now you open your favorite tool packaged with it.
