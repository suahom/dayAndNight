# 构建git仓库且与远程相连接

- 本地构建git

   `git init`

  

- 在github构建仓库

  直接在远程构建仓库即可，主要复制仓库的地址

- 如果远程已经有ssh key 了，则进行下一步，否则按照如下步骤进行

  - 形成密钥

    `ssh-keygen`

  - 将密钥传到github上

- 关联两个库

  `git remote add origin git@github.com:suahom/dayAndNight.git`

- 与远程进行关联

  - 如果远程没有建立分支

    `git push --set-upstream origin master`

  - 如果远程以及构建了分支

    `git branch --set-upstream-to=origin/<branch> master`

- 在本地建立文件，进行操作，然后添加到库，然后提交，然后推送，并同时可以从远程拉取

  `touch 88.txt`

  `git add . `

  `git commit -m 构建了88.txt文件`

  `git push`

  `git pull`







```

```