# dotfiles

[Mac OS, csh, Bash]

### Install Homebrew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

#### 安装VIM, TMUX, GIT, ZSH, CURL
`$ sudo apt install vim tmux git zsh curl` 
#### 安装 OH-MY-ZSH
`$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
#### 切换到ZSH
1. 运行如下命令，看看自己终端SHELL环境。
`$ echo $SHELL`
`/bin/zsh`
2. 如果还没有自动进入ZSH的环境, 运行命令。
`$ sudo chsh -s /bin/zsh`
3. 重新启动终端，如果仍然没有改变，则需要用户重新登录。
#### 安装DOTFILES
1. 从如下GIT仓库中克隆到用户根目录下
`$ cd & git clone https://github.com/xuzewei/dotfiles.git & cd dotfiles`
2. 执行SHELL
`$ sh .make.sh`
#### 安装VIM插件包undle
1. 从如下GIT仓库中克隆到OH-MY-ZSH的插件目录下。
`$ cd & git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim`
2. 打开VIM配置文件
`$ vim ~/.vimrc`
`: PluginInstall`
3. 如下图示参考
![Alt text](./Screenshot from 2018-07-05 17-21-28.png)
`:q` or `:q!`：退出VIM
7. 安装ZSH环境下命令行自动完成功能
从如下GIT仓库中克隆到OH-MY-ZSH的插件目录下。
`$ git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`
配置ZSH启动环境
`$ vim ~/.zshrc`
添加插件名称到插件列表中
`plugins=(zsh-autosuggestions)`
如下图示参考：
![Alt text](./Screenshot from 2018-07-06 08-37-41.png)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTk2MTM5MjY5LC0xNjkzMjEwNTk3LDIwNT
EzNzk1NTldfQ==
-->