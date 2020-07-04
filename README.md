* Download iTerm 2

* In iTerm 2 go to `iTerm2 > Preferences > Profiles > Terminal` and check `Unlimited Scrollback`

* Make sure you have zsh installed

* Install *Oh My zsh*
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

* Run `git config --global pager.branch false` to remove strange default paging of git output

* Go to ~/.zshrc

   - Add this line `alias setalias="vim ~/.zshrc && source ~/.zshrc"`
  
   - This will allow you to anywhere in the terminal type *setalias* and you will be able to create new aliases
   
   - Additional suggested aliases can be found in the file **aliases.txt** in this repo

* Auto suggestions for zsh 
   https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md
   I did the Git clone install
   
* Fuzzy find for terminal history
   https://github.com/junegunn/fzf#installation

   - `brew install fzf`

   - `$(brew --prefix)/opt/fzf/install`
   
   - Use ctrl + r to use it when in terminal
   
 
