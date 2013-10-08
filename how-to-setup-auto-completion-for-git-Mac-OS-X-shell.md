

`curl https://raw.github.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash`

Then add it to my ~/.bash_profile file the following 'execute if it exists' code:

```
if [ -f ~/.git-completion.bash ]; then
  . ~/.git-completion.bash
fi
```
