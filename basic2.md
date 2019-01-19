## basic commands 2

- create dir  
  cmddir\$mkdir testdir
- create file in test dir  
  testdir\$touch test_file.txt
- edit the file  
  testdir\$gedit test_file.txt
- copy the file, call it copied.txt  
  testdir\$cp test_file.txt copied.txt
- rename a file  
  testdir\$mv test_file.txt orig_file.txt
- create another dir at the same level as the current dir  
  testdir\$mkdir ../testdir2
- move orig_file.txt to testdir2  
  testdir\$mv orig_file.txt ../testdir2/
- OR move and rename  
  testdir\$mv orig_file.txt ../testdir2/somename.txt
- remove file  
  testdir\$rm filename
- copy dir  
  cmd-dir\$cp -r testdir testdir4
- remove dir  
  cmd-dir\$rm -r testdir4
