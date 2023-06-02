# Lipsa

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop (master)
$ mkdir geek                          // create a folder

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop (master)
$ cd geek                       //Go to that folder

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ touch first.txt                  //create a new file

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git init                              //initialize empty git repository
Initialized empty Git repository in F:/Desktop/geek/.git/

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git add first.txt                        //add the file to staging area 

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git commit -m "adding first.txt"                         //commit this file
[master (root-commit) 72075bc] adding first.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 first.txt

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git log                                                     //check the commit details
commit 72075bc84ff17d838d9ac5f5fbf879d7c0ea6b1f (HEAD -> master)
Author: Lipsa760 <lipsamayeejena76@gmail.com>
Date:   Fri Jun 2 10:36:36 2023 +0530

    adding first.txt

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ touch second.txt                                    //create another new file

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git add second.txt                                     //add to staging area

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git commit -m "adding second.txt"                          //commit with message
[master 1452994] adding second.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 second.txt

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git status                                                 //check the status
On branch master
nothing to commit, working tree clean

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git rm first.txt                            //remove first.txt file
rm 'first.txt'

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git add .                                      //add the changes to staging area

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git commit -m "removing first.txt"                     //commit with "remove message
[master fd0fe55] removing first.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 first.txt

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git log                                                      //check the commit details
commit fd0fe55a2373de95a5bf42f09749839f2f8baea0 (HEAD -> master)
Author: Lipsa760 <lipsamayeejena76@gmail.com>
Date:   Fri Jun 2 10:39:07 2023 +0530

    removing first.txt

commit 145299442e8a1f693926898eb982011eebc69e9f
Author: Lipsa760 <lipsamayeejena76@gmail.com>
Date:   Fri Jun 2 10:37:22 2023 +0530

    adding second.txt

commit 72075bc84ff17d838d9ac5f5fbf879d7c0ea6b1f
Author: Lipsa760 <lipsamayeejena76@gmail.com>
Date:   Fri Jun 2 10:36:36 2023 +0530

    adding first.txt

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git remote add origin https://github.com/Lipsa760/Lipsa.git                   //add those files in github

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (master)
$ git branch -M main                                              //change the branch from master to main

hp@DESKTOP-GK8PDCI MINGW64 /f/Desktop/geek (main)
$ git push -u origin main                                            //push the file to github repository
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (7/7), 654 bytes | 654.00 KiB/s, done.
Total 7 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Lipsa760/Lipsa.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
