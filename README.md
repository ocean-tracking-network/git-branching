# Git Branching

Branches are a pointer to a snapshot in the development of code. Branches can point to versions with new features,
fixes to bugs/issues, or stable versions. Looking at this branching model we can see very distinct branches on
the vertical axis.


![Git BRanching Model](images/git-model.png)
*Source:https://nvie.com/posts/a-successful-git-branching-model/*


To create a new branch on this repo we first need to clone it:
```bash
git clone https://github.com/ocean-tracking-network/2019-05-29-git-branching.git
```

Next, let's checkout what branches are available already:
```bash
git branch -r
```

We can see there is a development branch, let's get that one:
```bash
git checkout develop
```

We can see there is a development branch, let's get that one:
```bash
git checkout develop
```

Let's create a new branch, from develop:
```bash
git checkout -b <new branch name> develop
```

Check which branch you are currently on, make sure it's our new one:
```bash
git branch
```

Next, create a new file in this branch:
```bash
echo "echo <your name>" > <your_name>.sh
```

Add and commit your changes, then push your changes:
```bash
# Code to add changes
# Code to commit changes
git push -u origin <new branch name>
```
