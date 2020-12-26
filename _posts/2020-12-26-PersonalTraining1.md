---
layout: post
title: '个人训练记录 1'
date: 2020-12-26
author: Bazoka13
color: rgb(240,200,100)
cover: '../assets/1011.jpg'
tags: Training
---
### [Codeforces 1464A](https://codeforces.com/contest/1464/problem/A)

对于互相牵制的点去跑环，答案为环的个数+ $m$ -已经在对角线上的点

### [Codeforces 1464B](https://codeforces.com/contest/1464/problem/B)

最优情况一定是有一定长度的前缀为 $1(y\leq x)$ 或 $0(x\leq y)$，简单记录个前缀和遍历跑最小值就可以了 

### [Codeforces 1464C](https://codeforces.com/contest/1464/problem/C)

显然最后两个的正负性是确定的，并且我们可以将前 $n-2$ 个的正负变成任何组合

如果有某个前缀都是 - ，就从第一个开始一个一个划，就可以确保我们要构造一个一段前缀为 + 的序列，如果都为 + ，那么我们就从 $n-1$ ~ $n$ 之间划开，参考前缀为 - 的做法划分，如果有 -，我们就从前缀的 + 之后连续的 - 中最后一个 - 之后划分，剩下的相同处理方法即可。

然后就贪心搞就可以了，首先先把前 $n-2$ 个都加上，就变成了是否可以选择一些2的幂次之和为 $X$ ，乱搞就过了。

### [CodeChef  BEGGASOL](https://www.codechef.com/problems/BEGGASOL)

直接模拟就行了

挂个链接Continue [传送门](https://www.codechef.com/LTIME90B/)