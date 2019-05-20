# dotfiles

Ideas, commands taken from:

https://www.atlassian.com/git/tutorials/dotfiles

and

https://news.ycombinator.com/item?id=11071754
    
   
    git init --bare $HOME/.cfg
    alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
    config config --local status.showUntrackedFiles no
    echo "alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'" >> $HOME/.bashrc
    
    
    alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
    echo ".config" >> .gitignore
    git clone --bare <git-repo-url> $HOME/.cfg
    alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
    config checkout
    config config --local status.showUntrackedFiles no
    
