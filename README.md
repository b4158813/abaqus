# abaqus
abaqus 安装bug

## 问题1：安装完成后找不到从哪打开abaqus软件？！
**解决方法：按以下步骤来**

 找到安装目录下的abq6144.bat批处理文件，如下图所示
 
![比如我是安装在这个目录下的](https://img-blog.csdnimg.cn/20190902225506236.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)

 右击->发送到->桌面快捷方式，在桌面上找到这个快捷方式，右击->属性
 
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/2019090222565167.png)
 
 在“目标”这一栏后面加上 “ cae||pause” ，点击确定
 
 ![](https://img-blog.csdnimg.cn/20190902225902623.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902230117637.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)
 
 这样就可以啦！双击运行吧！
 （运行时会弹出来一个命令提示符窗口，如下图所示，等会儿就成功啦）
 
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902230227867.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)
 
 出来这个界面就表示成功啦
 
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902230416393.png)

## 问题2：按照问题1的解决步骤进行，最后出现的却是这个界面？！

> ![这里是引用](https://img-blog.csdnimg.cn/20190902230545937.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)


***这说明你没有启动license的server***
**解决方法：去启动一下就完事儿了**
打开你放license的文件目录，启动Imtools.exe![比如我是这里](https://img-blog.csdnimg.cn/20190902230759781.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)
按如图所示依次点击（这里默认你的证书文件设置都是正确的），然后关闭，再去启动辣个快捷方式即可！
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902230923237.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)

## 问题3：按照问题1的解决步骤进行，最后出现的却是这个界面？！
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902231312207.png)

*****这说明你的abq6144.bat内文件路径的设置有问题（即没有连接上主程序）*****
**解决方法：把路径改成正确的abq6144.bat路径就行了**

找到abq6144.bat文件，右击->编辑
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902231515117.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)
改正错误的文件路径（比如我这里sb乱入错导致，应该是Abaqus）
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902231605289.png)
改成自己正确的文件路径之后：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902231729477.png)
保存关闭即可


## 问题4：按照问题1的解决步骤进行，最后弹出这个界面？！

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902231939727.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)

解决方法：[教您快速解决丢失mfc100u.dll组件的问题](https://jingyan.baidu.com/article/c45ad29c0a61f9051753e2ef.html)


若在上述操作中出现了如下问题：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190902232303763.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)
参考以下解决方案：[mfc100u.dll加载失败解决方案](https://jingyan.baidu.com/article/ad310e80f8cef91848f49e74.html)


> **最后，如果觉得文件的图标不好看，可以考虑修改（右击->属性->更改图标->浏览->按如下路径找到图标即可）![我是这样的](https://img-blog.csdnimg.cn/20190902232642861.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDA0MjY0Mw==,size_16,color_FFFFFF,t_70)


