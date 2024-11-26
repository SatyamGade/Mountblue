# cat

**Description**
 - Displays the contents of a file.
 - Concatenates files.
 - Creates new files.

**Important Flags**
 - -n to Display file with line numbers

**Q&A**
- Display content of a file.
  
  > cat demo.txt
- Merge two files to other file.
  
  > cat first.txt second.txt > merged.txt
- Create new file.
  
  > cat > new.txt
   - note: type content and press Ctrl+D to save that content to newly created file




# touch

**Description**
 - Creates empty files.
 - Updates the timestamp of existing files.
   
**Important Flags**
 - -a to Update access time only.
 - -m to Update modification time only.

**Q&A**
 - Create a file.

   > touch file.txt
 - Create multiple files.

   > touch a.txt b.txt c.txt
 - Update only modification time.

   > touch -m file.txt




# grep

**Description**
 - Searches for a specified pattern in a file or stream.

**Important Flags**
 - -i to Case-insensitive search.
 - -n to Show line numbers with matches.
 - -c to Count the number of matching lines.
 - -r to Search recursively in directories.

**Q&A**
 - Search for a word in a file.
 
  '''
  grep "Word" file.txt
  grep -i "Word" file.txt   ( _case insesitive search_ )
  '''
 - Search recursively in a directory.

   > grep -r "word" /path/to/dir




# wc

**Description**
 - Counts lines, words, bytes or characters in a file.

**Important Flags**
 - -l to Count lines.
 - -w to Count words.
 - -c to Count bytes.
 - -m to Count characters.

**Q&A**
 - Count lines of a file.

   > wc -l file.txt
 - Count words of a file.

   > wc -w file.txt
 - Display all counts of a file.

   > wc file.txt




# tail

**Description**
 - 
head
more
less
uniq
