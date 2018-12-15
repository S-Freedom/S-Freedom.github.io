##通过cocosPod 引入第三方框架，并增加到代码仓库

###1.新建项目 testDemo

###2.进入终端到项目根目录下

###3在终端输入以下命令

（下面以AFN为例）
	搜索带 AFN 的第三方框架
	
	$ pod search AFN
创建 Podfile

	$ echo "pod 'AFNetworking'" > Podfile
 安装 Pod
 
    $ pod install
  4.将 CocoasPod 加入源代码管理
           
 		查看源代码库状态，红色部分是没有受源代码管理的文件 `?`
		$ git status

 将新添加的文件添加到源代码库管理
 
	$ git add .
    # 查看源代码库状态，绿色部分是加入源代码管理的文件 `A`
	$ git status

 提交修改，并且编写注释
 
	$ git commit -m "添加 AFN 框架"
	
 查看源代码库状态，nothing to commit, working directory clean 表示所有文件都已经提交至代码仓库管理
 
	$ git status