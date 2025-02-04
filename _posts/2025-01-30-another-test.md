---
layout: post
title: "Another example"
author: "Eric D. Cohen"
email: "nehoc@asdf.net"
---

# Factorial works like this

Yet another test

```c
uint64_t factorial(uint64_t num) {
    if (num == 1) {
        return 1;
    }

    return num * factorial(num - 1);
}
```
