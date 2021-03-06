# 数据结构 第三次实验课作业

# 题目

## 第七章实验题11
### 目的
深入掌握二叉树的遍历和构造算法。
### 内容
编写一个程序 ```exp7-11.cpp``` ，实现二叉树的序列化和反序列化

这里介绍通过先序遍历实现二叉树的序列化和反序列化（也可以采用层次遍历实现序列化和反序列化），假设二叉树每个结点值为单个字符（不含```#```，这里用```#```字符表示对应空结点）。

所谓序列化，就是对二叉树进行先序遍历产生一个字符序列的过程，与一般先序遍历不同的是，这里还要记录空结点。

例如，如```图7.26```所示的一棵二叉树，一般先序遍历是```ABDEGCFHI```，而这里的先序序列化的结果是```ABD##E#G##C#FH##I##```。
相当于在二叉树上标记上所有的空结点，如```图7.27```所示（也称为扩展二叉树），然后进行先序遍历。

|  ```图7.26```                         | \| |  ```图7.26```                         |
|:--------------------------------------|----|:--------------------------------------| 
|<img src="image/7.26.svg" width="320"/>|    |<img src="image/7.27.svg" width="320"/>|



所谓反序列化，就是通过先序序列化的结果串 ```str``` 构建对应的二叉树，其过程是：
用 ```i``` 从头到尾扫描 ```str``` ，采用先序方法，当 ```i``` 超限时返回 ```NULL``` ；
否则当遇到```#```字符，返回 ```NULL```，当遇到其他字符时，创建一个结点，然后递归构造它的左右子树。

可以证明，采用先序遍历实现的二叉树序列化和反序列化结果是唯一的。

实现上述过程，完成如下功能：
1. 创建二叉链 ```b``` 。
2. 采用括号表示输出二叉链 ```b``` 。
3. 对二叉链 ```b``` 进行先序遍历，产生先序序列化序列 ```str``` 。
4. 输出串 ```str``` 。
5. 由 ```str``` 构造二叉链 ```b1``` 。
6. 销毁二叉链 ```b``` 和 ```b1``` 。

# 提交
1. 将作业打包为压缩文件，如 ```zip``` 格式。
2. 压缩文件命名为你的学号， 如 ```2018302114514.zip``` 。
3. 将压缩文件以附件形式发送到邮箱 ```DS_Exp3 # superexercisebook.com```
4. 如果一切顺利，你将会收到一个投递成功回执。