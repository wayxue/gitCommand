# 简单介绍git与GitHub的使用
1. 使用git-bash.exe 设置用户名和邮箱,命令：            
    git config --global user.name "wayxue"          
    git config --global user.email "email"
2. 生成SSH Key,命令：           
    ssh-keygen -t rsa -C "邮箱"
3. 获取.ssh下的id_rsa.pub文件中的内容，复制到GitHub Personal setting -> SSH Keys 中。
4. 测试ssh key是否成功，使用命令“ssh -T git@github.com”，如果出现You’ve successfully authenticated, but GitHub does not provide shell access 。这就表示已成功连上github。
5. 获取GitHub上的工程（仓库）,命令：            
    git clone 仓库地址。(HTTP地址，SHH不好使)
6. 拉取仓库中的内容,命令：                                         
    git pull origin master
7. 本地创建text.txt，命令：                   
    git add text.txt                             
    git commit -m "add a new file"                       
    git push origin master                     
    这样就可以在GitHub上同步看到了。
8. 另外，个人感觉git-bash.exe 中的命令与linux命令很相似。
# 如何创建一个仓库
1. 在GitHub上新建一个仓库，复制地址，克隆到本地。
2. 在本地添加需要上传的代码。
3. git add .
4. git commit -m "instruction"
5. git push origin master
