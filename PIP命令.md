# PIP3命令

## **pip**命令介绍

> python是最近几年特别火的编程语言，经常会用到pip这个工具，用来安装相关的依赖库，也可以查询相关信息。python有版本2和版本3的区别，同样pip命令也有pip与pip3的区别，版本更新了而已。

## pip命令的安装与卸载

- 安装

> - 直接到官网下载pip安装包，然后解压，之后输入`python setup.py  install`命令
> - 在安装python环境的时候，安装过程中会有选项是否安装pip安装包，直接勾选就有了

- 卸载

>  **python -m pip uninstall pip** 

## pip命令安装依赖库

```c
//命令格式
pip3 install name(就是你要安装的第三方依赖库的名称)
```

**注意**

pip命令默认安装源是https://pypi.python.org/simple/,即从官网下载，网速较慢。可以采用国内比较知名的安装源：

- 阿里云 http://mirrors.aliyun.com/pypi/simple/
- 中国科技大学 https://pypi.mirrors.ustc.edu.cn/simple/
- 豆瓣 http://pypi.douban.com/simple
- v2ex http://pypi.v2ex.com/simple/
- 中国科学院 http://pypi.mirrors.opencas.cn/simple/
- 清华大学 https://pypi.tuna.tsinghua.edu.cn/simple/ 

```shell
//使用格式,一般豆瓣的安装源下载速度比较快
pip install 库名 -i https://pypi.tuna.tsinghua.edu.cn/simple
```

## pip命令的使用

- 使用pip3的时候可能出现下面这种情况

![python-1](https://github.com/hello-sources/Relative_Things/blob/master/img/Python_img/python-1.png?raw=true)

表示有新版本，根据提示输入下面格式即可

```shell
pip3 install --upgrade pip
```

<img src="https://github.com/hello-sources/Relative_Things/blob/master/img/Python_img/python-2.png?raw=true" alt="python-2" style="zoom:80%;" />

之后使用,即可看到对应版本

```shell
pip show pip
```

<img src="https://github.com/hello-sources/Relative_Things/blob/master/img/Python_img/python-3.png?raw=true" alt="python-3" style="zoom:80%;" />





## Linux下pip命令安装与更新

- 安装

```shell
sudo apt-get install python-pip
sudo apt-get install python-pip3
```

- 升级

```shell
sudo pip install --upgrade -i 国内源地址 pip
 sudo pip3 install --upgrade -i 国内源地址 pip
```

