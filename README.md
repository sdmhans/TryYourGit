# TryYourGit

本仓库用于课堂Git实验，目的是让同学们能以较快的速度掌握借助于git和Github的基本使用，以此更好地管理大作业的项目相关文件。

## Task 1

请认真听讲。

## Task 2

请Fork本仓库。

## Task 3

请将Fork的仓库clone到你的本机，然后基于signin分支的最新commit，创建一个名为你的学号的新分支，比如学号为2011013236的同学，需要创建一个分支并命名为2011013236，以下简称该分支为学号分支。

```
git clone https://github.com/ThssSE/TryYourGit.git
cd TryYourGit
```

## Task 4

切换至学号分支，在SignIn目录中创建一个新文件，命名为“你的学号.txt”，比如学号为2011013236的同学，需要创建的文件是“2011013236.txt”，文件内容为也为你的学号。

将新添加的文件加入版本库，使之被暂存（staged）。

```
git checkout signin
git checkout -b 201533333
echo 201533333 > SignIn/201533333.txt
git add SignIn/201533333.txt
```

## Task 5

提交一个Commit，该commit中仅包含新添加的那一个txt文件。

完成提交后，把学号分支push到你的Fork仓库去。

```
git commit -m "Task 5"
git push -u origin 201533333
```

## Task 6

提交一个Pull-Request请求到 https://github.com/ThssSE/TryYourGit ，将学号分支提交给该主版本库的signin分支。

//在github页面操作

如果没有出现conflicts，恭喜！

## Warm Prompt

以上练习作为课堂签到，望周知。

完成以上6个Task将得到100%的签到分。如果没有完成前5个Task将视作没有签到。如果提交给主版本库signin分支的不是学号分支，你得到的签到分将乘以系数0.5。学号分支提交的txt文件名或内容不符合要求，签到分也将乘以系数0.5。