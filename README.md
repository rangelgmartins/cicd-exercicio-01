# cicd-exercicio-01

# Output dos comandos executados no exercicio-01:

**A.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ echo 01 > arquivo.txt

**B.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git add arquivo.txt
@rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   arquivo.txt

**C.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git commit -m "git add primeiro-commit - arquivo.txt"
[main a289616] git add primeiro commit - arquivo.txt
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo.txt

**D.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ echo 02 > arquivo.txt

**E.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git diff arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02

**F.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git add arquivo.txt
@rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

**G.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git diff --staged arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02

**H.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ echo 03 > arquivo.txt

**I.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git diff arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03

**J.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git restore --staged arquivo.txt

**K.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git commit -m "Update arquivo.txt"
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")

**L.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ vim .gitignore
@rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ cat .gitignore
*.txt

**M.** @rangelgmartins ➜ ~/cicd-exercicio-01 (main) $ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

no changes added to commit (use "git add" and/or "git commit -a")
