# Shell-Script-cheatsheet

### Navigating your filesystem
|# | Command | Action |  
|--|---------|--------|
|1.| ```pwd``` | To get the path of directory you are in |
|2.| ```ls``` | List the contents of the directory|  
|3.| ```ls -lh``` | Displays the details of the files in a folder |
|4.| ```ls -a``` | Displays hidden files as well |
|5.| ```ls -R -F``` | List the files everything in the directory (nested)  |  
|6.| ```cd [path to the directory]``` | Move to the directory |
|7.| ```cd ..``` | Move to the parent directory one level above |
|8.| ```cd ../..``` | Move to the parent directory two levels above | 

### Create, Copy, Move, Rename, Delete files and directories
|# | Command | Action |  
|--|---------|--------|
|1.| ```mkdir [directory]``` | To create a new directory in the current directory|
|2.| ```touch [filename].txt``` | To create the file |
|3.| ```open [filename].txt ``` | Opens the file |
|4.| ```cp [filename] [new_filename]``` | Copy the file  |
|5.|```cp -R [foldername]/ [new_foldername]``` | Copy folders |
|6.| ```mv [filename] [directory]``` | Move file to the folder |
|7.|```mv [foldername] [foldername]```| Move folder|
|8.| ```mv [filename] [new filename]``` | Rename the file/folder |
|9.| ```rm [filename]``` | Delete the file |
|10.| ```rmdir [directory name]```| Delete the directory |
|11.| ```rm [filename]```| Remove the file |
|12.| ```rm -r [foldername]```| Remove the folder |
|13.| ```rm -rf [foldername]```| Remove the file |

### Find command
|# | Command | Action |  
|--|---------|--------|
|1.| find . | Shows all the files in the directory in a tree structure|
|2.| find . -type d| Shows only the directories |
|3.| find . -type f| Shows only files|
|4.| find . -type f -name "<filename.txt>" | Shows the path to the file |
|5.| find . -type f -name "test*" | Shows all the files starting with test (case sensitive)|
|6.| find . -type f -iname "test*" | Shows  all the files case insensitive of the name |
|7.| find . -type f -mmin -n | Returns the files modified in last n mins |
|8.| find . -type f -mmin +1 -mmin -5 | Returns the files modified more than 1 min and less than 5 mins |
|9.| find . -type f -mtime +20 | Returns the files modified more than 20 days ago |
|10.| find . -size +5M | Shows files bigger than 5MB |
|11.| find . -empty| Shows empty files |
|12. | find . -type f -name "*.jpg" -maxdepth 1| Shows files in current directory only as maxdepth is 1|
|13. | find . -type f -name "*.jpg" -maxdepth 1 -exec rm {} + | Removes the files ending with .jpg |

### Grep command
|# | Command | Action |  
|--|---------|--------|
|1.|grep "Harshith" names.txt| Returns the word from names.txt (Harshith, HarshithReddy)|
|2.|grep -w "Harshith names.txt | Returns only when Harshith is a word (Harshith)|
|3.|grep -wi "Harshith names.txt | Returns only when Harshith is a word and is also case insensitive (harshith, Harshith)|
|4.|grep -win "Harshith names.txt | Returns line numbers as well when Harshith is a word (Harshith)|
|5.|grep -win -A n "Harshith names.txt | Returns n lines after|
|6.|grep -win -B n "Harshith names.txt | Returns n lines before|
|7.|grep -win -C n "Harshith names.txt | Returns n lines in context|



