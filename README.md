# dotfiles for zsh

[Mac OS/Ubuntu]

### Install Homebrew (Mac OS)

    $ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    $ sudo brew vim tmux git zsh curl

#### Install VIM, TMUX, GIT, ZSH, CURL (Ubuntu)

    $ sudo apt install vim tmux git zsh curl

#### Install OH-MY-ZSH
    
    (option) $ sudo vi /etc/hosts (Append a line: 199.232.28.133 raw.githubusercontent.com)
    $ sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

#### Switch to ZSH shell

    $ sudo chsh -s /bin/zsh
    $ echo $SHELL

*notes: If use command 'echo $SHELL' without '/bin/zsh' then must be restart shell env.*

#### Install DOTFILES

    $ cd & git clone https://github.com/xuzewei/dotfiles.git & cd dotfiles
    $ sh .make.sh

#### Install VIM Plugin (option)

    $ cd & git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
    $ vim ~/.vimrc
    
*notes: switch to command line(use esc key), input ':PluginInstall'* 

#### Install ZSH Plugin (option)

    $ git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
