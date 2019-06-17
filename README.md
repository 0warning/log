
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

#### Argument list too long

```
ls -l| awk '{ print "rm -f ",$9}'|sh
```

#### linux autostart

sh:

```
#!/bin/sh
#chkconfig: 2345 80 90
#description:autostart
```

system:

```
cd /etc/rc.d/init.d/
chmod +x sh
chkconfig --add sh
chkconfig sh on
```

#### nginx 跨域

```
location /xxx {
  if ($request_method = 'OPTIONS') {
    add_header Access-Control-Allow-Origin *;
    add_header Access-Control-Allow-Methods GET,POST,PUT,DELETE,PATCH,OPTIONS;
    add_header Access-Control-Allow-Headers *;
    return 200;
  }
  proxy_pass http://xxx;	
}
```
