---

title: Jmeter快速入门

date: 2021-10-23 10:40:06

categories: java


---

# Jmeter快速入门







# 1.安装Jmeter

Jmeter依赖于JDK，所以必须确保当前计算机上已经安装了JDK，并且配置了环境变量。



## 1.1.下载

可以Apache Jmeter官网下载，地址：http://jmeter.apache.org/download_jmeter.cgi

![image-20210715193149837](Jmeter快速入门/image-20210715193149837.png)



当然，我们课前资料也提供了下载好的安装包：

apache-jmeter-5.4.1.zip



## 1.2.解压

因为下载的是zip包，解压缩即可使用，目录结构如下：

![image-20210715193334367](Jmeter快速入门/image-20210715193334367.png)

其中的bin目录就是执行的脚本，其中包含启动脚本：

![image-20210715193414601](Jmeter快速入门/image-20210715193414601.png)

### 1.3.运行

双击即可运行，但是有两点注意：

- 启动速度比较慢，要耐心等待
- 启动后黑窗口不能关闭，否则Jmeter也跟着关闭了

![image-20210715193730096](Jmeter快速入门/image-20210715193730096.png)



# 2.快速入门



## 2.1.设置中文语言

默认Jmeter的语言是英文，需要设置：

![image-20210715193838719](Jmeter快速入门/image-20210715193838719.png)

效果：

![image-20210715193914039](Jmeter快速入门/image-20210715193914039.png)



> **注意**：上面的配置只能保证本次运行是中文，如果要永久中文，需要修改Jmeter的配置文件



打开jmeter文件夹，在bin目录中找到 **jmeter.properties**，添加下面配置：

```properties
language=zh_CN
```

![image-20210715194137982](Jmeter快速入门/image-20210715194137982.png)



> 注意：前面不要出现#，#代表注释，另外这里是下划线，不是中划线





## 2.2.基本用法

### 线程组

在测试计划上点鼠标右键，选择添加 > 线程（用户） > 线程组：

![image-20210715194413178](Jmeter快速入门/image-20210715194413178.png)

在新增的线程组中，填写线程信息：

![image-20210715195053807](Jmeter快速入门/image-20210715195053807.png)



### http取样器

给线程组点鼠标右键，添加http取样器：

![image-20210715195144130](Jmeter快速入门/image-20210715195144130.png)



编写取样器内容：

![image-20210715195410764](Jmeter快速入门/image-20210715195410764.png)



### 添加监听报告：

![image-20210715195844978](Jmeter快速入门/image-20210715195844978.png)

### 添加监听结果树：

![image-20210715200155537](Jmeter快速入门/image-20210715200155537.png)



### 汇总报告结果：

![image-20210715200243194](Jmeter快速入门/image-20210715200243194.png)

### 结果树：

![image-20210715200336526](Jmeter快速入门/image-20210715200336526.png)

# 【Jmeter第三章】Jmeter给请求添加请求头

https://blog.csdn.net/weixin_47316183/article/details/130754845

![image-20230702173049426](img/img_Jmeter%E5%BF%AB%E9%80%9F%E5%85%A5%E9%97%A8/image-20230702173049426.png)

# Jmeter教程9：自增参数设置

https://blog.csdn.net/lala_yanzi/article/details/124269473