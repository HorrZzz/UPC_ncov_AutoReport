# windows平台Nodejs环境，实现报表自动提交
>因最近云函数开始收费了,本人无法使用[@tienskowl](https://github.com/tienskowl)大佬的脚本利用云函数创建自动提交项目,故而琢磨了一下Windows平台下Nodejs环境运行的方法分享出来.
## 免责声明
此脚本仅供参考学习，本人不对本脚本产生的任何影响负责。

请于下载本脚本之后24小时内彻底删除本脚本。

下载本脚本即视为同意此免责声明。
## Version 3.0
不再需要手动配置表单数据,现在可以实现不改动代码即可修改自动提交的数据

---
## 操作步骤
### ①Windows下配置Nodejs环境
[下载Nodejs12.16.0安装包并安装](https://nodejs.org/dist/v12.16.0/node-v12.16.0-x64.msi) 

[下载仓库源码并解压](https://github.com/HorrZzz/UPC_ncov_AutoReport/archive/refs/heads/HorrZzz-windows_Nodejs.zip)

打开解压的文件夹,在在文件夹空白处按住Shift+鼠标右键,`在此处打开Powershell窗口`输入`npm install`,安装所需依赖.
### ②代码文件准备
修改`Index.js`中的代码，使用上述准备的内容替换对应内容即可，修改完后打包即可。
### ③运行Run.bat文件
将index.js与Run.bat放在同一文件夹下，运行Run.bat文件即可。
### ④添加Windows计划任务
win+R,输入`taskschd.msc`运行计划任务;
按照下面的动图进行操作;
PS:启动程序-起始于一定要填脚本文件所在的文件夹绝对路径.
![pldeq.gif](https://s1.328888.xyz/2022/06/14/pldeq.gif)
	
