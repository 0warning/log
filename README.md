
#### 禁用启用笔记本自带键盘

```batch
sc config i8042prt start= disabled
sc config i8042prt start= auto
```

#### 清除网页所有定时器

```javascript
for (var i = 1; i < 1000; i++) {
  clearInterval(i);
}
```

#### 删除线

```
\u0336
```

#### Linux批量替换

```
find . -name *.ftl | xargs sed -i 's/http:\/\/www\.gsmz\.gov\.cn\//\//g'

find . -name *.ftl | xargs sed -i 's/http:\/\/www\.gsmz\.gov\.cn/\//g'


find . -name *.html | xargs sed -i 's/http:\/\/www\.gsmz\.gov\.cn\//\//g'

find . -name *.html | xargs sed -i 's/http:\/\/www\.gsmz\.gov\.cn/\//g'
```
