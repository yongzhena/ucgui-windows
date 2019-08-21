ucgui-windows
==========
https://blog.csdn.net/yyz_1987/article/details/99982912  
ucgui在windows上的移植  
使用方法:  
首先，windows上必须有GCC的环境。  
推荐安装mingwgcc  
我安装的是x86_64-810gcc-posix-seh-npMingw64v75.7z这个压缩包，直接解压。再配置环境变量即可。  
跟移植相关的，都在ucgui/GUI_X文件夹中。  
在ucgui/GUI文件夹中，有写好的makefile文件，直接make即可编译出libucgui.a库。  
然后需要把这个库放到GUIDemo_windows文件夹里。  
同时，里面有几个windows上需要依赖的库在里面。libGDI32.LIB,libWINMM.lib,   
同时多了两个文件MainTask.c和WinMain.c,其中windows程序的入口在WinMain.c中。  
这个里面也有一个makefile文件，可执行make命令，直接就生成了demo，test.exe可执行程序。   
# Author
yangyongzhen   
QQ:534117529  


