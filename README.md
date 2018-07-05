# dotfiles
@[Manual, Markdown]

1. 安装Vim, Tmux, Git, Zsh开发环境
`$ sudo apt install vim tmux git zsh` 
2. 安装 `oh-my-zsh` 
`$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
[oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
退出终端，打开终端，如果还没有自动进入`zsh`的环境, 运行命令
`$ sudo chsh -s /bin/zsh`
3. 下载`dotfiels`
`$ cd`
`$ git clone https://github.com/xuzewei/dotfiles.git`
4. 执行`.make.sh`
`$ sh .make.sh`
5. VIM安装插件包undle
`$ git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim`
