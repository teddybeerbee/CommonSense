​
通识类

#了解一些常见的软件项目文件夹命名
https://zhuanlan.zhihu.com/p/161640510

# WIN10如何在右下角显示到秒级别？
在電腦的工作列右側會顯示系统時間，往往只顯示到分，而想讓系统時間顯示到秒，操作方法如下：
方法\步骤：
 1、在Cortana搜尋輸入"regedit"，按Enter鍵進入登錄編輯程式；
2、搜尋路徑：HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\Advanced，新增DWORD（32位）值，重命名為”ShowSecondsInSystemClock”
3、修改數值資料為1
4、重新啟動explorer.exe(可按Windows鍵+R並在搜尋欄中輸入explorer or explorer.exe)
5、要想改回默認設置，直接刪除”ShowSecondsInSystemClock”登入值，重啟工作管理員即可。

Python

# python镜像源
https://pypi.tuna.tsinghua.edu.cn/simple
pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple

#Python 3.x | 史上最详解的 导入（import）
https://blog.csdn.net/weixin_38256474/article/details/81228492

#在python中如何设置当前工作目录
https://blog.csdn.net/weixin_30379911/article/details/96717461?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_baidulandingword~default-0.no_search_link&spm=1001.2101.3001.4242.1

# python路径拼接os.path.join()函数的用法
https://www.cnblogs.com/an-ning0920/p/10037790.html

# ​断网环境下利用pip安装Python离线安装包
https://zhuanlan.zhihu.com/p/22817250
# pip download与pip install简介
https://blog.csdn.net/happy_wealthy/article/details/116920402

# Python读取文件时出现UnicodeDecodeError: 'gbk' codec can't decode byte 0x80 in position xx: 解决方案
https://blog.csdn.net/zhang__shuang_/article/details/82527314

# Python按行读文件
https://www.cnblogs.com/xuxn/archive/2011/07/27/read-a-file-with-python.html

# python 字符串模糊匹配 Fuzzywuzzy
https://blog.csdn.net/weixin_41413177/article/details/90300139
https://www.cnblogs.com/traditional/p/12554215.html

# fuzzywuzzy完全指南，知乎有计算方式
https://zhuanlan.zhihu.com/p/437209647

# fuzzywuzzy github主页
https://github.com/seatgeek/thefuzz

# 在python中，在字符串中的每个字符后添加空格（python方法）
https://www.cnpython.com/qa/713551

# PyQt5 main函数
https://blog.csdn.net/H542723151/article/details/83586147

# Python按钮的响应事件详解
https://www.jb51.net/article/157328.htm

# python处理excel方式（openpyxl，xlrd，xlwt，openpyxl，panda）
https://blog.51cto.com/u_14320361/2493613

# Python基础-TypeError：takes 2 positional arguments but 3 were given
https://www.cnblogs.com/yswyzh/p/9558513.html

# 【python】代码换行的几种方法
https://blog.csdn.net/u014636245/article/details/87924595

# openpyxl：styles样式处理
https://www.jianshu.com/p/7af9a7c5b27d

# 利用openpyxl设置自动列宽（自适应列宽）
https://blog.csdn.net/crammy/article/details/120469646?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7Edefault-1.no_search_link&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7Edefault-1.no_search_link

# pip离线安装包
pip list #查看安装的包
pip freeze >requirements.txt
pip download （你的包名） -d"下载的路径（windows下双引号来表示文件夹)" （-r requirements.txt）
pip install --no-index --find-links=d:python27packages -r requirements.txt

# Python3通过chmod修改目录或文件权限的方法示例
# S_IRWXU等这些常量不知道为什么在我的os里没有，直接用数字代替可行，读写448，只读256
https://www.jb51.net/article/188262.htm

# matplotlib 生成的图像中无法显示中文字符的解决方法
https://www.jb51.net/article/188391.htm

# Python设置matplotlib.plot的坐标轴刻度间隔以及刻度范围
https://www.jb51.net/article/163842.htm
# 比较特殊的是，其中并没有对刻度值的字体进行设置的属性，所以我们需要使用下面两行进行设置，在最初使用plt.subplots中有得到一个返回值ax，我们使用ax.get_xticklabels()以及ax.get_yticklabels()来得到所有的刻度值，并使用set_fontname函数来设置属性。
https://blog.csdn.net/qq_40421671/article/details/109640106

# python多线程与多进程及其区别
https://www.cnblogs.com/yssjun/p/11302500.html

# PyQt5实时刷新
https://www.cnblogs.com/leoych/p/14450854.html

# 用python打包exe应用程序-PyInstaller
https://blog.csdn.net/bigzql/article/details/110944639?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522164208539916780357243160%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=164208539916780357243160&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_positive~default-1-110944639.pc_search_result_control_group&utm_term=pyinstaller&spm=1018.2226.3001.4187

打包有一个骚操作，若要将自己写的模块也使用pyinstaller打包到exe文件中，需要将自己写的模块复制到Python安装路径下的Lib\site-packages目录中。优化一下，把项目所有涉及到py代码的部分都复制到目录下。为了不和python维护的目录搞混，建议自己定义的package命名有明显标记。

pyinstaller --onefile main.py，实际上参数和-F一样，具体参见：
![微信图片_20220523130656](https://user-images.githubusercontent.com/46083193/169747570-e0487eb9-af9d-4359-916b-c96402dd1f26.png)


# Anaconda创建环境、删除环境、激活环境、退出环境
https://sleepingbug.blog.csdn.net/article/details/77370456?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7Edefault-1.no_search_link&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7ECTRLIST%7Edefault-1.no_search_link&utm_relevant_index=2

# python中怎么比较两个列表-Python3列表（list）比较
https://blog.csdn.net/weixin_37988176/article/details/109423397

# python解析json报错--json.decoder.JSONDecodeError: Unexpected UTF-8 BOM
https://www.cnblogs.com/muyuequzhi/p/13365823.html

C/C++

# MinGW-w64的安装及配置教程
https://blog.csdn.net/didi_ya/article/details/111240502

# win7旗舰版更新错误代码80072EFE怎么解决
各位我从百度知道里面解决的，下载了一个更新代理，有效 
https://docs.microsoft.com/zh-cn/troubleshoot/windows-client/deployment/update-windows-update-agent#automatically-download-windows-update-agent

# gets() 能读取含有空格的字符串，而 scanf() 不能

# vs典型错误1——错误严重性代码说明项目文件行禁止显示状态 错误C4996 'fopen': This function or variable may be unsafe
https://blog.csdn.net/qq_34706266/article/details/88941500

# 错误 C2371 “Cheer”: 重定义；不同的基类型
https://blog.csdn.net/qq_45418837/article/details/107125577?spm=1001.2101.3001.6650.6&utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-6.no_search_link&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-6.no_search_link

# C语言获取超大文件（超过2G）大小的功能
https://blog.csdn.net/codears/article/details/111405309


​
