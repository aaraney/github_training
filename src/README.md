# Setup `rc` files 
The script `setup` will append a few helpful lines of code to your
`.bash_profile` and `.inputrc` files. Theses files are used by your
shell aka your terminal for customization. In the `alias` file in 
this directory, you will find the alias for common `git` commands that
will be added to your `.bash_profile`. After restarting your shell or
running `source ~/.bash_profile; source ~/.inputrc`, you will be able
to use new alias. The setting added to `.inputrc` will disable case
sensitive typing while using terminal. So, say goodbye to having to
backspace to capitalize the 'D' in documents when attempting to change
directories.

## To Install
run `./setup`

This will
```
cat inputrc >> ~/.inputrc
cat alias >> ~/.bash_profile
```
