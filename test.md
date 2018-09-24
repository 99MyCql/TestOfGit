#微信小程序开发学习

###1、下载安装小乌龟TortoiseGit

####&nbsp;&nbsp;进入小乌龟官网，下载符合自己电脑版本的TortoiseGit，和汉化插件TortoiseGit-LanguagePack。点击安装，安装配置过程中，除了修改安装路径之外，全部默认配置即可。安装完TortoiseGit后，再安装汉化插件。
###2、了解GitHub项目
####&nbsp;&nbsp;airdb/index项目下有一个mkdocs.yml文件，该文件是一个将GitHub项目信息同步到(https://airdb.io)网站的配置文件。该文件中的pages:项之下的每条信息，都是一个文件的位置，对应网站菜单栏中的每一项。
###3、使用小乌龟下载、修改并上传GitHub项目
####&nbsp;&nbsp;（1）下载。新建一个存放GitHub项目的文件夹，在文件夹中点击右键，在右键菜单中选择Tortoise-clone（克隆）。将GitHub项目的地址(https://github.com/airdb/index)输入到出现窗口的URL地址中，然后在目录中选择新建文件夹的路径，最后确认即可。
####&nbsp;&nbsp;（2）修改。在下载好的index项目目录下，找到mkdocs.yml文件，并找到守护者对应的markdown文件 Maintainers.md。打开该文件，在airdb members中添加我的信息，保存。
####&nbsp;&nbsp;（3）提交。右键index项目文件夹，选择Tortoise-比较差异。通过差异的比较，确认自己的修改是否牵涉到意料之外的文件。确保无误之后，点击提交。在接下来出现窗口的日志信息中，写明这次改动的文件和相应事项，就可以提交了。
####&nbsp;&nbsp;（4）推送。推送之前还需要拉取，拉取的原因是，防止在你提交之前已经有人修改了项目文件。然后在进行推送，默认配置并点击确认之后，输入用户名密码，推送成功。
###4、下载node.js，再安装npm和vue
####&nbsp;&nbsp;（1）到node.js官网下载node.js。下载并安装成功后，在控制台输入：node -v ，查看node是否安装成功；输入：npm -v ，查看node自带的npm是否安装成功。
####&nbsp;&nbsp;（2）安装cnpm（中国版npm），控制台输入：npm install -g cnpm --registry=https://registry.npm.taobao.org 。
####&nbsp;&nbsp;（3）安装vue和vue-cli，控制台分别输入：cnpm install -g vue 和 cnpm install -g vue-cli 。（由于新版的vue-cli已经集成了webpack 所以下载了这个脚手架之后就不需要在下载webpack了）
###5、使用vue命令创建静态网站
####&nbsp;&nbsp;（1）在合适的地方新建一个vuejs文件夹。**控制台**进入该进入文件夹，并输入如下命令：vue init webpack test 。该命令新建一个vue项目，test是该项目的名字。输入之后，控制台会出现跳出一些询问，全部按下回车确认即可。
####&nbsp;&nbsp;（2）控制台进入vuejs/test目录下，依次输入：cnpm install 和 cnpm run dev。 成功之后再浏览器输入 localhost:8080 测试。
####&nbsp;&nbsp;（3）修改test/src/compoents/HelloWord.vue文件，修改并实现helloWord。
###6、下载微信开发工具，了解微信开发工具
####&nbsp;&nbsp;
###7、问题
####（1）为什么使用控制台生成的vue项目，有那么多文件，他们各自有什么作用呢？.vue是HTML的分离文件吗，该原理是什么？
####（2）为什么vue项目使用cnpm命令编译后，是在Tomcat容器上展现的？
####（3）推送GitHub项目失败，可能是因为新建了文件夹。
