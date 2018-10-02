# For \*nix User

- Install VIM, git, subversion

    Ubuntu

    ```
    sudo apt-get install vim vim-gtk3 subversion
    ```

    Mac

    ```
    brew install vim macvim subversion
    ```


- Configuration

    - vimrc

        ```
        svn checkout github.com/ikey4u/q/trunk/qvim/ ~/.vim/
        ```

    - font

        ```
        git clone --depth 1 --branch release https://github.com/adobe-fonts/source-code-pro.git ~/.fonts/adobe-fonts/source-code-pro
        fc-cache -f -v ~/.fonts/adobe-fonts/source-code-pro
        ```


# For Windows User

- Download gvim directly from [here](https://ftp.nluug.nl/pub/vim/pc/gvim81.exe).
Then install it with `Full` mode, keep others as origin is fine.

- Install svn from [here](https://tortoisesvn.net/downloads.html) with
command line enabled.

- Configuration

    ```
    svn checkout github.com/ikey4u/q/trunk/qvim/ %USERPROFILE%\vimfiles
    ```
