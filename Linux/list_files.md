# Understanding the `ls` Command

The `ls` command allows us to list the content of the directory.

## Usage


`ls`

list Without color

`ls --color=no`

list With color

`ls --color=yes`

for auto

`ls --color=auto`


### How to get more details

For clearing screen

`clear`

### Arguments

-> one dash informs the system that we will pass one letter argument, like 'l'
-> -- two dashes means that argument will contain more than one letter

`ls -l`
l means long listing format.

`ls -n` command. This works like `ls -l`, but it changes the user-friendly names to UIDs and GIDs.

### Sorting

Obviously, all lists can be sorted. There is no exception here.

Linux allows us to list files using multiple sorting options. ls command has some options built-in. First type of sort we already observed. By default ls sorts the files alphabetically. Let's try something else

different timestamps in linux
- atime - The last time when file was accessed.
- mtime - last modification time. By modification we mean change in the file content.
- ctime - last metadata modification time. We mean here - permissions change, location of the file, etc.

  Now first sorting option will be -t. This argument sorts files with the last modification time, newest files come first.

Let's try.

`ls -lt`

We use two arguments, to observe things better. We can specify exactly the modification time by adding u to the argument list. But please remember, in order to print this information properly you have to use t with another argument (u in this case).

`ls -ltu`

Ok, now let's print the list and order it by ctime - metadata change.

`ls -ltc`

Basically these are all sorting commands, we have to play with them as per requirements


### Sort content by size

`ls -s`

This shows the short list of files and allocated space. As we already know, we can combine this argument - s - with others. Let's do it.

`ls -ls`




