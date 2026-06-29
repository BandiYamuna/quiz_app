Windows PowerShell 5.1
Copyright (C) Microsoft Corporation. All rights reserved.

Install the latest PowerShell for new features and improvements! https://aka.ms/PSWindows

PS C:\Users\19400> mkdir StudentManagement


    Directory: C:\Users\19400


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        29-06-2026     22:40                StudentManagement


PS C:\Users\19400> cd StudentManagement
PS C:\Users\19400\StudentManagement> git init
Initialized empty Git repository in C:/Users/19400/StudentManagement/.git/
PS C:\Users\19400\StudentManagement> cd /
PS C:\> cd Users
PS C:\Users> cd 19400
PS C:\Users\19400> cd ecommerce
PS C:\Users\19400\ecommerce> git status
fatal: not a git repository (or any of the parent directories): .git
PS C:\Users\19400\ecommerce> git init
Initialized empty Git repository in C:/Users/19400/ecommerce/.git/
PS C:\Users\19400\ecommerce> git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
PS C:\Users\19400\ecommerce> git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\19400\ecommerce> git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        footer.html
        index.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\19400\ecommerce> git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        footer.html
        index.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\19400\ecommerce> git add index.html
PS C:\Users\19400\ecommerce> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        footer.html

PS C:\Users\19400\ecommerce> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        footer.html

PS C:\Users\19400\ecommerce> git add .
PS C:\Users\19400\ecommerce> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   about.html
        new file:   footer.html
        new file:   index.html

PS C:\Users\19400\ecommerce> git commit -m "footer about add"
[master (root-commit) 6dda493] footer about add
 3 files changed, 9 insertions(+)
 create mode 100644 about.html
 create mode 100644 footer.html
 create mode 100644 index.html
PS C:\Users\19400\ecommerce> git log
commit 6dda49354efd3f7714631a37f56824d060b1f699 (HEAD -> master)
Author: Yamuna <bandiyamuna15@gmail.com>
Date:   Mon Jun 29 23:44:44 2026 +0530

    footer about add
PS C:\Users\19400\ecommerce> git show 6dda49354efd3f7714631a37f56824d060b1f699
commit 6dda49354efd3f7714631a37f56824d060b1f699 (HEAD -> master)
Author: Yamuna <bandiyamuna15@gmail.com>
Date:   Mon Jun 29 23:44:44 2026 +0530

    footer about add

diff --git a/about.html b/about.html
new file mode 100644
index 0000000..e69de29
diff --git a/footer.html b/footer.html
new file mode 100644
index 0000000..e69de29
diff --git a/index.html b/index.html
new file mode 100644
index 0000000..47b3831
--- /dev/null
+++ b/index.html
@@ -0,0 +1,9 @@
+<!DOCTYPE html>
+<html>
+<body>
+
+<h1>My First Heading</h1>
+<p>My first paragraph.</p>
+<nav> this is nav</nav>
+</body>
+</html>
\ No newline at end of file
PS C:\Users\19400\ecommerce> git status
On branch master
nothing to commit, working tree clean
PS C:\Users\19400\ecommerce>  git remote add origin https://github.com/BandiYamuna/quiz_app.git
PS C:\Users\19400\ecommerce> git branch -M main
PS C:\Users\19400\ecommerce> git branch
* main
PS C:\Users\19400\ecommerce> git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 361 bytes | 90.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/BandiYamuna/quiz_app.git
 * [new branch]      main -> main
PS C:\Users\19400\ecommerce> git add .
PS C:\Users\19400\ecommerce> git commit -M "add test file"
error: unknown switch `M'
usage: git commit [-a | --interactive | --patch] [-s] [-v] [-u<mode>] [--amend]
                  [--dry-run] [(-c | -C | --squash) <commit> | --fixup [(amend|reword):]<commit>]
                  [-F <file> | -m <msg>] [--reset-author] [--allow-empty]
                  [--allow-empty-message] [--no-verify] [-e] [--author=<author>]
                  [--date=<date>] [--cleanup=<mode>] [--[no-]status]
                  [-i | -o] [--pathspec-from-file=<file> [--pathspec-file-nul]]
                  [(--trailer <token>[(=|:)<value>])...] [-S[<keyid>]]
                  [--] [<pathspec>...]

    -q, --[no-]quiet      suppress summary after successful commit
    -v, --[no-]verbose    show diff in commit message template

Commit message options
    -F, --[no-]file <file>
                          read message from file
    --[no-]author <author>
                          override author for commit
    --[no-]date <date>    override date for commit
    -m, --[no-]message <message>
                          commit message
    -c, --[no-]reedit-message <commit>
                          reuse and edit message from specified commit
    -C, --[no-]reuse-message <commit>
                          reuse message from specified commit
    --[no-]fixup [(amend|reword):]commit
                          use autosquash formatted message to fixup or amend/reword specified commit
    --[no-]squash <commit>
                          use autosquash formatted message to squash specified commit
    --[no-]reset-author   the commit is authored by me now (used with -C/-c/--amend)
    --trailer <trailer>   add custom trailer(s)
    -s, --[no-]signoff    add a Signed-off-by trailer
    -t, --[no-]template <file>
                          use specified template file
    -e, --[no-]edit       force edit of commit
    --[no-]cleanup <mode> how to strip spaces and #comments from message
    --[no-]status         include status in commit message template
    -S, --[no-]gpg-sign[=<key-id>]
                          GPG sign commit

Commit contents options
    -a, --[no-]all        commit all changed files
    -i, --[no-]include    add specified files to index for commit
    --[no-]interactive    interactively add files
    -p, --[no-]patch      interactively add changes
    -o, --[no-]only       commit only specified files
    -n, --no-verify       bypass pre-commit and commit-msg hooks
    --verify              opposite of --no-verify
    --[no-]dry-run        show what would be committed
    --[no-]short          show status concisely
    --[no-]branch         show branch information
    --[no-]ahead-behind   compute full ahead/behind values
    --[no-]porcelain      machine-readable output
    --[no-]long           show status in long format (default)
    -z, --[no-]null       terminate entries with NUL
    --[no-]amend          amend previous commit
    --no-post-rewrite     bypass post-rewrite hook
    --post-rewrite        opposite of --no-post-rewrite
    -u, --[no-]untracked-files[=<mode>]
                          show untracked files, optional modes: all, normal, no. (Default: all)
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character

PS C:\Users\19400\ecommerce> git commit -m "add test file"
[main b216e8c] add test file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test.txt
PS C:\Users\19400\ecommerce> git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\19400\ecommerce> git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 239 bytes | 239.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/BandiYamuna/quiz_app.git
   6dda493..b216e8c  main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\19400\ecommerce> git remote -v
origin  https://github.com/BandiYamuna/quiz_app.git (fetch)
origin  https://github.com/BandiYamuna/quiz_app.git (push)
PS C:\Users\19400\ecommerce>




