[TOC]

代码
```
PS C:\Users\lenovo\CmgStorage> ls


    目录: C:\Users\lenovo\CmgStorage


Mode                 LastWriteTime         Length Name   
----                 -------------         ------ ----   
d-----         2023/8/25     15:54                0.Daily
d-----         2023/8/25     15:55                A.MyNot
                                                  e      
                                                  ate     
d-----         2023/8/25     16:07                C.MyLea 
d-----         2023/8/25     15:56                D.MyLib 
                                                  rary    
d-----         2023/8/25     15:57                E.MyLif 
                                                  e       
d-----         2023/8/25     15:57                F.Other 
                                                  s       


PS C:\Users\lenovo\CmgStorage> git init
Initialized empty Git repository in C:/Users/lenovo/CmgStorage/.git/
PS C:\Users\lenovo\CmgStorage> ls


    目录: C:\Users\lenovo\CmgStorage


Mode                 LastWriteTime         Length Name    
----                 -------------         ------ ----    
d-----         2023/8/25     15:54                0.Daily 
d-----         2023/8/25     15:55                A.MyNot
                                                  e       
d-----         2023/8/25     16:06                B.MyCre 
                                                  rn
d-----         2023/8/25     15:56                D.MyLib      
                                                  rary
                                                  e
d-----         2023/8/25     15:57                F.Other      
                                                  s


PS C:\Users\lenovo\CmgStorage> git remote add origin https://github.com/ChenMinggao                                           thub.com/ChenMinggao
PS C:\Users\lenovo\CmgStorage> git push -u origin master       
error: src refspec master does not match any.
gao'                                                           gao'
PS C:\Users\lenovo\CmgStorage> git -V
unknown option: -V
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]
PS C:\Users\lenovo\CmgStorage> git
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:      

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)       
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink 
   reset      Reset current HEAD to the specified state        
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)   
   bisect     Use binary search to find the commit that introduced a bug
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   branch     List, create, or delete branches
   checkout   Switch branches or restore working tree files    
   commit     Record changes to the repository
   diff       Show changes between commits, commit and working 
tree, etc
   merge      Join two or more development histories together  
   rebase     Reapply commits on top of another base tip       
   tag        Create, list, delete or verify a tag object signed with GPG
collaborate (see also: git help workflows)
'git help -a' and 'git help -g' list available subcommands and 
some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
PS C:\Users\lenovo\CmgStorage> git --version
git version 2.18.0.windows.1
PS C:\Users\lenovo\CmgStorage> git config --global user.name "chenminggao"
PS C:\Users\lenovo\CmgStorage> git config --global user.email "zhangnihan1985@163.com"
PS C:\Users\lenovo\CmgStorage> git config --list
core.symlinks=false
core.autocrlf=true
core.fscache=true
color.diff=auto
color.status=auto
color.branch=auto
color.interactive=true
help.format=html
rebase.autosquash=true
http.sslcainfo=d:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
http.sslbackend=openssl
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
credential.helper=manager
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.required=true
user.name=chenminggao
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
remote.origin.url=https://github.com/ChenMinggao
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*        
PS C:\Users\lenovo\CmgStorage> git init
Reinitialized existing Git repository in C:/Users/lenovo/CmgStorage/.git/
PS C:\Users\lenovo\CmgStorage> ls


    目录: C:\Users\lenovo\CmgStorage

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----         2023/8/25     15:54                0.Daily      
d-----         2023/8/25     15:55                A.MyNote     
d-----         2023/8/25     16:06                B.MyCreate   
d-----         2023/8/25     16:07                C.MyLearn    
d-----         2023/8/25     15:56                D.MyLibrary  
d-----         2023/8/25     15:57                E.MyLife     
d-----         2023/8/25     15:57                F.Others     


PS C:\Users\lenovo\CmgStorage> git status
On branch master

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        B.MyCreate/
        C.MyLearn/

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\lenovo\CmgStorage> git add .
PS C:\Users\lenovo\CmgStorage> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   B.MyCreate/0.Meta/EssayTemplate.md
        new file:   B.MyCreate/0.Meta/Readme.md
        new file:   B.MyCreate/0.Meta/StoryTemplate.md
        new file:   "B.MyCreate/1.Chinese/Essay/\344\275\234\346\226\207.md"
        new file:   "B.MyCreate/1.Chinese/Essay/\345\217\257\347\210\261\347\232\204\345\215\227\347\223\234.md"
        new file:   "B.MyCreate/1.Chinese/Essay/\345\255\246\346\240\241\347\232\204\350\212\261.md"
        new file:   "B.MyCreate/1.Chinese/Essay/\346\210\221\345\255\246\344\274\232\344\272\206\345\256\275\345\256\271.md"  
        new file:   "B.MyCreate/1.Chinese/Essay/\346\210\221\347\232\204\347\214\253\345\244\264\351\271\260\347\210\270\347\210\270.md"
        new file:   "B.MyCreate/1.Chinese/Essay/\346\213\211\345\261\216.md"
        new file:   "B.MyCreate/1.Chinese/Essay/\346\240\221\346\207\222\347\210\266\345\255\220\344\277\251.md"
        new file:   "B.MyCreate/1.Chinese/Essay/\346\250\261\35        new file:   "B.MyCreate/1.Chinese/Essay/\347\233\270\347\272\246\345\215\201\350\277\220.md"
        new file:   "C.MyLearn/8.SoftDevelopment/C++/\345\221\250\351\225\277.cpp"
        new file:   "C.MyLearn/8.SoftDevelopment/C++/\345\271\263\346\226\271.cpp"
        new file:   "C.MyLearn/8.SoftDevelopment/C++/\347\272\277\346\256\265.CPP"
        new file:   "C.MyLearn/8.SoftDevelopment/C++/\350\264\255\347\211\251.CPP"

PS C:\Users\lenovo\CmgStorage> git commit -m "first commit"    
[master (root-commit) 9751488] first commit
 16 files changed, 296 insertions(+)
 create mode 100644 B.MyCreate/0.Meta/EssayTemplate.md
 create mode 100644 B.MyCreate/0.Meta/Readme.md
 create mode 100644 B.MyCreate/0.Meta/StoryTemplate.md
 create mode 100644 "B.MyCreate/1.Chinese/Essay/\344\275\234\346\226\207.md"
 create mode 100644 "B.MyCreate/1.Chinese/Essay/\345\217\257\347\210\261\347\232\204\345\215\227\347\223\234.md"
 create mode 100644 "B.MyCreate/1.Chinese/Essay/\345\255\246\346\240\241\347\232\204\350\212\261.md"
 create mode 100644 "B.MyCreate/1.Chinese/Essay/\346\210\221\345\255\246\344\274\232\344\272\206\345\256\275\345\256\271.md"  
 create mode 100644 "B.MyCreate/1.Chinese/Essay/\346\210\221\347\232\204\347\214\253\345\244\264\351\271\260\347\210\270\347\210\270.md"
 create mode 100644 "B.MyCreate/1.Chinese/Essay/\346\213\211\345\261\216.md"
 create mode 100644 "B.MyCreate/1.Chinese/Essay/\346\240\221\346\207\222\347\210\266\345\255\220\344\277\251.md"
0\212\261\346\240\221.md"
 create mode 100644 "B.MyCreate/1.Chinese/Essay/\347\233\270\347\272\246\345\215\201\350\277\220.md"
 create mode 100644 "C.MyLearn/8.SoftDevelopment/C++/\345\221\250\351\225\277.cpp"
 create mode 100644 "C.MyLearn/8.SoftDevelopment/C++/\345\271\263\346\226\271.cpp"
 create mode 100644 "C.MyLearn/8.SoftDevelopment/C++/\347\272\277\346\256\265.CPP"
 create mode 100644 "C.MyLearn/8.SoftDevelopment/C++/\350\264\255\347\211\251.CPP"
PS C:\Users\lenovo\CmgStorage> ls


    目录: C:\Users\lenovo\CmgStorage


----                 -------------         ------ ----
d-----         2023/8/25     15:55                A.MyNote     
d-----         2023/8/25     15:56                D.MyLibrary  
d-----         2023/8/25     15:57                E.MyLife     

PS C:\Users\lenovo\CmgStorage> git remote add origin https://gifatal: remote origin already exists.
PS C:\Users\lenovo\CmgStorage> git commit -m 
error: switch `m' requires a value
PS C:\Users\lenovo\CmgStorage> git commit -m essay
On branch master
PS C:\Users\lenovo\CmgStorage> git commit -m essagy
[master e2c9f77] essagy
fatal: unable to access 'https://github.com/ChenMinggao/': Failed to connect to github.com port 443: Timed out
PS C:\Users\lenovo\CmgStorage> git remote add origin https://github.com/ChenMinggao/CmgStorage
fatal: remote origin already exists.
PS C:\Users\lenovo\CmgStorage> git remote set-url origin git@htPS C:\Users\lenovo\CmgStorage> git push origin master
PS C:\Users\lenovo\CmgStorage> git remote set-url origin git@gifatal: 'git@github.com/ChenMinggao/CmgStorage.git' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\lenovo\CmgStorage> git remote rm origin\
PS C:\Users\lenovo\CmgStorage> git remote rm origin
.com/ChenMinggao/CmgStorage.git
ear to be a git repository
fatal: Could not read from remote repository.

and the repository exists.
PS C:\Users\lenovo\CmgStorage> git remote add origin https://github.com/ChenMinggao/CmgStorage.git
PS C:\Users\lenovo\CmgStorage> git remote rm origin
PS C:\Users\lenovo\CmgStorage> git remote add origin https://github.com/ChenMinggao/CmgStorage.git
PS C:\Users\lenovo\CmgStorage> git push -u origin master       
fatal: unable to access 'https://github.com/ChenMinggao/CmgStorage.git/': OpenSSL SSL_connect: SSL_ERROR_SYSCALL in connection to github.com:443
PS C:\Users\lenovo\CmgStorage> git push -u origin master       
fatal: unable to access 'https://github.com/ChenMinggao/CmgStorage.git/': OpenSSL SSL_connect: SSL_ERROR_SYSCALL in connection to github.com:443
PS C:\Users\lenovo\CmgStorage> git push -u origin master       
Enumerating objects: 31, done.
Counting objects: 100% (31/31), done.
Delta compression using up to 4 threads.
Compressing objects: 100% (25/25), done.
Writing objects: 100% (31/31), 9.13 KiB | 283.00 KiB/s, done.  
Total 31 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/ChenMinggao/CmgStorage.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
PS C:\Users\lenovo\CmgStorage> ls


    目录: C:\Users\lenovo\CmgStorage


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----         2023/8/25     15:54                0.Daily      
d-----         2023/8/25     15:55                A.MyNote     
d-----         2023/8/25     16:06                B.MyCreate   
d-----         2023/8/25     16:07                C.MyLearn   
d-----         2023/8/25     15:56                D.MyLibrary  
d-----         2023/8/25     15:57                E.MyLife     
d-----         2023/8/25     15:57                F.Others     


PS C:\Users\lenovo\CmgStorage> 

```

## git bash
```

lenovo@LAPTOP-0KN3I6GI MINGW64 ~ (master)
$ ^C

lenovo@LAPTOP-0KN3I6GI MINGW64 ~ (master)
$ ssh-keygen -t rsa -C "zhangnihan1985@163.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/lenovo/.ssh/id_rsa):
/c/Users/lenovo/.ssh/id_rsa already exists.
Overwrite (y/n)? y
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/lenovo/.ssh/id_rsa.
Your public key has been saved in /c/Users/lenovo/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:Ak8qCUjk2Eh0r33npOPrQ7Nrox7N5ReobEEuh1s2xLA zhangnihan1985@163.com
The key's randomart image is:
+---[RSA 2048]----+
|o= . .           |
|*o. . +          |
|=.. .E.+         |
| . .o==   .      |
|  o..+oOS= .     |
|   .  @+@   .    |
|     o.Ooo .     |
|      +=. .      |
|    .o+==        |
+----[SHA256]-----+

lenovo@LAPTOP-0KN3I6GI MINGW64 ~ (master)
$ ssh -T git@github.com
The authenticity of host 'github.com (20.205.243.166)' can't be established.
ECDSA key fingerprint is SHA256:p2QAMXNIC1TJYWeIOttrVc98/R1BUFWu3/LiyKgUfQM.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'github.com,20.205.243.166' (ECDSA) to the list of known hosts.
Hi ChenMinggao! You've successfully authenticated, but GitHub does not provide shell access.

lenovo@LAPTOP-0KN3I6GI MINGW64 ~ (master)
$

```







## 参考
- [Github——git本地仓库建立与远程连接](http://www.taodudu.cc/news/show-1252114.html?action=onClick)
- [三种方法解决 fatal: remote origin already exists](https://blog.csdn.net/qq_34769162/article/details/116379638)

## changelog
- 2023年8月30日21:57:31 by chenhao
