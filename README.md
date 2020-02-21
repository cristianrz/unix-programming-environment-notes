# "The Unix Programming Environment" notes

## Commands

* ctrl + u deletes the current line
* ctrl + d closes the terminal if there is nothing written
* `p` is like the old `more`
* `pr` prints as if it was a book
* `tail -1` does the same as `tail -n 1`
* `tail +3` prints file starting from line 3
* `cmp` finds the first that differs
* `rmdir` will only remove an empty directory
* `grep < file` does what `cat file | grep` does
* `nohup` does what ctrl+z would do
* `nice` does the same as `nohup` but, for expensive commands, is nicer to other users
* `at 3am < script` runs the script at that time
* You can write to other tty's with `date > /dev/tty0`
* `crypt` encrypts stdin to stdout
* `<< str` pass stdin until `str` is found on a line by itself

## Mail

* `mail` is quite useful for reminders
* `write` works like a chat, quite cool

## Regexp

* `[a-z]` one char from a to z
* `?` any single char

## Concepts

* "If no filenames are specified, the standard input is processed.
* If a directory has execute permissions but not the others, you can only open contents if you know the name.
* Files know when they were last modified, when they were last read or executed and when the inode was updated (e.g. to change permissions)
* Inside directories there are links to inodes (rather than inodes)
* `ln` creates a new link for the same inodec
* It is common for some commands that if they are called without arguments, they show their internal lists.

## Others

* `/etc/motd` contains the login message of the day
* `PS2` contains the prompt on the second line, e.g. after `command \`
