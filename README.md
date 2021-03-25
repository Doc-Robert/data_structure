# 数据结构导论 Arrange

# 第四章 数和二叉树

**二叉树的性质**：

> - 性质1 ：二叉树第i层上至多有2^i^ ^-^ ^1^ 个结点
> - 深度为 k （k>=1）的二叉树至多有2^k^ -1 个结点，最少 k个
> - 二叉树，若度数为0的节点个数为n~0~，度数为2的结点个数为n~2~，则n~0~=n~2~+1。



# 第五章 图

## 5.1 图的概念

图的定义：

有向完全图 ：n个顶点有 n（n-1）/2 条边
无向完全图 ：n（n-1）条边



## 5.2 图的存储结构

### 5.2.1 邻接矩阵

用矩阵来描述图中顶点之间的关联关系

### 5.2.2 邻接表

顺序存储和链式存储相结合的存储方法

## 5.3 图的遍历

深度优先搜索

广度优先搜索

> 类似树的按层次遍历

## 5.4 图的应用



### 5.4.1 最小生成树

prim生成最小生成树



### 5.4.2 拓扑排序

步骤：

> 1. 选择入度为0的顶点，输出该顶点
> 2. 删除与其相关连的弧
> 3. 重复执行1,2 直到剩下一个

拓扑排序算法的时间复杂度 为O(n+e)

# 第六章 查找



## 6.1基本概念

> 查找：从大量数据元素找出指定的数据元素
>
> 关键字：简称键，数据元素的某个数据项
>
> 键值：该数据项的值‘



## 6.2静态查找表

### 1.顺序表的查找

> **查找长度**：数据元素的键值与给定值的比较次数
>
> **平均查找长度**：对于一个长度为n的顺序表，采用顺序查找法，平均查找长度为（n+1）/2





### 2.有序表的查找

#### 二分查找

​		给定值 key 与处于mid 的中间位置的数据元素比较， 大于或小于中间值判断给定值位置，并不断缩小范围

> 平均查找长度：ASL~b~ =  n/n+1  * log~2~（n+1）-1 



### 3.索引顺序表的查找

​		一个索引表一个顺序表

步骤：

1. 确定待查元素所在的块
2. 在块内顺序查找

#### 分块查找

> 平均查找长度：ASL~b~ =1/2  ( n/s + s )+1





## 6.3 二叉排序树

> **性质：**
>
> - **若左子树不空，则左子树上所有结点的键值均小于它的根节点键值**
> - **若右子树不经，则右子树上所有结点的键值均大于它的根节点键值**
> - **根的左、右子树也分别为二叉排序树**

`二叉排序树具有递归性`

`左子树节点小于根节点`

`右子树节点大于根节点`

`tips:`

​	若中序遍历 则



# 第七章 排序



## 7.2 插入排序

直接插入排序需要一个记录的辅助空间

时间复杂度O(n^2^)

空间复杂度O（n）

## 7.3 交换排序

### 7.3.1 冒泡排序

第一个与第二个比较，第二个比第一个大就交换，持续

### 7.3.2 快速排序

冒泡排序的一种改进，

在n个记录中取某一个记录的键值作为标准，通常去第一个记录键值为基准，通过一趟排序的记录分为小于这个键值或者大于这个键值的两个独立的部分，这时一部分记录的键值均比另一部分的键值小，然后快速排序



## 7.4 选择排序

### 7.4.1 直接选择排序

时间复杂度

好：O（nlog~2~n）

坏：O(n^2^)



### 7.4.2 堆排序



## 7.5 归并排序

归并排序与要求 待排序列由若干个有序子序列组成

7.5.1

### 7.5.2 二路归并排序

两个有序表合并为一个有序表

假设序列有n个记录 ，看作n个有序子序列。将相邻的两个记录合并，在将上述子序列两两合并。重复此。得到一个长度为n的有序序列