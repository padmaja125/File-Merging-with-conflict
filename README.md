vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ git init
Reinitialized existing Git repository in C:/Data/Padhu/Training/Assignment/Git/exercise-9/.git/

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ vi index.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ git add .

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ git commit -m 'updated the file'
[master 1241778] updated the file
 2 files changed, 7 insertions(+)
 create mode 100644 index.html.orig

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ git branch my-new-branch

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ vi about-us.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ git add .

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ vi index.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ git checkout my-new-branch
Switched to branch 'my-new-branch'
M       about-us.html
M       index.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (my-new-branch)
$ vi about.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (my-new-branch)
$ vi about-us.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (my-new-branch)
$ vi index.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (my-new-branch)
$ git add .
warning: LF will be replaced by CRLF in about.html.
The file will have its original line endings in your working directory

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (my-new-branch)
$ git commit -m 'commited in branch'
[my-new-branch d10c116] commited in branch
 3 files changed, 5 insertions(+), 1 deletion(-)
 create mode 100644 about.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (my-new-branch)
$ git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ vi index.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ git add .

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ git commit -m 'commited in master'
[master 8a094ab] commited in master
 1 file changed, 2 insertions(+), 3 deletions(-)

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master)
$ git merge my-new-branch
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master|MERGING)
$ vi index.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master|MERGING)
$ git add index.html

vimal@CREATIVEBEE MINGW64 /c/Data/Padhu/Training/Assignment/Git/exercise-9 (master|MERGING)
$ git commit -m "Resolved merge conflict by updated index.html'
> "
[master 49f7af4] Resolved merge conflict by updated index.html'
