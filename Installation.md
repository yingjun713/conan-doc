# Installation

conan是一个UI自动化测试工具，是浏览器的一个插件，由于没有进入浏览器的应用商店，所以安装起来，步骤想对来说要多一些；下文将阐述如何安装Conan。

1.安装node。先确认自己的机子是否安装了node，如果安装了可以跳过这一步骤；若没有，就需要先安装，可以直接从官网上下载，网址：[https://nodejs.org/en/](https://nodejs.org/en/)，或者直接使用brew安装：

```
brew install node
```

2.安装浏览器驱动。可以安装多个浏览器驱动。下面是几个常用的：

chromedriver  安装方式： 直接解压后将chromedriver执行文件放到/usr/local/bin目录下

```
[https://attachments.tower.im/tower/0b7e2fa4b2ef43de9afecb4cd050049b?download=true&filename=chromedriver\_mac64.zip](https://attachments.tower.im/tower/0b7e2fa4b2ef43de9afecb4cd050049b?download=true&filename=chromedriver_mac64.zip)
```

safaridriver    安装方式： 直接执行SafariDriver.safariextz

```
[https://attachments.tower.im/tower/4712449284444a36a389ebeeabf6c923?download=true&filename=SafariDriver.safariextz](https://attachments.tower.im/tower/4712449284444a36a389ebeeabf6c923?download=true&filename=SafariDriver.safariextz)
```

operadriver    安装方式：直接解压后将operadriver执行文件放到/usr/local/bin目录下

```
[https://attachments.tower.im/tower/cdebd994ba0e4943b359c8dd48d20135?download=true&filename=operadriver\_mac64.zip](https://attachments.tower.im/tower/cdebd994ba0e4943b359c8dd48d20135?download=true&filename=operadriver_mac64.zip)
```

phatomjs       安装方式： 直接解压后将bin下的phantomjs执行文件放到/usr/local/bin目录下

```
[https://attachments.tower.im/tower/c7267e0a831a4c25970a7f8b907ca435?download=true&filename=phantomjs-2.1.1-macosx.zip](https://attachments.tower.im/tower/c7267e0a831a4c25970a7f8b907ca435?download=true&filename=phantomjs-2.1.1-macosx.zip)
```

3.从git上clone conan 的项目，git地址：git@git.terminus.io:production/conan.git

```
git clone git@git.terminus.io:production/conan.git
```

若没有安装git，先安装git：

```
brew install git
```

4.打开clone下来的项目，将conan/extension/build.crx 文件拖到chrome的管理界面[chrome://extensions/ ](chrome://extensions/)，确认打开了develop mode，勾选该插件后的enable，添加成功之后，在浏览器的右上角会有一个插件的图标，如下图所示。最后复制该插件的ID。

![](/assets/extension.png)

5.

