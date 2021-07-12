**更新V1.3**<br />**优化界面，存活检测改为可选，增加fofa语法帮助**<br />**​**
![image.png](https://cdn.nlark.com/yuque/0/2021/png/603531/1626060360320-e78d7464-b4ce-4280-ab28-0d9c6e41a421.png?x-oss-process=image%2Fresize%2Cw_1239)<br />

**更新 V1.2：**<br />**修复系统开启代理后无法获取数据**<br />**​**

**更新 V1.1：**<br />**1、默认线程数300，默认获取数量1000**<br />**2、修改了图标**<br />**3、添加了鼠标左键双击事件，使用默认浏览器打开URL**<br />
<br />**工具介绍**<br />基于python3 tkinter 开发的，打包后内存有点大，特别是导入pandas后直接40+M，改为csv，然后用upx压缩后还是有11M<br />~~~QAQ<br />通过fofa api获取资产，支持存活检测，添加了icon_hash转换功能， 支持备份文件检测(前提得先存活检测)，方便获取指定app的源码，进行代码审计。<br />
<br />**使用方法**<br />将三个文件放在同一目录下<br />![image.png](https://cdn.nlark.com/yuque/0/2021/png/603531/1624523681215-77453b01-9b0c-4aff-aa00-71da97d7f060.png#height=99&id=ub890d6f3&margin=%5Bobject%20Object%5D&name=image.png&originHeight=197&originWidth=467&originalType=binary&ratio=1&size=31180&status=done&style=none&width=233.5)<br />**fofa.json格式如下：**
```python
{"fofa_email":"xxxxxx","fofa_key":"xxxxx"}
```
![image.png](https://cdn.nlark.com/yuque/0/2021/png/603531/1625834996690-f810ecc5-bd63-4f41-99e4-9425d876f424.png#clientId=u77fbd705-eae2-4&from=paste&height=386&id=u473da26e&margin=%5Bobject%20Object%5D&name=image.png&originHeight=772&originWidth=1240&originalType=binary&ratio=1&size=193641&status=done&style=none&taskId=u270d0839-7361-412c-a707-11949f998ca&width=620)<br />icon_hash功能<br />![image.png](https://cdn.nlark.com/yuque/0/2021/png/603531/1625835082814-930c2ac2-5e6a-4503-bf3c-bf96aa20419d.png#clientId=u77fbd705-eae2-4&from=paste&height=384&id=u3d32efcf&margin=%5Bobject%20Object%5D&name=image.png&originHeight=768&originWidth=1241&originalType=binary&ratio=1&size=190661&status=done&style=none&taskId=u431c83b0-921d-4227-9df2-9704f256d2f&width=620.5)<br />导出表格<br />![image.png](https://cdn.nlark.com/yuque/0/2021/png/603531/1625738276354-bcf5b267-4e69-452a-acac-93bb3c577540.png#height=367&id=vfPqe&margin=%5Bobject%20Object%5D&name=image.png&originHeight=733&originWidth=1190&originalType=binary&ratio=1&size=170978&status=done&style=stroke&width=595)<br />
<br />**不足&问题：<br />1、tkinter和threading模块，当任务耗时多时，会导致界面卡顿，不会影响实际扫描速度。**<br />**2、python终止多线程问题，线程不能及时停止。**<br />
<br />
<br />

