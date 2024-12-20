# JDK 1.8.0_333 for Linux x86_64

## 资源说明
本仓库提供了Linux（适用于x86_64架构）平台上的Java Development Kit (JDK) 版本1.8.0_333的压缩包下载。此版本是Java开发的经典选择，广泛应用于各种服务器和开发环境中。

## 安装步骤

### 下载与解压
首先，您需要从本仓库下载`jdk1.8.0_333.x86_64-linux.tar.gz`文件。下载后，通过以下命令将其解压至合适的位置，例如 `/usr/local/java` 目录：

```shell
tar -zxvf jdk1.8.0_333.x86_64-linux.tar.gz -C /usr/local/java/
```

### 设置环境变量
为了能在系统级别使用Java，您需要编辑用户的bash配置文件。通常，可以通过如下命令打开`.bashrc`文件：

```shell
sudo vi ~/.bashrc
```

在文件末尾添加以下环境变量设置（如果之前没有设置过）:

```shell
export JAVA_HOME=/usr/local/java/jdk1.8.0_333
export JRE_HOME=${JAVA_HOME}/jre
export CLASSPATH=.:${JAVA_HOME}/lib:${JRE_HOME}/lib
export PATH=${JAVA_HOME}/bin:$PATH
```

之后保存并关闭文件。

### 生效环境变量
为了让修改后的环境变量立即生效，执行：

```shell
source ~/.bashrc
```

### 验证安装
安装完成后，您可以验证JDK是否已经正确安装及环境变量设置无误，通过运行以下命令：

```shell
java -version
```

屏幕上会显示您刚刚安装的Java版本信息，即表示安装成功。

## 注意事项
- 请确保您有足够的权限进行解压操作和修改系统配置。
- 根据您的具体Linux发行版，编辑环境变量的文件可能略有不同（例如，对于某些系统可能是`.profile`或`.zshrc`）。
- 此安装过程适用于大多数基于Unix的系统，包括Ubuntu、Debian、CentOS等。

通过遵循以上简单步骤，您就能在Linux系统上顺利地搭建好Java开发环境，开始您的编码之旅。

## 下载链接

[JDK1.8.0_333forLinuxx86_64](https://pan.quark.cn/s/721bfe18f80d)