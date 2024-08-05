@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank $ git config --global user.name "Alan Lira"
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank $ git config --global user.email "alan.lira@aluno.impacta.com.br"
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank $ mkdir exercicio
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank $ cd exercicio/
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio $ git init
Initialized empty Git repository in /workspaces/codespaces-blank/exercicio/.git/
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ cd .git/
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio/.git (main) $ ls -a
.  ..  HEAD  branches  config  description  hooks  info  objects  refs
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio/.git (main) $ cd ..
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ echo "teste" > README.md
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ ls
README.md
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git add .
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ echo 01 > arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ ls
README.md  arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        arquivo.txt

@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git add .
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
        new file:   arquivo.txt

@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git commit -m "git add example - arquivo.txt"
[main (root-commit) f37e162] git add example - arquivo.txt
 2 files changed, 2 insertions(+)
 create mode 100644 README.md
 create mode 100644 arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main
nothing to commit, working tree clean
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ echo 02 > arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ ls
README.md  arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git log
commit f37e162a7eff5061a9d5b04e21f3b05291469c00 (HEAD -> main)
Author: Alan Lira <alan.lira@aluno.impacta.com.br>
Date:   Sun Aug 4 23:23:11 2024 +0000

    git add example - arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git add arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git diff
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git diff arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ echo 03 > arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git restore arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git commit -m "commit ex K  > arquivo.txt 
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git log
commit 6eee80ead50f87f75ed73215d5d64dd07335ec5b (HEAD -> main)
Author: Alan Lira <alan.lira@aluno.impacta.com.br>
Date:   Sun Aug 4 23:44:59 2024 +0000

    commit ex K

commit f37e162a7eff5061a9d5b04e21f3b05291469c00
Author: Alan Lira <alan.lira@aluno.impacta.com.br>
Date:   Sun Aug 4 23:23:11 2024 +0000

    git add example - arquivo.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ vi .gitignore
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ cat .gitignore 
*.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ echo "testando o gitignore" > teste.txt
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

no changes added to commit (use "git add" and/or "git commit -a")
@AlanDiegoBatistadelira ➜ /workspaces/codespaces-blank/exercicio (main) $ 
