## basic cmds 3

- list all dirs and files in testdir  
  cmd-dir\$find testdir
- list only dir/file  
  cmd-dir\$find . -type d  
  cmd-dir\$find . -type f
- find all files in the current dir starting with name basi  
  cmd-dir\$find . -type f -name "basi\*"
- find all files in the current dir ending with .py  
  cmd-dir\$find . -type f -name "\*.py"
- find files modified less than 10 min ago  
  cmd-dir\$find . -type f -mmin -10
- find files modified >5 ago >10 min  
  cmd-dir\$find . -type f -mmin +5 -mmin -10
- return files modified less than 10 days ago  
  cmd-dir\$find . -type f -mtime -10
- other options include amin, atime, cmin, ctime
- search file by size >size in M, k, G  
   cmd-dir\$find . -size +10M
- list emty files  
  cmd-dir\$find . -empty
- search based on permissions  
  cmd-dir\$find . -perm 777  
  cmd-dir\$find testdir -perm 664
- change group ownership of user salad to www-data on cmd-dir files  
  {} holds the result, + ends the command  
  cmd-dir\$find . -exec chown salad:www-data {} +
- change permission on testdir directory  
  cmd-dir\$find cmd -type d -exec chmod 755 {} +
- find all the files with .jpg extension  
  cmd-dir\$find . -type f -name "\*.jpg"  
  cmd-dir\$find . -type f -name "\*.jpg" -maxdepth 1 -exec rm {} +
