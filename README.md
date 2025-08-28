# cs61b-sp21
本项目主要用于记录学习UC Berkeley的cs61a的spring21课程的作业提交和操作指南。
# Preparations
首先，在Git bash中运行<br>
`ssh -T git@github.com`<br>
连接到github（要先在github中获取一个ssh）,当看到如下内容<br>
`Hi USERNAME! You've successfully authenticated, but GitHub does not provide shell access.`<br>
我们就顺利连接github了。<br>
其次，我们可以前往课程主页[cs61b-sp21](https://sp21.datastructur.es/)以创建一个github仓库储存作业代码，然后我们要将其与远程仓库skeleton联系起来，运行以下代码<br>
`git remote add skeleton https://github.com/Berkeley-CS61B/skeleton-sp21.git`<br>
然后运行(如果master不行可改成main)<br>
`git pull skeleton master`<br>
将作业代码拉取到自己的仓库中。这里要注意，如果出现拒绝拉取代码的情况，运行<br>
`git pull skeleton master --allow-unrelated-histories`<br>
就能解决此问题。<br>
此时，当我们打开作业文件时，我们会发现有些java文件下端有红波浪线，这是因为没有配置好。我们要先拉取一个library24文件夹（最好不要将其放在自己的仓库文件夹中）<br>
`git clone https://github.com/Berkeley-CS61B/library-sp24`<br>
在IntelliJ中打开File -> Project Structure-project选项，SDK中点击Download并下载1.8的版本，Language Levels选择8开头的版本。然后在library选项中点击左上角的+，选择之前的library24文件夹。<br>
对于提交作业，我们只需注意每次完成一个小任务就将change的文件commit上去，最后完成任务时，运行<br>
`git push origin main`<br>
将commits从本地仓库推送到远程仓库去，这时我们就能在github上看到更改了，再用gradescope评分即可。<br>
## lab2
该lab主要是教会我们运用Debugger工具找出每个文件的bugs。


