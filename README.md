[TOC]

---

#### 禁用启用笔记本自带键盘

```console
sc config i8042prt start= disabled
sc config i8042prt start= auto
```

#### 清除网页所有定时器

```
for(var i = 1; i < 1000; i++) {
  clearInterval(i);
}
```

#### 删除线

```
\u0336
```
