# Dev Tools runs as root
```
xcode-select --install
```
OR 
Command Line Tools for Xcode
via: https://developer.apple.com/downloads/index.action
Direct link: https://download.developer.apple.com/Developer_Tools/Command_Line_Tools_for_Xcode_12.3/Command_Line_Tools_for_Xcode_12.3.dmg 

## new terminal runs as user
    ```
    mkdir src work
    scp -r <host>:~/.dotfiles .
    ./.dotfiles/bin/makesym 
    ```
# Install homebrew
    ```
    curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh > install.sh 
    ## VERIFY CONTENT and check MD5
    chmod +x install.sh 
    ./install.sh
    ```
## brew apps
    ```
    apps="awscli bash cowsay curl fortune gdbm gettext git go jq libevent libzip ncurses oniguruma openssl@1.1 pcre2 python@3.8 readline sublime-text sqlite tldr tmux utf8proc vcprompt vim xz"

    for app in $apps; do
        brew install ${app}
    done
    ```
## brew cask 
    ```
    brew install --cask alfred
    brew install --cask dropbox
    brew install --cask iterm2
    brew install --cask spectacle
    brew install --cask firefox
    brew install --cask visual-studio-code
    ```
## brew tap fonts 
    ```
    brew tap homebrew/cask-fonts
    brew install --cask font-jetbrains-mono font-source-sans-pro font-source-code-pro font-fira-code 
    ``` 

## Configure iterm2 
    Ctrl+,
    - Apperances -> General Tab -> Theme -> Minimal
    - Code Font: Fira Code
    - Dark Mode
## Configure Finder -> Alfred
    - SysPref -> finder -> spotlight -> uncheck 
# Misc 
   ```
   open -a "Firefox" --args --make-default-browser
   ```
