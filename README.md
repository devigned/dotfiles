# dotfiles
dotfiles that help me get stuff done

## Consumption
1) Clone to your home directory.
    ```
    cd ~
    git clone https://github.com/devigned/dotfiles .dotfiles
    ```
2) Source init in your `.bash_profile`
    ```
    echo "[ -f ~/.dotfiles/init ] && source ~/.dotfiles/init" >> .profile
    ```
    You may also need to source your `.bash_profile` elsewhere, like in `.bashrc`.
3) Add an include in your `.gitconfig`
    ```
    cat >> .gitconfig <<EOF
    [include]
        path = ~/.dotfiles/git
    EOF
    ```
### Extension
If you would like to add some sensitive stuff that will be git ignored, the `.gitconfig` will try to include
`.git_extras` by default, and `init` will try to include `extras` by default.

## Make it your own
Fork it and make it your own. 