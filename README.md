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
   - note: type content and press enter and then press Ctrl+D to save that content to newly created file




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

   > grep "Word" file.txt
   
   > grep -i "Word" file.txt   ( _case insesitive search_ )
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
 - Displays the last lines of a file. (last 10 by default)

**Important Flags**
 - -n N to Show the last N lines.

**Q&A**
 - Display the last 5 lines of a file.

   > tail -n 5 file.txt




# head

**Description**
 - Displays the first lines of a file. (first 10 by default)

**Important Flags**
 - -n N to Show the first N lines.

**Q&A**
 - Display the first 5 lines of a file.

   > head -n 5 file.txt




# more

**Description**
 - Displays file contents one screen at a time.

**Important Flags**
 - -d to Show a message in the terminal for quit or continue.
 - -c to Clear the screen before showing new content.

**Q&A**
 - Paginate a file.

   > more file.txt
 - Show content of a file one screen at a time with messages for quit or continue.

   > more -d file.txt




# less

**Description**
 - Displays file content, allowing navigation (backward and forward).

**Important Flags**
 - -N to Show line numbers.

**Q&A**
 - Navigate a file.

   > less file.txt

   > less -N file.txt  (_navigate a file with line numbers_)

    - note: For searching a word interactively press / and type the word and navigate the file.




# uniq

**Description**
 - Removes duplicate lines in sorted input.

**Important Flags**
 - -c to Prefix lines with the number of occurrences.
 - -u to Display only unique lines.
 - -d to Display only duplicate lines.

**Q&A**
 - Remove duplicate lines from a file.

   > sort file.txt | uniq
 - Show duplicate lines with counts.

   > sort file.txt | uniq -c
