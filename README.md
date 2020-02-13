# dotfiles

Ideas, commands taken from:

- https://www.atlassian.com/git/tutorials/dotfiles
- https://news.ycombinator.com/item?id=11071754
- https://github.com/Siilwyn/my-dotfiles/tree/master/.my-dotfiles
    
   
    
alias config='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'

echo ".dotfiles" >> .gitignore

git clone --bare <git-repo-url> $HOME/.dotfiles

config checkout

config config --local status.showUntrackedFiles no
    
