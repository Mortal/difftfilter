# difftastic in git add -p

Setup:

```sh
mkdir -p ~/.local/lib &&
git clone https://github.com/Mortal/difftfilter ~/.local/lib/difftfilter &&
ln -s ../lib/difftfilter/difftfilter ~/.local/bin/difftfilter
```

Test it out: `git -c interactive.difffilter=$HOME/.local/bin/difftfilter add -p`

Use permanently: `git config interactive.difffilter $HOME/.local/bin/difftfilter`

Uninstall: `git config interactive.difffilter "" && rm -rf ~/.local/lib/difftfilter ~/.local/bin/difftfilter`
