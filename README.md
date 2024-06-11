Markdown,文本修饰语言，用特殊符号修饰正文效果<br>
## 标题修饰符\#

# 标题修饰符(一级标题)
## (二级标题)
### (三级标题)
#### (四级标题)
##### (五级标题)

## 正文内容

   输入成文内容，但是如果需要换行，用\<br\>标签

## 修饰正文
   
*一段测试文本*

**一段测试文本**

***一段测试文本***

~~一段测试文本~~

---

## 引用效用\>表示
> 你自己就是一座金矿，关键在于如何挖掘和利用自己
>> 苏格拉底
>>> 三级引用
>>>> 四级引用

## 列表修饰符
### 无需列表 \*
* 二次元游戏
  * 原神
    * 审理精华
* 大逃杀类
  * PUBG
  * APEX

### 有序列表 1.
1. 物理学
   1. 粒子物理
   2. yuanziwuli
   3. 京剧太物理
2. 计算机科学
   1. 分布式架构
   2. 云计算
### 混合泪飙
1. 测试一级
   * 测试二级
   2. 测试三级

### 表格
名称|技能|排行
--|:--:|--:
辩护下|youqian|32
还望|youying|23
shandixnia|pao|18

### 代码片段

```c
       #include<stdio.h>
       int main(void)
       {
       printf("test code\n");
       return 0;
       }

```
```cpp
      #include<iostream>
```
```python
      import<os>
```
```bash
      echo"测试"
      pwd
      ps aux
      ls -l
```

### 超链接技术

[Github](https://github.com/dashboard "点击访问")

### 图片链接

![桌面图片](https://i.postimg.cc/LXr71Bcw/1.jpg "点击访问")

# 笔记
## Github
### 关键字查询
* awesome,去此标签类别中查询项目
* python tutorial,查询资料，书籍，文档
* socket sample,查询对应技术的代码样本
### github 三要素
* Repository 仓库
  * 仓库是github项目管理存储的基本单元
  * 一个仓库中存储一个项目，一个用户可以拥有多个仓库，一般仓库分为public,private
* Commit 提交
  * 程序员在整个开发周期，有大量的代码资源的迭代和修改，都可以通过Commit的方式进行记录，便于程序员回溯代码，即使这些代码被删除，提交便于使用者观察整个工程的开发流程以及设计流程
* Branch 分支 
  * 在仓库中可以包含多个分支，分支才是代码文件的第一存储单位，默认的仓库主分支为Master/main
  * 不仅可以管理代码存储，便于多人协作开发
![流程图](https://i.postimg.cc/sgNkK7Z2/2.jpg "点击查看")
### 仓库内容
* Code,资源存储，代码资源，二进制，项目管理脚本，许可证等等
* issues，使用时遇到的bug 或 进行提交，等待反馈
* README,使用markdown语言编写，工程自述文件，开发进度，版本更新，使用介绍等等
* LICENSE 许可证
  * GPL 2.0，3.0，Apalce2.0,Mit,这些许可证，给使用者最大权限以及最少的限制
### Git 软件，分布式版本控制系统
* 仓库管理软件，使用git管理私人代码或企业代码
![图片](https://i.postimg.cc/434D1GPX/3.jpg "点击查看")
### 设备认证
1. 如何让网站的账户与设备绑定，后续完成代码的管理，上传下载
* 后续对仓库的操作，都要在仓库位置（master）,是SSH远程访问
  * git init //创建本地仓库
  * git config --list//查看git的配置文件
  * git config --global user.email"邮箱"
  * git config --global user.name "用户名"
  * ssh-keygen -t rsa -C "注册邮箱" //创建本地密文
  * 去对应的目录查找密文文件
  * rsa.pub 复制密文，粘贴，setting->SSH key and GPG -> new ssh key ->粘贴
![图片](https://i.postimg.cc/HLyz91z2/6.jpg "点击创建")
2. 为目标仓库起别名，定为目标仓库，后续上传
  * git remote add orgin "ssh地址" //为ssh仓库地址创建别名origin
  * git remote remove orgin //删除orgin别名
  * git remote add orgin "ssh地址" //为ssh仓库地址创建别名origin
### 本地设备与云端仓库的交互逻辑
![图片](https://i.postimg.cc/vZdz9TNg/4.jpg "点击查看")
* git add //添加内容
* git rm //删除本地文件并删除仓库数据
* git restroe //恢复被删除(仓库存在)
![图片](https://i.postimg.cc/j58b6fZP/5.jpg "点击查看")
* git rm code.c //删除本地文件及仓库中文件
* git restore code.c //复位误删除文件 (仓库存在) 
### 代码更新的依赖关系被破坏
* 本地内容要比云端新，完成更新替换，但是如果直接修改云端内容，导致，本地网内容无法再次提交
* 先拉取git pull 云端内容与本地内容合并或操作，而后再次推即可
  * git pull --rebase origin master
  * git rebase --skip"忽略旧版 更新本地后可以上传"
  * git rebase --continue “版本合并 解决冲突后可以直接上"
  * git rebase --abort "忽略新版，此时还不能上传"
### 下载开源代码
* git clone "https仓库地址" //下载开源项目code资源
### 分支Branch
* 关于分支的相关命令，创建分支，选择分支，合并分支等等


    
