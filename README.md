# My actions
for use my own github actions

## 关于时区的问题

github action触发的时区应该是UTC时区，和北京时间(UTC+8)差了八个小时。

使用在设置crontab自动触发的时候，需要换算一下时间才能正确按照我们的时区时间触发

其实还有一种方法是用一个全局的变量

```yaml
env:
  TZ: Asia/Shanghai
```

这样写据说可以，但是我还没尝试成功



## 关于checkout的问题

