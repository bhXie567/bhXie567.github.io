---
title: Test-Cache地址映射
date: 2026-08-05 20:00:00
updated: 2026-08-05 20:00:00
categories:
  - 笔记
  - 11408
  - 计算机组成原理
tags:
  - "408"
  - Cache
math: true
comments: true
---

## 基本概念

Cache利用程序访问的时间局部性和空间局部性。

主存地址通常被划分为：

$$
\text{主存地址}
=
\text{标记位}
+
\text{组号}
+
\text{块内地址}
$$

<!-- more -->

## 直接映射

直接映射满足：

$$
\text{Cache行号}
=
\text{主存块号}
\bmod
\text{Cache行数}
$$

## 易错点

1. 块内地址位数由块大小决定。
2. 标记位不包含有效位和脏位。
3. 注意区分主存块号与Cache行号。

## 例题

假设主存地址为32位，Cache数据区容量为32 KB，块大小为64 B。

块内地址位数为：

$$
\log_2 64=6
$$

```cpp
#include <iostream>

int main() {
    std::cout << "Hello, Hexo!" << std::endl;
    return 0;
}
```

![Test1](/img/postBanner.jpg)
![Test2](/img/post/test.png)
