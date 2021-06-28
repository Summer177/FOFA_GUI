**更新 V1.2：**
**修复系统开启代理后无法获取数据**<br/>
**更新 V1.1：**<br />**1、默认线程数300，默认获取数量1000**<br />**2、修改了图标**<br />**3、添加了鼠标左键双击事件，使用默认浏览器打开URL**<br />
<br />**工具介绍**<br />基于python3 tkinter 开发的，打包后内存有点大，特别是导入pandas后直接40+M，改为csv，然后用upx压缩后还是有11M<br />~~~QAQ<br />通过fofa api获取资产，进行了存活检测，添加了icon_hash转换功能， 支持备份文件检测，方便获取指定app的源码，进行代码审计。<br />
<br />**使用方法**<br />将三个文件放在同一目录下<br />![image.png](https://cdn.nlark.com/yuque/0/2021/png/603531/1624523681215-77453b01-9b0c-4aff-aa00-71da97d7f060.png#clientId=uf227b51d-5d00-4&from=paste&height=99&id=ub890d6f3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=197&originWidth=467&originalType=binary&ratio=2&size=31180&status=done&style=none&taskId=u9d4fed6c-9159-4dd3-a404-47419ff5d01&width=233.5)<br />**fofa.json格式如下：**
```python
{"fofa_email":"xxxxxx","fofa_key":"xxxxx"}
```
![image.png](https://cdn.nlark.com/yuque/0/2021/png/603531/1624525944963-5261a3f5-5629-4328-b433-f5332212a336.png#clientId=uf227b51d-5d00-4&from=paste&height=322&id=u3009e1db&margin=%5Bobject%20Object%5D&name=image.png&originHeight=643&originWidth=994&originalType=binary&ratio=2&size=264285&status=done&style=none&taskId=u6e05e285-8ca9-42c5-82cc-26def732e7d&width=497)<br />icon_hash功能<br />![image.png](https://cdn.nlark.com/yuque/0/2021/png/603531/1624526400684-c5163407-3f4e-42fc-9dc1-cb81af02f56d.png#clientId=uf227b51d-5d00-4&from=paste&height=327&id=u83845af9&margin=%5Bobject%20Object%5D&name=image.png&originHeight=653&originWidth=996&originalType=binary&ratio=2&size=217947&status=done&style=none&taskId=u5a4b5b5a-9df0-4882-89e8-e1bf921eb5c&width=498)<br />导出表格<br />![image.png](https://cdn.nlark.com/yuque/0/2021/png/603531/1624526475634-8f0c5371-8d8b-4ee2-9eec-2f0498f251e2.png#clientId=uf227b51d-5d00-4&from=paste&height=363&id=u7927e1e4&margin=%5Bobject%20Object%5D&name=image.png&originHeight=725&originWidth=854&originalType=binary&ratio=2&size=137582&status=done&style=none&taskId=ua64c6ea5-816d-44c3-ae16-87d9f346ae3&width=427)<br />
<br />**不足&问题：<br />1、tkinter和threading模块，当任务耗时多时，会导致界面卡顿，不会影响实际扫描速度。**<br />**2、python终止多线程问题，线程不能及时停止。**<br />**​**

**​**

