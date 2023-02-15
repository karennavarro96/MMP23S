:wqHW 1:

2.A

karennavarro@Karens-MacBook-Pro $ git branch
* main
  test1
  test2

2.B
2.C
2.D

karennavarro@Karens-MacBook-Pro $ git add test.txt 
karennavarro@Karens-MacBook-Pro $ git commit -am "Test1 branch, made test.txt"
[test1 e6dcdf9] Test1 branch, made test.txt
 1 file changed, 1 insertion(+)
 create mode 100644 HW/VCS/test.txt
karennavarro@Karens-MacBook-Pro $ 

2.E

karennavarro@Karens-MacBook-Pro $ git checkout test2
Switched to branch 'test2'
karennavarro@Karens-MacBook-Pro $ ls
README.md

I dont see the file because I have not merge all the branches together. The file only exist in one branch. 

2.F
2.G

karennavarro@Karens-MacBook-Pro $ vim test.txt
karennavarro@Karens-MacBook-Pro $ git checkout test1
error: The following untracked working tree files would be overwritten by checkout:
	HW/VCS/test.txt
Please move or remove them before you switch branches.
Aborting
karennavarro@Karens-MacBook-Pro $ 
karennavarro@Karens-MacBook-Pro $ git add test.txt
karennavarro@Karens-MacBook-Pro $ git commit -am "Test2 branch, made test.txt"
[test2 f2cf0e4] Test2 branch, made test.txt
 1 file changed, 1 insertion(+)
 create mode 100644 HW/VCS/test.txt
karennavarro@Karens-MacBook-Pro $ git checkout test1
Switched to branch 'test1'



2.H

2.O

karennavarro@Karens-MacBook-Pro $ git branch -d test1
error: The branch 'test1' is not fully merged.
If you are sure you want to delete it, run 'git branch -D test1'.

2.P


karennavarro@Karens-MacBook-Pro $ git branch -d test1
error: The branch 'test1' is not fully merged.
If you are sure you want to delete it, run 'git branch -D test1'.
karennavarro@Karens-MacBook-Pro $ git branch
* main
  test1
  test2

At the moment I get the same error message for both trying to delete.

2.R

karennavarro@Karens-MacBook-Pro $ git branch -d test2
error: Cannot delete branch 'test2' checked out at '/Users/karennavarro/Documents/MM3/MMP23S'


2.S

karennavarro@Karens-MacBook-Pro $ git branch -D test2
Deleted branch test2 (was f2cf0e4).
karennavarro@Karens-MacBook-Pro $ git branch -D test1
Deleted branch test1 (was 0d7ac7d).
karennavarro@Karens-MacBook-Pro $ git branch




E325: ATTENTION
Found a swap file by the name ".README.md.swp"
          owned by: karennavarro   dated: Wed Feb 15 09:56:26 2023
         file name: ~karennavarro/Documents/MM3/MMP23S/HW/VCS/README.md
          modified: YES
         user name: karennavarro   host name: Karens-MacBook-Pro.local
        process ID: 15042
While opening file "README.md"
             dated: Wed Feb 15 09:56:26 2023

(1) Another program may be editing the same file.  If this is the case,
    be careful not to end up with two different instances of the same
    file when making changes.  Quit, or continue with caution.
(2) An edit session for this file crashed.
    If this is the case, use ":recover" or "vim -r README.md"
    to recover the changes (see ":help recovery").
    If you did this already, delete the swap file ".README.md.swp"
    to avoid this message.

Swap file ".README.md.swp" already exists!
"README.md" 3L, 8B
Using swap file ".README.md.swp"
Original file "~/Documents/MM3/MMP23S/HW/VCS/README.md"
E308: Warning: Original file may have been changed
Recovery completed. You should check if everything is OK.
(You might want to write out this file under another name
and run diff with the original file to check for changes)
You may want to delete the .swp file now.





