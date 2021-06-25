jekyll new [projectName]

cd ./website/lab4

bundle exec jekyll serve 

bundle add webrick // cannot load such file -- webrick (LoadError)





发布：



git init

git checkout -b gh-pages

git status





```Shell
git init
git status
git add . 
git commit -m "initial commit"
# 从最开始创建的新GitHub repo页面，复制项目网址，粘贴到下面网址部分
git remote add origin https://github.com/USER-NAME/USER-NAME.github.io.git 
git push -u origin master
```

在输入以上最后一条指令后，也许会出现 `fatal: unable to access 'https://github.com/USER-NAME/USER-NAME.github.io.git': The requested URL returned error: 403` 这样的错误信息，这是权限的问题，可以尝试输入以下指令来解决：

```
git remote set-url origin https://USER-NAME@github.com/USER-NAME/USER-NAME.github.io.git
# 检查刚刚输入的那串url是否在这儿出现了
git remote -v
# 重新 push 一次，此时需要输入你的GitHub账号密码
git push -u origin master
# 确认刚刚提交的改动是否出现在日志里
git log
```



```Shell
git commit -m "initial commit"
```













git init

git status

git add .

git commit -m "test"

 git push origin gh-pages

