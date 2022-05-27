## stealth.min.js

selenium 过环境检测

```python
with open(path+'/stealth.min.js') as f:
    js = f.read()

driver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {
  "source": js 
})
```

### 效果

- 注入前

![](./img/previous.png)

- 注入后

![](./img/after.png)

### 参考资料

- https://blog.csdn.net/weixin_42453905/article/details/122086184
- http://fengpiaoxus.com/blog/detail/3/
