# remote-vimrc

This following line can be executed in your command-line inside Vim. It downloads the content of the vimrc in the `a` register and sources it.
Useful on servers where you cannot or don't want to store a vimrc file.

```sh
let @a = system('curl -s https://raw.githubusercontent.com/justijndepover/remote-vimrc/refs/heads/master/.vimrc') | execute @a | echo 'Configuration loaded'
```
