# 数据结构 第六次课堂作业

# 题目

## 第七章练习题 20
假设二叉树以二叉链存储，设计一个算法判断一颗二叉树 ```b``` 是否为完全二叉树。

## 课堂题目
假设二叉树采用二叉链存储结构，设计一个算法求二叉树 ```b``` 的宽度（采用层次遍历方法）。
```c++
    int BTWidth2(BTNode *b)
    {
        struct
        {
            int lno;
            BTNode *p;
        } Qu[MaxSize];
        int front, rear;

        int lnum, widthm, i, n;
        front = rear = 0;
    }
```

# 提交
1. 将作业打包为压缩文件，如 ```zip``` 格式。
2. 压缩文件命名为你的学号， 如 ```2018302114514.zip``` 。 
3. 将压缩文件以附件形式发送到邮箱 ```DS_Task6 # superexercisebook.com```
4. 如果一切顺利，你将会收到一个投递成功回执。