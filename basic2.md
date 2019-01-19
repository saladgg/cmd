##basic commands 2

_create dir_
cmddir$mkdir testdir
*create file in test dir*
testdir$touch test*file.txt
\_edit the file*
testdir$gedit test_file.txt
*copy the file*
testdir$cp test*file.txt copied.txt
\_rename a file*
testdir$mv test_file.txt orig_file.txt
*create another dir at the same level as the current dir*
testdir$mkdir ../testdir2
_move orig_file.txt to testdir2_
testdir$mv orig_file.txt ../testdir2/
*OR move and rename*
testdir$mv orig*file.txt ../testdir2/somename.txt
\_remove file*
testdir$rm filename
*copy dir*
cmd-dir$cp -r testdir testdir4
_command to copy/rename dir = file_
_remove dir_
cmd-dir\$rm -r testdir4
