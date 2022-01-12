# Chapter 1

## 1.1 Data Structures

*Data Structure* is a **way** of 组织、存储、执行 data. Including 访问、更新、搜索、插入、删除 data. 

| Data Structure | Description                                     | Insert                      |
|:--------------:|:-----------------------------------------------:|:---------------------------:|
| Record         | *Record* 存储子元素fields并给每个field赋予名字               |                             |
| Array          | *Array*存储有序的元素，每个元素通过位置索引访问                     | 创建一个位置给新插入的元素               |
| Linked List    | *Linked List*的Node存储有序元素，指针指向下一个Node            | 新元素的指针指向插入位置的后方元素而前方元素指向新元素 |
| Binary tree    | *Binary tree*的每个Node存储两个数据Left/Right Child      |                             |
| Hash table     | *Hash table*将每个元素无序地映射到数组的位置中                   |                             |
| Heap           | *Max-heap*的Node的keys&ge;子Node的keys而*Min-heap*反之 |                             |
| Graph          | *Graph*的一个元素储存在由边连接的Vertex而两个储存在边               |                             |

## 1.2 Introduction to Algorithms

*Algorithm*是进行计算的步骤集合，可以用自然语言、伪代码、编程语言、硬件来描述。*Computational Problem*会指定一个输入、关于输入的问题、和输出。

### Practical applications of algorithms

| 应用领域           | Computational Problem          | Common Algorithm                                                                         |
|:--------------:|:------------------------------:|:----------------------------------------------------------------------------------------:|
| DNA Analysis   | 求两个来自不同个体的DNA序列中最长的共价核苷酸序列是什么？ | *Longest common substring problem*:最长共同子串算法确定两个输入字符串中存在的最长共同子串。DNA序列可以由ACGT组成的字符串表示四个核苷酸 |
| Search Engines | 求所有库存产品的排序数组，产品是否有库存，产品的价格     | *Binary search*: 元素会被排序，且可以直接访问                                                          |
| Navigation     | 求用户从当前位置步行到目的地的最快路线            | *Dijkstra's shortest path*: 该算法确定了从起始顶点到图中每个顶点的最短路径                                      |

### Efficient algorithms and hard problems

**NP-complete** problems是已知没有高效算法的NP问题集合，包含以下特征：

- 目前还没有发现解决NP问题的高效算法。

- 解决NP问题的高效算法是有可能存在的。

- 如果一个NP问题存在高效算法，那所有NP问题都可被解决。

##### Hint

1. 通过已知一个问题是NP问题，程序员可以专注于找到一个非最优解的算法，而不是浪费时间试图找到一个更高效的算法来解决问题。

2. Polynomial runtime大多数时候都比Exponential runtime更高效。

3. 一个高效的算法只服务于特定类型的问题。

## 1.3 Relation Between Data Structures and Algorithms

### Algorithms for data structures

*Data Structures*定义了存储方式，而*Algorithms*实现了如何和处理数据。

#### Hint

- 大部分情况下，不同的数据结构需要不同的算法，同时，也会存在通用的算法。

### Algorithms using data structures

**Description**：算法利用数据结构来存储和组织算法执行过程中的数据。

## 1.4 Abstract data types

### Abstract data types (ADTs)

*Abstract Data Type*是一种预定义的用户操作描述的数据类型，如"在后方插入数据"，而不指出是如何实现的。一个*ADT*可以使用不同的底层数据结构来实现。然而，程序员不需要太了解就可以使用*ADT*。

**Example**: *Linked List*是一个常见的保存有序数据的*ADT*，具有附加、删除、搜索元素，以及元素是否存在和显示列表等操作。*ADT*通常使用*Array*或*Linked List*来实现。

### Common ADTs

| Abstract data type | Description  | Common underlying data structures |
|:------------------:|:------------:|:---------------------------------:|
| List               | 有序，允许复制      | Array, linked list                |
| Dynamic array      | 有序，允许访问      | Array                             |
| Stack              | 在顶部添加、删除     | Linked list                       |
| Queue              | 尾部添加，顶部删除    | Linked list                       |
| Deque              | 顶部尾部添加、删除    | Linked list                       |
| Bag                | 无序，允许复制      | Array, linked list                |
| Set                | 无序，不允许复制     | Binary search tree, hash table    |
| Priority queue     | 优先元素顶部的Queue | Heap                              |
| Dictionary (Map)   | 元素被映射        | Hash table, binary search tree    |

## 1.5 Applications of ADTs

### Abstraction and optimization

*Abstraction*让用户与更简单、更高层的操作进行交互，而底层细节将会被隐藏。*ADT*通过隐藏底层的细节并提供定义明确的操作来简化交互。使用*ADT*能让程序员专注于更高层的操作和算法，来提高效率。然而，若需分析或提高程序运行效率，则需要了解底层细节。

### ADTs in standard libraries

多数语言提供实现常见*ADT*的标准库。有些语言允许用户选择用于*ADT*的基础数据结构。其他语言可能使用特定的数据结构来实现每个ADT，或自动选择底层数据结构。

| Programming language | Library                          | Common supported ADTs                       |
| -------------------- | -------------------------------- | ------------------------------------------- |
| Python               | Python standard library          | list, set, dict, deque                      |
| C++                  | Standard template library (STL)  | vector, list, deque, queue, stack, set, map |
| Java                 | Java collections framework (JCF) | Collection, Set, List, Map, Queue, Deque    |

# Chapter 2

## 2.1
