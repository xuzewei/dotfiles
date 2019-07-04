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

#### Install DOTFILES

    $ cd & git clone https://github.com/xuzewei/dotfiles.git & cd dotfiles
    $ sh .make

#### Install VIM Plugin (option)

    $ cd & git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
    $ vim ~/.vimrc
    
*notes: switch to command line(use esc key), input ':PluginInstall'* 

#### Install ZSH Plugin (option)

    $ git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
