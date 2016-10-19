Setup
-----
Clone repository in your home directory (~/VimConfiguration should be created).

Execute following lines

```bash
$> ln -s ~/VimConfiguration/.vim ~
$> ln -s ~/VimConfiguration/.vimrc ~
$> ln -s ~/VimConfiguration/.vimrc_custom ~
$> ln -s ~/VimConfiguration/.gvimrc ~
```

Now it's time to update submodules:
```bash
$> cd VimConfiguration
$> git pull
$> git submodule init
$> git submodule update
$> cd ~/VimConfiguration/.vim/bundle/neobundle.vim
$> git checkout master
```

Now open vim.
It will ask you to install plugins.
However for some reason it sometimes doesn't work.
You can install missing plugins by calling
```bash
:NeoBundleUpdate
```
from vim.
