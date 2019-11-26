# pip相关

## pip基本命令

1. pip install [package-name]              # 安装名为[package-name]的包
2. pip install [package-name]==X.X         # 安装名为[package-name]的包并指定版本X.X
3. pip install [package-name] --proxy=代理服务器IP:端口号         # 使用代理服务器安装
4. pip install [package-name] --upgrade    # 更新名为[package-name]的包
5. pip install -i [URL] [package-name] # 从URL镜像下载名为[package-name]的包
6. pip uninstall [package-name]            # 删除名为[package-name]的包
7. pip list                                # 列出当前环境下已安装的所有包

## pip更换镜像源

### Windows10

直接在user目录中创建一个pip目录，如：C:\Users\xx\pip，然后新建文件pip.ini，即 %HOMEPATH%\pip\pip.ini，在pip.ini文件中输入以下内容（以清华镜像为例）：

```txt
[global]
index-url =  https://pypi.tuna.tsinghua.edu.cn/simple 
```

### Linux

 修改 ~/.pip/pip.conf (没有就创建一个文件夹及文件。文件夹要加“.”，表示是隐藏文件夹)
内容如下： 

```txt
[global]
index-url =  https://pypi.tuna.tsinghua.edu.cn/simple 
```

## 常见镜像源

（1）阿里云 http://mirrors.aliyun.com/pypi/simple/

（2）豆瓣http://pypi.douban.com/simple/

（3）清华大学 https://pypi.tuna.tsinghua.edu.cn/simple/

（4）中国科学技术大学 http://pypi.mirrors.ustc.edu.cn/simple/

（5）华中科技大学http://pypi.hustunique.com/