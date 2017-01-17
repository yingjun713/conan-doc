# 可能遇到的问题

1.在执行sudo npm run conan 的之后可能会遇到下图所示问题：

![](/assets/报错1.png)

解决方法：

查看有没有这个目录

```
cd /Library/Google/Chrome
```

如果有，直接在该目录下新建文件夹

```
sudo mkdir NativeMessagingHosts
```

如果没有这个目录，直接手动新建这个目录

```
sudo mkdir -p /Library/Google/Chrome/NativeMessagingHosts
```

2./var/log/conan的权限不对

解决方法：

先查询当前用户的权限

```
who am i
```

结果如下图所示：

![](/assets/log权限.png)

再查当前用户所属的用户组\(账户名例如：sherr\) groups michaelzhao

```
groups sherry
```

结果如下图所示：

![](/assets/q2.png)

再更改/var/log/conan的用户组

```
sudo chown -R sherry:staff /var/log/conan
```

3.chrome最新版本，安装了conan插件后，关闭浏览器，下次打开后，就会提示conan被禁用，就需要重新安装。

解决方法：

