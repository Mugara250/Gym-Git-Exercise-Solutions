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