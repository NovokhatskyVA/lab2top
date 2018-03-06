
u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA

$ git config --global user.name 'Питенин Иван'

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA

$ git config --global user.email 'ivan.pitenin@gmail.com'

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA

$ cd /c/Users/u211-05/Desktop/labslab02RepoA

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA

$ git init

Initialized empty Git repository in C:/Users/u211-05/Desktop/labslab02RepoA/.git/

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git status

On branch master

　

Initial commit

　

Untracked files:

  (use "git add <file>..." to include in what will be committed)

　

        .idea/

        CMakeLists.txt

        cmake-build-debug/

        main.cpp

　

nothing added to commit but untracked files present (use "git add" to track)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add main.cpp

warning: LF will be replaced by CRLF in main.cpp.

The file will have its original line endings in your working directory.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git status

On branch master

　

Initial commit

　

Changes to be committed:

  (use "git rm --cached <file>..." to unstage)

　

        new file:   main.cpp

　

Untracked files:

  (use "git add <file>..." to include in what will be committed)

　

        .idea/

        CMakeLists.txt

        cmake-build-debug/

　

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "создал проект и добавил файл main.cpp"

[master (root-commit) 5fac16b] создал проект и добавил файл main.cpp

 1 file changed, 7 insertions(+)

 create mode 100644 main.cpp

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add CMakeLists.txt.

fatal: pathspec 'CMakeLists.txt.' did not match any files

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add CMakeLists.txt

warning: LF will be replaced by CRLF in CMakeLists.txt.

The file will have its original line endings in your working directory.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "добавил файл CMakeLists.txt"

[master fb6f1cc] добавил файл CMakeLists.txt

 1 file changed, 7 insertions(+)

 create mode 100644 CMakeLists.txt

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git status

On branch master

Changes not staged for commit:

  (use "git add <file>..." to update what will be committed)

  (use "git checkout -- <file>..." to discard changes in working directory)

　

        modified:   main.cpp

　

Untracked files:

  (use "git add <file>..." to include in what will be committed)

　

        .idea/

        cmake-build-debug/

　

no changes added to commit (use "git add" and/or "git commit -a")

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add main.cpp

warning: LF will be replaced by CRLF in main.cpp.

The file will have its original line endings in your working directory.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "добавил программу ввода двух чисел"

[master 67bf313] добавил программу ввода двух чисел

 1 file changed, 6 insertions(+), 5 deletions(-)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git ad -a

git: 'ad' is not a git command. See 'git --help'.

　

Did you mean one of these?

        add

        am

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -a

error: unknown switch `a'

usage: git add [<options>] [--] <pathspec>...

　

    -n, --dry-run         dry run

    -v, --verbose         be verbose

　

    -i, --interactive     interactive picking

    -p, --patch           select hunks interactively

    -e, --edit            edit current diff and apply

    -f, --force           allow adding otherwise ignored files

    -u, --update          update tracked files

    -N, --intent-to-add   record only the fact that the path will be added later

    -A, --all             add changes from all tracked and untracked files

    --ignore-removal      ignore paths removed in the working tree (same as --no-all)

    --refresh             don't add, only refresh the index

    --ignore-errors       just skip files which cannot be added because of errors

    --ignore-missing      check if - even missing - files are ignored in dry run

    --chmod <(+/-)x>      override the executable bit of the listed files

　

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

warning: LF will be replaced by CRLF in main.cpp.

The file will have its original line endings in your working directory.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "добавил вывод суммы введенных чисел"

[master 14efa8b] добавил вывод суммы введенных чисел

 1 file changed, 1 insertion(+)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ touch .gitignore

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add .gitignore

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "добавил файлы, которые будут игнорироваться при пуше"

[master 30db045] добавил файлы, которые будут игнорироваться при пуше

 1 file changed, 1 insertion(+)

 create mode 100644 .gitignore

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git status

On branch master

Untracked files:

  (use "git add <file>..." to include in what will be committed)

　

        .idea/

        cmake-build-debug/

　

nothing added to commit but untracked files present (use "git add" to track)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git log

commit 30db0455b2e6fdfe02c42d756700d7dc625ec6b6

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:49:22 2018 +0300

　

    добавил файлы, которые будут игнорироваться при пуше

　

commit 14efa8bfc0d080c4a52e1b28e0ee14cb3840c4fb

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:46:51 2018 +0300

　

    добавил вывод суммы введенных чисел

　

commit 67bf3137384226987ece6f64f2757c67e05a2e23

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:44:56 2018 +0300

　

    добавил программу ввода двух чисел

　

commit fb6f1cc69806cb4a0edf748dafc8b8132da84ef8

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:41:12 2018 +0300

　

    добавил файл CMakeLists.txt

　

commit 5fac16ba88d531368430fbd930991b0d5edc9ada

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:39:30 2018 +0300

　

    создал проект и добавил файл main.cpp

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git diff^C

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git diff 30db0455b2e6fdfe02c42d756700d7dc625ec6b6

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git diff 30db0455b2e6fdfe02c42d756700d7dc625ec6b6 67bf3137384226987ece6f64f2757c67e05a2e23

diff --git a/.gitignore b/.gitignore

deleted file mode 100644

index 5b1511f..0000000

--- a/.gitignore

+++ /dev/null

@@ -1 +0,0 @@

-.idea/, cmake-build-debug/

\ No newline at end of file

diff --git a/main.cpp b/main.cpp

index 467f584..7ef698a 100644

--- a/main.cpp

+++ b/main.cpp

@@ -5,5 +5,4 @@ using namespace std;

 int main()

 { int a, b;cout << "Enter A and B: ";

  cin >> a >> b;

-    cout << "A + B = " << a + b << '\n';

  }

\ No newline at end of file

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git checkout -- main.cpp

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "удалил все строки из main.cpp"

[master 61157da] удалил все строки из main.cpp

 1 file changed, 9 deletions(-)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git reset --hard HEAD~1

HEAD is now at 30db045 добавил файлы, которые будут игнорироваться при пуше

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git remote add origin https://github.com/dolonche/sdt-lab02.git

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git remote -v

origin  https://github.com/dolonche/sdt-lab02.git (fetch)

origin  https://github.com/dolonche/sdt-lab02.git (push)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git push --set-upstream origin master

Username for 'https://github.com': dolonche

Counting objects: 15, done.

Delta compression using up to 2 threads.

Compressing objects: 100% (13/13), done.

Writing objects: 100% (15/15), 1.91 KiB | 0 bytes/s, done.

Total 15 (delta 1), reused 0 (delta 0)

remote: Resolving deltas: 100% (1/1), done.

Branch master set up to track remote branch master from origin.

To https://github.com/dolonche/sdt-lab02.git

 * [new branch]      master -> master

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git clone https://github.com/dolonche/sdt-lab02.git /c/Users/u211-05/Desktop/labslab02RepoA

fatal: destination path 'C:/Users/u211-05/Desktop/labslab02RepoA' already exists and is not an empty directory.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git clone https://github.com/dolonche/sdt-lab02.git /c/Users/u211-05/Desktop/labslab02RepoB

Cloning into 'C:/Users/u211-05/Desktop/labslab02RepoB'...

remote: Counting objects: 15, done.

remote: Compressing objects: 100% (12/12), done.

remote: Total 15 (delta 1), reused 15 (delta 1), pack-reused 0

Unpacking objects: 100% (15/15), done.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "добавил вывод первго числа, умноженного на два"

[master 9051876] добавил вывод первго числа, умноженного на два

 1 file changed, 1 insertion(+)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git push origin master

Username for 'https://github.com': dolonche

Counting objects: 3, done.

Delta compression using up to 2 threads.

Compressing objects: 100% (3/3), done.

Writing objects: 100% (3/3), 391 bytes | 0 bytes/s, done.

Total 3 (delta 2), reused 0 (delta 0)

remote: Resolving deltas: 100% (2/2), completed with 2 local objects.

To https://github.com/dolonche/sdt-lab02.git

   30db045..9051876  master -> master

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ cd /c/Users/u211-05/Desktop/labslab02RepoB

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ git pull

remote: Counting objects: 3, done.

remote: Compressing objects: 100% (1/1), done.

remote: Total 3 (delta 2), reused 3 (delta 2), pack-reused 0

Unpacking objects: 100% (3/3), done.

From https://github.com/dolonche/sdt-lab02

   30db045..9051876  master     -> origin/master

Updating 30db045..9051876

Fast-forward

 main.cpp | 1 +

 1 file changed, 1 insertion(+)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ git log

commit 905187614d3dade491139f3ba4e616d29117b681

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 10:06:04 2018 +0300

　

    добавил вывод первго числа, умноженного на два

　

commit 30db0455b2e6fdfe02c42d756700d7dc625ec6b6

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:49:22 2018 +0300

　

    добавил файлы, которые будут игнорироваться при пуше

　

commit 14efa8bfc0d080c4a52e1b28e0ee14cb3840c4fb

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:46:51 2018 +0300

　

    добавил вывод суммы введенных чисел

　

commit 67bf3137384226987ece6f64f2757c67e05a2e23

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:44:56 2018 +0300

　

    добавил программу ввода двух чисел

　

commit fb6f1cc69806cb4a0edf748dafc8b8132da84ef8

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:41:12 2018 +0300

　

    добавил файл CMakeLists.txt

　

commit 5fac16ba88d531368430fbd930991b0d5edc9ada

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:39:30 2018 +0300

　

    создал проект и добавил файл main.cpp

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ git history

git: 'history' is not a git command. See 'git --help'.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ cd /c/Users/u211-05/Desktop/labslab02RepoA

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ cd /c/Users/u211-05/Desktop/labslab02RepoB

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ git commit -m "добавил печать разности введенных элементов"

[master 094d25c] добавил печать разности введенных элементов

 1 file changed, 1 insertion(+)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ git push origin master

Username for 'https://github.com': dolonche

Counting objects: 3, done.

Delta compression using up to 2 threads.

Compressing objects: 100% (3/3), done.

Writing objects: 100% (3/3), 394 bytes | 0 bytes/s, done.

Total 3 (delta 2), reused 0 (delta 0)

remote: Resolving deltas: 100% (2/2), completed with 2 local objects.

To https://github.com/dolonche/sdt-lab02.git

   9051876..094d25c  master -> master

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ cd /c/Users/u211-05/Desktop/labslab02RepoA

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "добавил комментарий в файл main.cpp"

On branch master

Your branch is up-to-date with 'origin/master'.

Untracked files:

        .idea/

        cmake-build-debug/

　

nothing added to commit but untracked files present

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "добавил комментарий в файл main.cpp"

[master 4ba8e60] добавил комментарий в файл main.cpp

 1 file changed, 1 insertion(+), 1 deletion(-)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git fetch

remote: Counting objects: 3, done.

remote: Compressing objects: 100% (1/1), done.

remote: Total 3 (delta 2), reused 3 (delta 2), pack-reused 0

Unpacking objects: 100% (3/3), done.

From https://github.com/dolonche/sdt-lab02

   9051876..094d25c  master     -> origin/master

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git log

commit 4ba8e608cf1be02913402a0b34ea70ad57fb9a3b

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 10:16:20 2018 +0300

　

    добавил комментарий в файл main.cpp

　

commit 905187614d3dade491139f3ba4e616d29117b681

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 10:06:04 2018 +0300

　

    добавил вывод первго числа, умноженного на два

　

commit 30db0455b2e6fdfe02c42d756700d7dc625ec6b6

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:49:22 2018 +0300

　

    добавил файлы, которые будут игнорироваться при пуше

　

commit 14efa8bfc0d080c4a52e1b28e0ee14cb3840c4fb

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:46:51 2018 +0300

　

    добавил вывод суммы введенных чисел

　

commit 67bf3137384226987ece6f64f2757c67e05a2e23

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:44:56 2018 +0300

　

    добавил программу ввода двух чисел

　

commit fb6f1cc69806cb4a0edf748dafc8b8132da84ef8

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:41:12 2018 +0300

　

    добавил файл CMakeLists.txt

　

commit 5fac16ba88d531368430fbd930991b0d5edc9ada

Author: Питенин Иван <ivan.pitenin@gmail.com>

Date:   Tue Mar 6 09:39:30 2018 +0300

　

    создал проект и добавил файл main.cpp

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git rebase origin/master

First, rewinding head to replay your work on top of it...

Applying: добавил комментарий в файл main.cpp

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "преобразовал локальные фалйы"

On branch master

Your branch is ahead of 'origin/master' by 1 commit.

  (use "git push" to publish your local commits)

Untracked files:

        .idea/

        cmake-build-debug/

　

nothing added to commit but untracked files present

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git status

On branch master

Your branch is ahead of 'origin/master' by 1 commit.

  (use "git push" to publish your local commits)

Untracked files:

  (use "git add <file>..." to include in what will be committed)

　

        .idea/

        cmake-build-debug/

　

nothing added to commit but untracked files present (use "git add" to track)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git pull

Already up-to-date.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git pull originn master

fatal: 'originn' does not appear to be a git repository

fatal: Could not read from remote repository.

　

Please make sure you have the correct access rights

and the repository exists.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git pull origin master

From https://github.com/dolonche/sdt-lab02

 * branch            master     -> FETCH_HEAD

Already up-to-date.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git fetch

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git rebase origin/master

Current branch master is up to date.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git status

On branch master

Your branch is ahead of 'origin/master' by 1 commit.

  (use "git push" to publish your local commits)

Untracked files:

  (use "git add <file>..." to include in what will be committed)

　

        .idea/

        cmake-build-debug/

　

nothing added to commit but untracked files present (use "git add" to track)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git push

Username for 'https://github.com': dolonche

Counting objects: 3, done.

Delta compression using up to 2 threads.

Compressing objects: 100% (3/3), done.

Writing objects: 100% (3/3), 397 bytes | 0 bytes/s, done.

Total 3 (delta 2), reused 0 (delta 0)

remote: Resolving deltas: 100% (2/2), completed with 2 local objects.

To https://github.com/dolonche/sdt-lab02.git

   094d25c..7ae7fad  master -> master

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ cd /c/Users/u211-05/Desktop/labslab02RepoB

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ git pull

remote: Counting objects: 3, done.

remote: Compressing objects: 100% (1/1), done.

remote: Total 3 (delta 2), reused 3 (delta 2), pack-reused 0

Unpacking objects: 100% (3/3), done.

From https://github.com/dolonche/sdt-lab02

   094d25c..7ae7fad  master     -> origin/master

Updating 094d25c..7ae7fad

Fast-forward

 main.cpp | 2 +-

 1 file changed, 1 insertion(+), 1 deletion(-)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ git pull --ff-only

Already up-to-date.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoB (master)

$ cd /c/Users/u211-05/Desktop/labslab02RepoA

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git checkout -b division HEAD~1

error: Your local changes to the following files would be overwritten by checkout:

        main.cpp

Please commit your changes or stash them before you switch branches.

Aborting

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "именил программу на основании пункта 5.1"

[master fb47673] именил программу на основании пункта 5.1

 1 file changed, 11 insertions(+), 8 deletions(-)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git checkout -b division HEAD~1

Switched to a new branch 'division'

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (division)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (division)

$ git commit -m "заменил умножение делением"

[division f5542a6] заменил умножение делением

 1 file changed, 9 insertions(+), 7 deletions(-)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (division)

$ git checkout master

Your branch is ahead of 'origin/master' by 1 commit.

  (use "git push" to publish your local commits)

Switched to branch 'master'

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git merge division

Auto-merging main.cpp

CONFLICT (content): Merge conflict in main.cpp

Automatic merge failed; fix conflicts and then commit the result.

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master|MERGING)

$ git status

On branch master

Your branch is ahead of 'origin/master' by 1 commit.

  (use "git push" to publish your local commits)

You have unmerged paths.

  (fix conflicts and run "git commit")

  (use "git merge --abort" to abort the merge)

　

Unmerged paths:

  (use "git add <file>..." to mark resolution)

　

        both modified:   main.cpp

　

Untracked files:

  (use "git add <file>..." to include in what will be committed)

　

        .idea/

        cmake-build-debug/

　

no changes added to commit (use "git add" and/or "git commit -a")

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master|MERGING)

$ git add main.cpp

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master|MERGING)

$ git commit -m "решаю конфликты"

[master e575f49] решаю конфликты

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "решаю конфликты x2"

[master 5fb7ee0] решаю конфликты x2

 1 file changed, 1 insertion(+), 3 deletions(-)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git status

On branch master

Your branch is ahead of 'origin/master' by 4 commits.

  (use "git push" to publish your local commits)

Untracked files:

  (use "git add <file>..." to include in what will be committed)

　

        .idea/

        cmake-build-debug/

　

nothing added to commit but untracked files present (use "git add" to track)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git push origin master

Username for 'https://github.com': dolonche

Counting objects: 12, done.

Delta compression using up to 2 threads.

Compressing objects: 100% (12/12), done.

Writing objects: 100% (12/12), 1.25 KiB | 0 bytes/s, done.

Total 12 (delta 8), reused 0 (delta 0)

remote: Resolving deltas: 100% (8/8), completed with 1 local object.

To https://github.com/dolonche/sdt-lab02.git

   7ae7fad..5fb7ee0  master -> master

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git add -u

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git commit -m "дорешал конфликт"

[master c2ee41f] дорешал конфликт

 1 file changed, 1 insertion(+), 4 deletions(-)

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git push origin master

Username for 'https://github.com': dolonche

Counting objects: 3, done.

Delta compression using up to 2 threads.

Compressing objects: 100% (3/3), done.

Writing objects: 100% (3/3), 329 bytes | 0 bytes/s, done.

Total 3 (delta 2), reused 0 (delta 0)

remote: Resolving deltas: 100% (2/2), completed with 2 local objects.

To https://github.com/dolonche/sdt-lab02.git

   5fb7ee0..c2ee41f  master -> master

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$ git log --decorate --oneline --graph

* c2ee41f (HEAD -> master, origin/master) дорешал конфликт

* 5fb7ee0 решаю конфликты x2

*   e575f49 решаю конфликты

|\

| * f5542a6 (division) заменил умножение делением

* | fb47673 именил программу на основании пункта 5.1

|/

* 7ae7fad добавил комментарий в файл main.cpp

* 094d25c добавил печать разности введенных элементов

* 9051876 добавил вывод первго числа, умноженного на два

* 30db045 добавил файлы, которые будут игнорироваться при пуше

* 14efa8b добавил вывод суммы введенных чисел

* 67bf313 добавил программу ввода двух чисел

* fb6f1cc добавил файл CMakeLists.txt

* 5fac16b создал проект и добавил файл main.cpp

　

u211-05@UII-15 MINGW64 ~/Desktop/labslab02RepoA (master)

$
