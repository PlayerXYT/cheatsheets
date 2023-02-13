# rc Configuration Cheatsheet

rcs (or more boradly) dotfiles are config files that can be exported and imported to any linux running the compatible app.

## Basic usage

rc files are app-specific but they generally follow the following format:

`~/.[app name]rc`

You'll notice that the name of the file starts with ".", in Unix-based operating systems, "." denotes a hidden file.

Open the file with your favourtie text editor, a common (and default one) being nano or vim. The file is commonly a list of commands to execute on startup.

## Examples

By default most modern linux distros come with the "bash" shell, here is an example of a simple ".bashrc":

```sh
alias ls="ls -A"
alias l="ls -lA"

run_something() {
	cd ~
	ls
}

neofetch
```

The `alias ls="ls -A"` command sets a non-recursive alias so running the `ls` command will actually execute `ls -A`

Similarly `alias l="ls -lA"` will replace `l` with `ls -lA`

Next a function is defined called `run_something` which will go to the user's home directory and run `ls`

Finally `neofetch` will just call the neofetch command, a popular app for displaying system information with ascii art.

## Notes

Dotfiles may not show up in your home directory, in that case the second most common place is `~/.config/[app name]`, for example i3 will be located in `~/.config/i3/config`, neovim will be located in `~/.config/nvim/init.lua` and so on.

If none of these locations are right then review the app's documentation for this information, for example ssh is located in `/etc/ssh/sshd_config` because the config is applied system-wide.
