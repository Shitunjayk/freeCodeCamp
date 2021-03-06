---
title: ACID
localeTitle: 酸
---
## 酸

在计算机科学中，ACID（原子性，一致性，隔离性，耐久性）是用于数据库修改的一组属性。它们有助于保证事务的有效性，即使出现错误或失败也是如此。

**事务**是满足ACID属性的任何数据库操作序列，可以视为对数据的单个逻辑操作。一个例子是将资金从一个银行账户转移到另一个银行账户。这涉及多项更改，例如借记一个帐户并贷记另一个帐户，但被视为单个交易。

### 原子性

这意味着复杂的交易要么完全处理，要么根本不处理。如果事务的一部分失败，则整个事务未完成且数据库未更改。这样，如果发生崩溃，电源故障或错误，数据库最终不会处于仅完成部分事务的状态。

### 一致性

这意味着数据将保持一致。输入数据库的任何数据必须是有效的，并且必须基于您指定的任何约束。它确保任何事务都将数据库从一个有效状态更改为另一个有效状态。

### 隔离

这意味着如果两个事务同时执行，则一个事务无法从尚未完成的事务中读取数据。每个事务都将看到数据库，就好像事务是按顺序执行一样。如果一个事务需要读取另一个事务正在写入的数据，则必须等到另一个事务完成。不完整交易的影响不会影响另一笔交易。

### 耐久力

这意味着一旦交易完成，即使出现断电或其他错误，交易仍将如此。它保证将所有更改记录到非易失性存储介质（例如硬盘）中，并记录已完成的事务。

### 更多信息：

*   ACID文章： [维基百科](https://en.wikipedia.org/wiki/ACID)
*   视频概述： [YouTube](https://www.youtube.com/watch?v=LSB4eceRsw8)