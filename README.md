# 数据结构导论 Arrange

# 第四章 数和二叉树

**二叉树的性质**：

> - 性质1 ：二叉树第i层上至多有2^i^ ^-^ ^1^ 个结点
> - 深度为 k （k>=1）的二叉树至多有2^k^ -1 个结点，最少 k个
> - 二叉树，若度数为0的节点个数为n~0~，度数为2的结点个数为n~2~，则n~0~=n~2~+1。







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