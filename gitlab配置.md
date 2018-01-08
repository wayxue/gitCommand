# 同时使用github和gitlab的方法
1. 生成gitlab秘钥
    ssh-keygen -t rsa -C "email"                                
    重新指定生成秘钥的名称，地址不变
2. 在.ssh 文件夹下添加 config 文件，内容：                                
    #github   
    Host github     
        HostName github.com                   
        IdentityFile ~/.ssh/id_rsa                   
    #gitlab   
    Host gitlab  
        HostName gitlab.com  
        IdentityFile ~/.ssh/gitlab_id_rsa
3. 初始化     
    git config --local user.name "gitlab用户名"    
    git config --local user.email "email"
