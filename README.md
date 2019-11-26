# vim-tmux-configuration
Backup configuration files for vim and tmux

Configuration
-------------

1. Download:

```bash
git clone https://github.com/Hao-Xu/vim-tmux-configuration.git
cp vim-tmux-configuration/.vimrc ~/
cp vim-tmux-configuration/.tmux.conf ~/
```


2. Set up vim:

Set up [Vundle] and [pathogen]:

```bash
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/vundle
mkdir -p ~/.vim/autoload ~/.vim/bundle && \
curl -LSso ~/.vim/autoload/pathogen.vim https://tpo.pe/pathogen.vim
```

```vim
:PluginInstall
```

3. Configure YouCompleteMe:

```bash
cd ~/.vim/bundle/YouCompleteMe
git submodule update --init --recursive
sudo apt install build-essential cmake python-dev
python install.py
```

4. Install Ctags:

```bash
sudo apt install ctags
Ctags -R
```
