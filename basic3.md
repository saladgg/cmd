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
_other options include amin, atime, cmin, ctime_
_search file by >10mbs, kbs, gbs_
cmd-dir$find . -size +10M/k/G
*list emty files*
cmd-dir$find . -empty
_search based on permissions_
cmd-dir$find . -perm 777
cmd-dir$find testdir -perm 664
_change group ownership of user salad to www-data on cmd-dir files_
_{} holds the result, + ends the command_
cmd-dir$find . -exec chown salad:www-data {} +
*change permission on testdir directory*
cmd-dir$find cmd -type d -exec chmod 755 {} +
_find all the files with .jpg extension_
cmd-dir$find . -type f -name "*.jpg"
cmd-dir$find . -type f -name "\*.jpg" -maxdepth 1 -exec rm {} +
