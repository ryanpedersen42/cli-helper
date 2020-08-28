### Basics

Good writeup: [https://www.codecademy.com/articles/command-line-commands](https://www.codecademy.com/articles/command-line-commands)

```jsx
//ls lists files in directory
ls

//list all files including hidden
ls -a

// show latest mod file or dir date as last (more detail, reverse order)
ls -ltr

//tail displays the last part of a file
tail <file name>

//choose how many lines of the file you want to display
tail -n <number> <file name>

//cat concatenates and prints files
cat <file name>

//ps is process status
ps

//https://www.gnu.org/software/grep/manual/grep.html
//to test regex: https://regex101.com/
//grep is (globally search a regular expression and print)
//-i is case insensitive
//-r is recursive, so look through all subdirectories and files
// /* is everything after the main /
grep -ri "Hello World!" /*

//adding q will instruct it to run in quiet mode, returning 0 if there is a match
grep -qri "Hello World" <file / dir>

//return only the matched (non-empty) parts of matching lines, each part of response takes up a line
grep -o "Hello" <file / dir>

//For even more legibility, use ps and pipe it to grep.
ps <something> | grep <something>

//a: Show processes for all users
//u: Display the user who is using the process
//x: Show all processes. (Without this, ps won’t show processes running in a GUI environment.)
ps aux | grep i <something>

//top displays and updates sorted process information.
top
```

```jsx
//netstat shows the network status. This command shows network ports in use and their incoming connections
netstat

//To retrieve more detailed information about which files use the disk space in a directory
//-h makes human readable, -s is total size
du
du -s * | sort -nr // sort by number, reverse order

//lsof lists the open files associated with the application
lsof

//chmod can correct the permissions to enable your user to run the binary.
chmod

//kill
kill
```

```jsx
http://www.linfo.org/redirection.html

> takes the standard output of the command on the left and redirects it to the file on the right.
>> takes the standard output of the command on the left and appends (adds) it to the file on the right.

| is a “pipe”. The | takes the standard output of the command on the left, and pipes it as standard input to the command on the right. You can think of this as “command to command” redirection.
```

```jsx
//open up vim 
//esc after input, then :wq for write and quit (saving and quitting)
vi <file name>
```

```jsx
//opens bashrc
open ~./bashrc
open ~./bash_profile // mac
```

