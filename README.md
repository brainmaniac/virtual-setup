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
   
 * Add this to gitconfig
   - `cleanup = branch --merged | rg -v master | xargs git branch -d` 

* I VScode:
   ### User settings (JSON)
   ```
   {
      "workbench.colorTheme": "Field Lights",
      "workbench.statusBar.visible": true,
      "explorer.openEditors.visible": 0,
      "workbench.activityBar.visible": false,
      "editor.minimap.enabled": false,
      "workbench.editor.showTabs": false,
      "git.enableSmartCommit": true,
      "javascript.updateImportsOnFileMove.enabled": "always",
      "files.trimTrailingWhitespace": true,
      "workbench.sideBar.location": "left",
      "explorer.confirmDelete": false,
      "editor.inlineSuggest.enabled": true,
      "[python]": {
        "editor.formatOnType": true
      },
      "window.zoomLevel": 2
   }
   ```
   
   ### Keybindings.json
   ```
   // Place your key bindings in this file to override the defaultsauto[]
   [
       {
           "key": "shift+cmd+g",
           "command": "workbench.view.scm"
       },
       {
           "key": "ctrl+shift+g",
           "command": "-workbench.view.scm"
       },
       {
           "key": "ctrl+cmd+u",
           "command": "git.pull"
       },
       {
           "key": "ctrl+cmd+p",
           "command": "git.push"
       },
       {
           "key": "ctrl+up",
           "command": "spaceBlockJumper.moveUp"
       },
       {
           "key": "ctrl+down",
           "command": "spaceBlockJumper.moveDown"
       }
   ]

   ```
   
   
   ### Extensions:
   ```
   code --install-extension AkankshaSingh872.case-change
   code --install-extension amiralizadeh9480.laravel-extra-intellisense
   code --install-extension bmewburn.vscode-intelephense-client
   code --install-extension bradgashler.htmltagwrap
   code --install-extension bradlc.vscode-tailwindcss
   code --install-extension dansysanalyst.pest-snippets
   code --install-extension dbaeumer.vscode-eslint
   code --install-extension eamodio.gitlens
   code --install-extension esbenp.prettier-vscode
   code --install-extension felixfbecker.php-intellisense
   code --install-extension GitHub.copilot
   code --install-extension jmfirth.vsc-space-block-jumper
   code --install-extension m1guelpf.better-pest
   code --install-extension mikestead.dotenv
   code --install-extension ms-azuretools.vscode-docker
   code --install-extension ms-python.isort
   code --install-extension ms-python.python
   code --install-extension ms-python.vscode-pylance
   code --install-extension ms-toolsai.jupyter
   code --install-extension ms-toolsai.jupyter-keymap
   code --install-extension ms-toolsai.jupyter-renderers
   code --install-extension ms-toolsai.vscode-jupyter-cell-tags
   code --install-extension ms-toolsai.vscode-jupyter-slideshow
   code --install-extension ms-vscode-remote.remote-containers
   code --install-extension ms-vscode-remote.remote-ssh
   code --install-extension ms-vscode-remote.remote-ssh-edit
   code --install-extension ms-vscode.remote-explorer
   code --install-extension ms-vsliveshare.vsliveshare
   code --install-extension msjsdiag.vscode-react-native
   code --install-extension octref.vetur
   code --install-extension patbenatar.advanced-new-file
   code --install-extension Prisma.prisma
   code --install-extension rcore.rcore-unused-css-classes
   code --install-extension rebornix.ruby
   code --install-extension ryannaddy.laravel-artisan
   code --install-extension sashaweiss.bracket-jumper
   code --install-extension sleistner.vscode-fileutils
   code --install-extension smlombardi.slime
   code --install-extension streetsidesoftware.code-spell-checker
   code --install-extension sveggiani.vscode-field-lights
   code --install-extension unifiedjs.vscode-mdx
   code --install-extension viktorzetterstrom.non-breaking-space-highlighter
   code --install-extension vscodevim.vim
   code --install-extension waderyan.gitblame
   code --install-extension wingrunr21.vscode-ruby
   ```
