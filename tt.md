# Tips & tricks <!-- omit in toc -->

Here you can find solutions, workarounds and tips about Linux, Software Development, Vim and other topics that I deal with on a daily basis.

- [Shared clipboard on vim](#shared-clipboard-on-vim)

## Shared clipboard on vim

I like to give Vim the access to the main system clipboard, so I can copy/paste from/to it without messing with the registers `*` and `+`. Simply add in the `.vimrc` file the following line:

    set clipboard^=unnamed,unnamedplus

With this command, by default, each copy/paste will go directly in the registers `*` and `+`, so the content will be accessible outside Vim and vice versa.

If you are interested in other Vim configurations, checkout my repo [dotfiles](https://github.com/ceccoemi/dotfiles) on GitHub.