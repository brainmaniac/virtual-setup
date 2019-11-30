* Download iTerm 2

* Make sure you have zsh installed

* Install *Oh My zsh*
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

* Run `git config --global pager.branch false` to remove strange default paging of git output

* Go to ~/.zshrc

   - Add this line `alias setalias="vim ~/.zshrc && source ~/.zshrc"`
  
   - This will allow you to anywhere in the terminal type *setalias* and you will be able to create new aliases
   
   - Additional suggested aliases can be found in the file **aliases.txt** in this repo
   
 
