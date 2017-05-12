# annual_report_crawl
爬取中國年報
Readme
created time : 2016.12.04 
created by : Shen Chen


## 三个 python 文件 和 stockNum.xlsx、annual_report文件夹要在相同目录下

# AR_spider.py

这个是主要的爬虫软件。
- 要求
需要在运行目录下创建一个名为「annual_report」的文件夹，并和「stockNum.xlsx」在同一个目录下。

- 执行
```
python AR_spider.py
```
命令即可。
如果提示未安装什么 module ， 安装相应的 module 即可。

- 执行结果
年报内容会在「annual_report」文件夹下，对应的目录会在「index.tsv」文件中

# tsv2csv.py
- 要求
和「index.tsv」在同一个目录下

- 执行
```
python tsv2csv.py
```

- 执行结果
index.tsv 转成 index.csv 文件

# findMissing

- 在相同目录下

- 执行
```
python findMissing.py
```

- 执行结果
找出index.tsv中存在而annual_report文件夹里不存在的年报
