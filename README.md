# dotfiles

[Ubuntu/Ubuntu with Win10 subsystem]

#### Install VIM, TMUX, GIT, ZSH, CURL

    $ sudo apt install vim tmux git zsh curl

#### Install OH-MY-ZSH

    $ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

#### Switch to ZSH shell

    $ sudo chsh -s /bin/zsh
    $ echo $SHELL

*notes: If use command 'echo $SHELL' without '/bin/zsh' then must be restart shell env.*

#### 安装DOTFILES
从如下GIT仓库中克隆到用户根目录下
`$ cd & git clone https://github.com/xuzewei/dotfiles.git & cd dotfiles`

执行SHELL
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
eyJoaXN0b3J5IjpbLTE5MDMwOTAxMjQsLTExMDQyMTMzMDMsND
c0NDUwMjM0XX0=
-->