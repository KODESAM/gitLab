# Git Create Branch 
Nautilus developers are actively working on one of the project repositories, /usr/src/kodekloudrepos/cluster. 
They recently decided to implement some new features in the application, and they want to maintain those new changes in a separate branch. 
Below are the requirements that have been shared with the DevOps team:

On Storage server in Stratos DC create a new branch xfusioncorp_cluster from master branch in /usr/src/kodekloudrepos/cluster git repo.
```
thor@jump_host ~$ ssh natasha@ststor01
The authenticity of host 'ststor01 (172.16.238.15)' can't be established.
ECDSA key fingerprint is SHA256:U10N6tIhLYp+cUhSAYN7cXLIvJw0IZRBbqul8Oltvc0.
ECDSA key fingerprint is MD5:a0:fc:e4:7e:b7:c4:cb:62:bc:b5:a5:7a:cb:20:21:35.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'ststor01,172.16.238.15' (ECDSA) to the list of known hosts.
natasha@ststor01's password: 
[natasha@ststor01 ~]$ sudo su -

We trust you have received the usual lecture from the local System
Administrator. It usually boils down to these three things:

    #1) Respect the privacy of others.
    #2) Think before you type.
    #3) With great power comes great responsibility.

[sudo] password for natasha: 
[root@ststor01 ~]# cd /usr/src/kodekloudrepos/cluster
[root@ststor01 cluster]# ls -l
total 8
-rw-r--r-- 1 root root 34 Apr  9 20:51 data.txt
-rw-r--r-- 1 root root 34 Apr  9 20:51 info.txt
```
```
[root@ststor01 cluster]# git status
```
On branch kodekloud_cluster
nothing to commit, working directory clean

```
[root@ststor01 cluster]# git checkout master
```
Switched to branch 'master'

```
[root@ststor01 cluster]# git status
```
On branch master
nothing to commit, working directory clean
```
[root@ststor01 cluster]# git checkout -b xfusioncorp_cluster
```
Switched to a new branch 'xfusioncorp_cluster'
```
[root@ststor01 cluster]# git status
```
On branch xfusioncorp_cluster
nothing to commit, working directory clean
```
[root@ststor01 cluster]# git branch -a
```
  kodekloud_cluster
  master
* xfusioncorp_cluster
  remotes/origin/master
[root@ststor01 cluster]# 
