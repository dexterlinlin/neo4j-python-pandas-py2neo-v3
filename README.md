# neo4j-python-pandas-py2neo-v3
利用pandas将excel中数据抽取，以三元组形式加载到neo4j数据库中构建相关知识图谱
# Neo4j知识图谱构建
![](https://s1.ax1x.com/2018/11/13/iObQkn.png)

### 1.运行环境：  
python3.6.5  
windows10  
具体包依赖可以参考文件requirements.txt
```
pip install -r requirements.txt
``` 

### 2.Pandas抽取excel数据
Excel数据结构如下

<img src="https://s1.ax1x.com/2018/11/13/iObTc8.png" width="800" hegiht="500" align=center />

通过函数data_extraction和函数relation_extrantion分别抽取构建知识图谱所需要的节点数据以及联系数据，构建三元组。  
数据提取主要采用pandas将excel数据转换成dataframe类型    
invoice_neo4j.py  
<img src="https://s1.ax1x.com/2018/11/13/iOb4ht.png" width="500" hegiht="313" align=center />

### 3.建立知识图谱所需节点和边数据  
DataToNeo4jClass.py  
<img src="https://s1.ax1x.com/2018/11/13/iXk6iV.png" width="500" hegiht="313" align=center />

-----------------------------------------------------------------------------------------------------
## 2019.2.15更新
### 更新neo4j_matrix.py代码，将知识图谱中数据抽取转化成矩阵，为机器学习模型提供数据

## Enjoy it!

## 2019.3.30
4.安装Neo4j
https://neo4j.com/licensing/ 选择Community Edition
5、关于python requirements安装
requirements.txt比较老，建议运行完pip install -r requirements.txt,再整体更新所有Python库



### Neo4j教程
https://www.w3cschool.cn/neo4j/
https://cloud.tencent.com/developer/article/1336299

豆瓣电影实战：
https://blog.csdn.net/Chen18125/article/details/84101458

### TODO
 Vue + Django + Neo4j 完整实例