# man Command Cheatsheet

man is an app that comes default with most versions on linux and BSD, it is a command that shows the **man**ual of a specified command

## Basic usage

The basic usage of the `man` command is as follows:

```sh
man [command]
```

- `[command]`: The command to view

## Common Options

Here are some of the most commonly used options for the `man` command:

- `-c`: Print to console instead of using less

## Examples

- `man ls`: Displays the manual of the `ls` command

- `man -c cd`: Displays the manual of the `cd` command and prints to stdout

- `man -c pwd | grep "-P"`: Prints the manual of the `pwd` command and asks grep to search for "-P"
