# cd Command Cheatsheet

cd is a command in Unix-line and DOS operating systems that is used to go to a specified directory

## Basic Usage

The basic usage of the `cd` command is as follows:

```sh
cd [path]
```

- `[path]`: The path of the directory to go to

## Shortcuts (Universal)

`.` is used to go to the same directory

- `cd ./foo` is the same as `cd foo`

`..` is used to go to the last directory

- In the foo directory `cd ../foo/bar` is the same as `cd bar`

## Shortcuts (Unix)

`/` is used to go to the root directory

- `cd /etc` will go to "/etc" no matter what directory you are in

`~`, `$HOME` is used to go to the home directory

- As the user foo `cd ~` is the same as `cd /home/foo` and  `cd $HOME`

- As root `cd ~` is the same as `cd /root` and `cd $HOME`

## Shortcuts (DOS)

`[drive-name]:` is used to go to the selected drive

- `D:` will switch to the root directory in the D drive
