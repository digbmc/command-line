# Commands

## Core commands

`pwd` - show the current (or "working") directory. Stands for "print working directory"

`ls` - show the files and folders in the working directory. I think of it as standing for "list stuff," but it's probably just short for "list."

- `ls -1` - show the files and folders in a nice vertical column.

`cd` - move to a directory, i.e. `cd Desktop` will move to the "Desktop" folder. Some special cases:

- `cd ..` - go to the directory above
- `cd ~` go to your "home" directory, i.e. /Users/<yourname>
- `cd` (by itself) also goes to the home directory
- `cd -` go to the last directory you were in before the current
- `cd ../..` travel two directories up
- `cd Documents/thesis-drafts` move two directories, from the home folder to "thesis-drafts," skipping "Documents"

`touch <filename>` - Create an empty text file named `<filename>` in your current directory.

`atom <filename>` - Open file in atom (and create it, if it does not already exist).

`mkdir <folder name>` - Create a directory named `<folder name>` in the current working directory.

`echo <some text>` - Print out any text you give it. Often used with a redirect to add text to a file.

`cat <filename>` - Print the contents of a file to the screen, in this case the contents of `<filename>`

`>` - Redirects printed output to a text file. For example `echo "this is some text" > hello.txt` would put "this is some text" in a file called hello.txt

`>>` - Redirect and append. If there's already a file with text in it, this command will add that text to the file without destroying and recreating it.

`|` - Pipe symbol. Takes output from one command and uses it as input for another command.

`less <filename>` - Print out the contents of a file in a paginated form. Use `<Control-v>` and `<Alt-v>` (or `<Command-v` and `<Option-v>`) to move up and down. Press `q` to quit.

`head <filename>` - Print the first section of a file (first 10 lines or other specified quantity)

`tail <filename>` - Print the last section of a file (last 10 lines or other specified quantity)

`wc -l` - Takes input and returns the number of lines in that input, as in `cat <filename> | wc -l`

`sort` - Arrange lines in a file in numeric and alphabetical order.

`uniq` - Remove duplicate lines from input, as in `cat <filename> | uniq`. To show the duplicate files, use `uniq -d`. Often most useful after using `sort`, since it only removed duplicates that are next to one another.

`mv` - Move or rename a file. For example, `mv file1 file2` will rename `file` to `file2`. You can also specify another destination, so that `mv file1 ~` will move file1 to the home folder without renaming it.

`rm <filename>` - Permanently remove a file from your computer.

`clear` - Clears our terminal window of the command history (you can also type `Control` + `l`).

`grep -i <text>` - Searches text and prints any line that matches a specified pattern (here "text"). "Grep" stands for "global regular expressions."

`rev` - Reverses the text you give it, i.e. `echo "Hello there" | rev`


## Other useful commands

`<tab>` - The `<tab>` key on your keyboard will complete names of commands and files. Start typing a filename and hit tab twice to see all possible acceptable completions. If there is only one possibility, the rest of the name will be filled in for you.

`<up>` - The `<up>` key will fill in the last command you ran. Hit it multiple times to cycle through the last commands you've entered.

`man <command name>` - The `man` or manual command will provide information on any UNIX command. Try `man ls`, `man grep`, or `man man`.

`exit` - Exit the terminal session. You can also use `<Control-d>`

`sudo` - Run before a command to run it as an administrator. You will need to enter your password, and note that no asterisks or special characters will appear as you type. 

`su` - Become the root user of the system. Your `$` prompt will change to a `#` prompt.

`!!` - Run the last command. To run the last command you entered with administrative privileges, use `sudo !!`

`*` - refer to all files and folders in a directory, i.e., `cat *.txt`

`clear` or `<Control-l>` - Clear the terminal window.

`which` - Show where a command is stored on your system, i.e. `which python`

`history` - See the previous commands you've entered in the terminal. Useful in conjunction with `grep`

`cp` - Copy a file. `cp file1 file2` will make a copy of `file1` named `file2`. Can be used with the `-r` flag to copy whole folders.

`rm` - This command can be dangerous, so use it carefully. Removes a file or files. If used with the wrong flags or in the wrong place, you can delete a lot of important files, so be careful with this one.

`rmdir` - Remove an empty directory.

`.` and `..` - `.` Refers to the folder you're in, while `..` refers to the folder above.

`.hello.txt` - Any file with a `.` in front of its name is a hidden file. You won't see it in `ls` or in the GUI. To reveal hidden files, use `ls -A`

`ping` - Use `ping google.com` to see if your internet is working.

`df -hl` - Tells you how much hard drive space you have left.

`top` - Monitor which processes are using up your memory

`kill` and `killall` - Kill a particular process or kill a category of processes by name. Try `killall chrome` or `killall firefox`

`sudo shutdown -r` - Reboot the computer. `shutdown -h` turns off the computer. 

`time` - Use before a command to find out how long that command takes to run.

`uptime` - Tells how long your computer has been on.

### Not particularly useful commands

`cal` - Show a calendar.

`telnet towel.blinkenlights.nl` - Watch Star Wars in the terminal. Because.

`say "Hello there"` - Have your computer talk to you. (Use `espeak` on Linux.)

Find so much more on the command line:

[Bash manual](https://www.gnu.org/software/bash/manual/bashref.html) - the no nonsense text descriptions of bash commands.  
[explain shell](https://explainshell.com/) - a site that explains commands you paste into the form. This site is fantastic for breaking down commands you find in the wild on the internet.  
[Easy shell guide](https://lucasviola.github.io/easyshell/) - a friendly, styled (pastel!) list of common commands you might want to try out.
