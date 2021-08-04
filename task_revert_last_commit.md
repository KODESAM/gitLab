[root@ststor01 apps]# ls -l
total 4
-rw-r--r-- 1 root root 33 Aug  4 16:23 apps.txt
[root@ststor01 apps]# ls -a
.  ..  apps.txt  .git
[root@ststor01 apps]# git reset --soft HEAD~1
[root@ststor01 apps]# git status
# On branch master
# Your branch is behind 'origin/master' by 1 commit, and can be fast-forwarded.
#   (use "git pull" to update your local branch)
#
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#       deleted:    info.txt
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#       apps.txt
[root@ststor01 apps]# git log --oneline
03296e3 initial commit
[root@ststor01 apps]# 
