# dotfiles

Ideas, commands taken from:

- https://www.atlassian.com/git/tutorials/dotfiles
- https://news.ycombinator.com/item?id=11071754
- https://github.com/Siilwyn/my-dotfiles/tree/master/.my-dotfiles
    
   
    git init --bare $HOME/.cfg
    alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
    config config --local status.showUntrackedFiles no
    echo "alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'" >> $HOME/.bashrc
    
    
    alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
    echo ".dotfiles" >> .gitignore
    git clone --bare <git-repo-url> $HOME/.dotfiles
    alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
    config checkout
    config config --local status.showUntrackedFiles no
    
