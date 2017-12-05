---
title: Git工作中的使用
---
 
在这几个月实习中，参与了新媒体项目，用到了git。就我自己总结下来的一些git提交项目代码与解决冲突使用步骤。
   1，cd 文件夹  // 进入本地项目文件夹
   2，git pull    //更新项目代码     若出现Your local changes to the fllowing files would be overwriteen by merge:  则需要下面步骤；
        1, git stash    //退回上次提交的版本
		2, git pull     //重新一次更新项目代码
		3, git stash pop    //把本地原始修改的代码添加上   注意:出现绿色的代表添加上的   出现红色的代表冲突文件  解决办法；找到对应文件  用"===="或者">>>>"查找冲突地方  解决冲突
   3，git add . 或者 git add -A
   4, git commit -m '注释'
   5, git push
   