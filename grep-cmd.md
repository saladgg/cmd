## global regular expression print

- search for lines containing lorem a file  
  cmd-dir\$grep "lorem" search.txt
- search for exact match of the word lorem  
  cmd-dir\$grep -w "lorem" search.txt
- search ignoring case  
  cmd-dir\$grep -wi "lorem" search.txt
- include the line number to search result  
  cmd-dir\$grep -win "lorem" search.txt
- search for 2 lines before our match  
  cmd-dir\$grep -win -B 2 "electronic" search.txt
- include 2 lines before and after match  
  cmd-dir\$grep -win -C 2 "electronic" search.txt
- include two lines after our match  
  cmd-dir\$grep -win -A 2 "electronic" search.txt
- search for the word cat in all files in the current dir  
  cmd-dir\$grep -win "electronic" ./\*.txt
- search recursively for a word in all current dir/subdir files  
  cmd-dir\$grep -winr "make" .
- search recursively for a word in all current dir/subdir files, list the files that contain the match.  
  cmd-dir\$grep wirl "make" .
- list all git commit command history  
  cmd-dir\$history | grep "git commit"
- find commit on specific file  
  cmd-dir\$history | grep "git commit" | grep "basic2.md"
