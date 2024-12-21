# Gym-Git-Exercise-Solutions

# Bundle1
## Exercise1

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~$ mkdir Gym_Git_Exercises
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~$ git init
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~$ echo "# Gym-Git-Exercise-Solutions" >> README.md
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~$ git branch -M main
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~$ git add README.md 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~$ git commit -m "First commit"
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~$ git remote add origin https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~$ git push -u origin main
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git branch dev
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout dev
M	README.md
Switched to branch 'dev'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git branch
* dev
  main
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git branch test
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git branch -d test
Deleted branch test (was 608ce99).
```

## Exercise2

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add home.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git stash 
Saved working directory and index state WIP on main: 1277fe5 changes
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add about.html
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git stash 
Saved working directory and index state WIP on main: 1277fe5 changes
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add team.html
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git stash 
Saved working directory and index state WIP on main: 1277fe5 changes
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (0ac2ccfe6a70b4b0faa748cb58163d9ea9766eba)
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped stash@{1} (2d9be56b05f17add34498bef92adf6ce79b5458c)
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "Exercise2"
[main d84820e] Exercise2
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 about.html
 ```

 ```bash
 mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git stash pop
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git reset --hard
HEAD is now at d84820e Exercise2
```

# Bundle2
## Exercise1

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git branch ft/bundle-2
```
```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git branch
  dev
  ft/bundle-2
  list
* main
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout ft/bundle-2 
Switched to branch 'ft/bundle-2'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add services.html
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "New file added"
[ft/bundle-2 8825fd3] New file added
 1 file changed, 16 insertions(+)
 create mode 100644 services.html
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push --set-upstream origin ft/bundle-2 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 508 bytes | 508.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Mugara250/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote: 
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```

# Bundle2
## Exercise2

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (2/2), 978 bytes | 978.00 KiB/s, done.
From https://github.com/Mugara250/Gym-Git-Exercise-Solutions
   b3acab2..fd0dd35  main       -> origin/main
Updating b3acab2..fd0dd35
Fast-forward
 services.html | 16 ++++++++++++++++
 1 file changed, 16 insertions(+)
 create mode 100644 services.html

````

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add services.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "changes on services.html"
[ft/service-redesign b02b751] changes on services.html
 1 file changed, 2 insertions(+)
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 340 bytes | 340.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Mugara250/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote: 
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add services.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "made changes on services.html"
[main d1bab90] made changes on services.html
 1 file changed, 2 insertions(+)

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 346 bytes | 346.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
   fd0dd35..d1bab90  main -> main
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout ft/service-redesign 
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git diff main
diff --git a/services.html b/services.html
index cbf2c93..2520312 100644
--- a/services.html
+++ b/services.html
@@ -11,8 +11,8 @@
         <li>Business consultancy</li>
         <li>Web development</li>
         <li>Graphic design</li>
-        <li>Cybersecurity</li>
-        <li>Data analytics</li>
+        <li>Digital marketing</li>
+        <li>Photography</li>
     </ol>
 </body>
 </html>
\ No newline at end of file
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add services.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "merged branch 'main' into 'ft/service-
redesign'"
[ft/service-redesign 33e25ed] merged branch 'main' into 'ft/service-redesign'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 380 bytes | 380.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
   b02b751..33e25ed  ft/service-redesign -> ft/service-redesign

```

# Bundle3
## Exercise1

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add team.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "added team.html"
[ft/team-page a532603] added team.html
 1 file changed, 17 insertions(+)
 create mode 100644 team.html
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 514 bytes | 514.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Mugara250/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote: 
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout ft/team-page 
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git log
commit a532603073d2b4f25a9e1acef6dc58f59fb33b0d (HEAD -> ft/team-page, origin/ft/team-page)
Author: Mugara250 <mbonyumugara52@gmail.com>
Date:   Thu Dec 19 12:02:36 2024 +0200

    added team.html

commit 33e25ed76fa58196b2925d692ca40208241cff42 (origin/ft/service-redesign, ft/service-redesign)
Merge: b02b751 d1bab90
Author: Mugara250 <mbonyumugara52@gmail.com>
Date:   Wed Dec 18 17:19:21 2024 +0200

    merged branch 'main' into 'ft/service-redesign'

commit d1bab909db445bccc97af3450f55ded80962102e (origin/main, main, ft/contact-page)
Author: Mugara250 <mbonyumugara52@gmail.com>
Date:   Wed Dec 18 16:58:59 2024 +0200

    made changes on services.html

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout ft/contact-page 
Switched to branch 'ft/contact-page'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git cherry-pick a532603073d2b4f25a9e1acef6dc58f59fb33b0d
[ft/contact-page a83e786] added team.html
 Date: Thu Dec 19 12:02:36 2024 +0200
 1 file changed, 17 insertions(+)
 create mode 100644 team.html
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add contact.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "added contact.html"
[ft/contact-page 30abed2] added contact.html
 1 file changed, 14 insertions(+)
 create mode 100644 contact.html
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push --set-upstream origin ft/contact-page 
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 994 bytes | 994.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Mugara250/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote: 
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add faq.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "added faq.html"
[ft/faq-page 5b58220] added faq.html
 1 file changed, 13 insertions(+)
 create mode 100644 faq.html
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push --set-upstream origin ft/faq-page 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 535 bytes | 535.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Mugara250/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote: 
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git log
commit 5b5822008a6d2bd1510668c421b086d28747c33f (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Mugara250 <mbonyumugara52@gmail.com>
Date:   Thu Dec 19 12:55:15 2024 +0200

    added faq.html

commit 30abed2d9f7dc3bfa92931100d245e917c5d5b74 (origin/ft/contact-page, ft/contact-page)
Author: Mugara250 <mbonyumugara52@gmail.com>
Date:   Thu Dec 19 12:44:26 2024 +0200

    added contact.html

commit a83e786121d1473f4f6630c74f9fb3964648c33a
Author: Mugara250 <mbonyumugara52@gmail.com>
Date:   Thu Dec 19 12:02:36 2024 +0200

    added team.html

commit d1bab909db445bccc97af3450f55ded80962102e (origin/main, main)
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git revert a83e786121d1473f4f6630c74f9fb3964648c33a
[ft/faq-page 97b693d] Revert "added team.html"
 1 file changed, 17 deletions(-)
 delete mode 100644 team.html

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 276 bytes | 276.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
   5b58220..97b693d  ft/faq-page -> ft/faq-page

```

# Bundle3
## Exercise2

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout ft/faq-page 
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add home.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "made changes in home.html"
[main 4fd586f] made changes in home.html
 1 file changed, 1 insertion(+)

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 362 bytes | 362.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
   7772d07..4fd586f  main -> main

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout ft/home-page-redesign 
Switched to branch 'ft/home-page-redesign'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add home.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "added more content to home.html"
[ft/home-page-redesign 25c85bd] added more content to home.html
 1 file changed, 3 insertions(+)

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 431 bytes | 431.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Mugara250/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote: 
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
```

# Bundle4
## Exercise1

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git remote add git-copy https://github.com/Mugara250/
gym-git-exercises.git
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git remote
git-copy
origin
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add home.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "added more content to home.html"
[main 8b440d9] added more content to home.html
 1 file changed, 15 insertions(+), 9 deletions(-)
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 511 bytes | 511.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
   ec61b03..8b440d9  main -> main

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push origin
Everything up-to-date
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push git-copy 
Enumerating objects: 91, done.
Counting objects: 100% (91/91), done.
Delta compression using up to 8 threads
Compressing objects: 100% (85/85), done.
Writing objects: 100% (91/91), 17.09 KiB | 1.00 MiB/s, done.
Total 91 (delta 39), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (39/39), done.
To https://github.com/Mugara250/gym-git-exercises.git
 * [new branch]      main -> main

```

# Bundle4
## Exercise2

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add faq.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "added more content to faq.html"
[ft/footer 49b88b7] added more content to faq.html
 1 file changed, 1 insertion(+)

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add contact.html 
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "added more content to contact.html"
[ft/footer 1008be9] added more content to contact.html
 1 file changed, 2 insertions(+), 1 deletion(-)

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push --set-upstream origin ft/footer
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 703 bytes | 703.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 3 local objects.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Mugara250/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote: 
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git merge --squash ft/footer
Updating 284a83b..1008be9
Fast-forward
Squash commit -- not updating HEAD
 contact.html | 3 ++-
 faq.html     | 1 +
 2 files changed, 3 insertions(+), 1 deletion(-)

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git commit -m "footer changes squashing"
[ft/squashing 6b6f84a] footer changes squashing
 2 files changed, 3 insertions(+), 1 deletion(-)

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git push --set-upstream origin ft/squashing
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 468 bytes | 468.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
remote: 
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/Mugara250/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote: 
To https://github.com/Mugara250/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.
```

# Bundle5
## Exercise1

Link to the Github pages of the repo: https://mugara250.github.io/Gym-Git-Exercise-Solutions/

# Bundle5
## Exercise2

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Desktop/THE_GYM$ git clone https://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@github.com/Mugara250/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 92 (from 1)
Receiving objects: 100% (107/107), 1.95 MiB | 410.00 KiB/s, done.
Resolving deltas: 100% (5/5), done.
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Desktop/THE_GYM/git-cafe-exercise$ git add index.html
```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Desktop/THE_GYM/git-cafe-exercise$ git commit -m "changed the h2 title inside index.html"
[main 0b71bf9] changed the h2 title inside index.html
 1 file changed, 1 insertion(+), 1 deletion(-)

```

```bash
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Desktop/THE_GYM/git-cafe-exercise$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 338 bytes | 338.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Mugara250/git-cafe-exercise.git
   d1d3f9c..0b71bf9  main -> main

```