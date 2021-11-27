# Python,From here to start(WinOS)

## 部署Python

### 安装Python

> 如果已经由VisualStutio或Anaconda安装
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
> ```
> 



> pip
>
> ```
> pip --help
> 
> pip list
> pip install [PackageName]
> ```
> 

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

### Issues

#### 删除过长的Prcharm右键菜单

> 删除注册表中整个PyCharm文件夹(可能是带Community的)
>
> > 计算机\HKEY_CLASSES_ROOT\Directory\Background\shell\PyCharm
> >
> > 计算机\HKEY_CLASSES_ROOT\Directory\shell\PyCharm



