# Bash Basics

Bash is an incredibly powerfull tool that will increase your productivity. It might take an investment on your part, but it's well worth it. This guide is by no means exhaustive, it only shows you the basics.

### Starting Up a Terminal

Assuming your on linux, go ahead and launch a new terminal session. This is starting what is called an _interactive_ shell. Both its standard `input` and `output` are connected to the terminal you just launched. Standard `input` or `stdin` is the source of input data for command line programs. Standard `output` on the other hand is the data that is the result of a command.

When you frist startup a terminal, your `~/.bashrc` file is executed. Go ahead and modify your `~/.bashrc` file so it looks like the following:

```
echo "Hello world!"
```

Now start up a new terminal. You should see `Hello world!` in the terminal.

### Navigating the File System

##### Listing Files
Lets look at the `ls` command. This simply lists all the files in your current directory. When you start up a new terminal it will put you in your user's home directory. If you run `ls -a` it will also list files that start with a `.`.

##### Changing Directories
The `cd` command will change your current directory. `cd ~/` will take you back to home directory, `cd ..` will take you up one directory, and `cd -` will take you back to the previous working directory. Simply run `cd` _directory_ to step into a directory

### Shortcuts
Typing commands and filepaths can be cumbersome, so let's learn some keyboard shortcuts to help us be more proficient.

Use `tab` to autocomplete commands and arguments. Especially useful when trying to type out file paths.

The `up` and `down` arrows will cycle through previous commands. You can also run `history` to see all you recent commands.

`ctrl+U` will clear the entire line.

`ctrl+K` will delete all characters on the line following the cursor.

`ctrl+R` will search your command history. Just start typing to search for previous commands that match your search term.

### Editing Files
Sometimes you need a quick way to edit a file from the command line. The easiest way to do this is by learning a command line editor. `vim` is extremly popular, but can be frustrating for new users. Lets look at some `vim` basics:

When you first enter `vim` you will be in _normal_ mode. You can't edit any text at this point. You need to be in _insert_ mode. Simply type `i` to enter into _insert_ mode. Now you can edit text. To get out of insert mode hit the `esc` key.

Navigating `vim` can be awkward at first. You need to be in _normal_ mode to navigate through text. You can either use the arrow keys or `h` `j` `k` `l`. Once you get used to using the letters, it's extremely efficient.

To exit `vim` you **need** to be in _normal_ mode. Type `:wq` to save the file and exit `vim`. You can use `:q!` to exit without saving. `:w` will save file, but will keep you inside `vim`.

If you want a more in-depth tutorial run `vimtutor` on the command line.
