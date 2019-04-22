[<<< Previous](grep.md)  
[<<< Return to introduction](README.md)

## Commands

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

Also check out [other useful commands](other-commands.md)

[<<< Return to introduction](README.md)
