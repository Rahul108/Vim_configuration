# Introduction
I will specify my vim configuration steps here...

# Steps
* Installing Vim (On ubuntu 18.04)
```sh
$ sudo apt-get update
$ sudo apt-get install vim
```
* Opening Vim
```sh 
$ vim
```
* Configuring [**The NERD tree : A tree explorer plugin for navigating the filesystem**](https://www.vim.org/scripts/script.php?script_id=1658) 
```sh
$ git clone https://github.com/scrooloose/nerdtree.git ~/.vim/pack/vendor/start/nerdtree
$ vim -u NONE -c "helptags ~/.vim/pack/vendor/start/nerdtree/doc" -c q
# For Pathogen
$ git clone https://github.com/Xuyuanp/nerdtree-git-plugin.git ~/.vim/bundle/nerdtree-git-plugin
```

* To run this on vim startup, on .vimrc
```sh
# If .vimrc not availabe create a file named .vimrc
$ vim .vimrc
# then cpoy paste the following line and save
autocmd vimenter * NERDTree
```
