# Python,From here to start(WinOS)

## 部署Python

### 安装Python

> 如果已经由VisualStutio或Anaconda安装
>
> > 对于Anaconda
> >
> > 可能出现_ssl或squite3包无法装载的问题
> >
> > [win10中的import ssl报错处理_dally2的博客-CSDN博客](https://blog.csdn.net/dally2/article/details/103917604)
> >
> > 缺哪个补哪个
>
> 检查系统环境路径PATH是否已添加Python环境

### Python开发环境

#### IDE

> Pycharm
>
> Jupyter notebook
>
> VisualStudio

#### 包管理

> Anaconda-基于Conda
>
> Anaconda提供可视化程度高的包管理列表
>
> 据此进行安装包的查看,安装,更新,卸载等
>
> ```
> conda update conda
> #更新conda
> conda update --all
> #更新包
> 
> ```
> conda包换源
>
> ```
> conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
> 
> conda config --set show_channel_urls yes
> ```
>
> > 如果出现 `CondaHTTPError: HTTP 000 CONNECTION FAILED `
> >
> > 可以尝试转到 `C:\Users\[username]\.condarc` 把https换成http
> >
> > 并把-default删掉


> pip
>
> ```
> pip --help
> 
> pip list
> pip install [PackageName]
> ```
> pip包换源
>
> 修改或者创建C:\Users\用户名\pip\pip.ini文件
>
> ```
> [global]
> index-url = https://pypi.tuna.tsinghua.edu.cn/simple
> 
> #查看是否换源
> pip config l
> ```
>
> 其他可选择源：
> 阿里云 http://mirrors.aliyun.com/pypi/simple/
>
> 中国科技大学 https://pypi.mirrors.ustc.edu.cn/simple/
>
> 豆瓣(douban) http://pypi.douban.com/simple/
>
> 清华大学 https://pypi.tuna.tsinghua.edu.cn/simple/

## 使用VS2019运行Python项目

### 界面说明

> VS这个强大的IDE在python方面提供了许多窗口
>
> **在Python环境窗口中可以一站式访问所有窗口**
>
> - 初始化:生成Python应用程序
> - 在解决方案管理中可以变更Python环境-**尤其是使用Anaconda进行包管理**
> - Python命令行:直接在工具中打开PowerShell命令行就可以进入(~~不是什么交互窗口,那个是实例用的~~)
> - 工具-Python-交互窗口/交互中执行项目

### GoodByeVS-真有你的呵VS

```
交互窗口中发生内部错误。请重启 Visual Studio。
交互 Python 进程已退出。
交互窗口中发生内部错误。请重启 Visual Studio。
```

## Here we go! PyCharm

> [Download Community and FREE PyCharm: ](https://www.jetbrains.com/pycharm/download/#section=windows)

### Tips

> - Click twice `Shift` to open all-in-one SEARCHFUNC
> - Return to [Welcome to PyCharm]: File->Close Project
> - 文件名变红是这些文件还没有在git中提交
> - 官方插件库中有**中文插件**

### Issues

#### 删除过长的Prcharm右键菜单

> 删除注册表中整个PyCharm文件夹(可能是带Community的)
>
> > 计算机\HKEY_CLASSES_ROOT\Directory\Background\shell\PyCharm
> >
> > 计算机\HKEY_CLASSES_ROOT\Directory\shell\PyCharm

## JupyterNotebook

> 交互方式的工程形式
>
> 仅是进行数据科学计算、可视化用Jupyter也行
>
> ~~libiglPython库基本只能在Jupyter上跑了，写方法的时候就没写控制符导致本地跑还得改包函数~~
>
> [(50条消息) Jupyter更改默认路径_Miracle8070-CSDN博客_jupyter路径设置](https://blog.csdn.net/wuzhongqiang/article/details/89702046)
>
> > 路径替换为C:\\\Users\\\16708\\\source\\\JupyterProj	防止转义

插件：

- [打造实用的Jupyter Notebook 扩展插件 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/97394628)



