##basic cmds 3

_list all dirs and files in testdir_
cmd-dir$find testdir
*list only dir/file*
cmd-dir$find . -type d
cmd-dir$find . -type f
*find all files in the current dir starting with name basi*
cmd-dir$find . -type f -name "basi\*"
_find all files in the current dir ending with .py_
cmd-dir$find . -type f -name "*.py"
*find files modified less than 10 min ago*
cmd-dir$find . -type f -mmin -10
_find files modified >5 ago >10 min_
cmd-dir\$find . -type f -mmin +5 -mmin -10
_return files modified less than 10 days ago_
cmd-dir\$find . -type f -mtime -10

7.5 min
