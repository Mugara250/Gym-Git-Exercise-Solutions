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
mugara@mugara-Lenovo-Yoga-C940-14IIL:~/Gym_Git_Exercises$ git add home.html
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