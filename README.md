# 自製FinLab課程環境
[[課程網址](https://hahow.in/cr/python-finance)]
## package
(網頁爬取)  
* requests
* BeautifulSoup4
* [pyquery](https://aji.tw/slides/pycon2017 "投影片")
* Scrapy

(資料分析)
* pandas  
* numpy
* lxml

(影片下載)
* youtube_dl  

(資料庫連接)
* pymysql
* sqlite

(視覺化)
* dash

(股票分析)
* talib
* twstock


啟動方式(Linux):  
```shell
docker run -d --name=ds-jupyter --restart=always \
-p 8888:8888 \
-v /your/python/path:/home/jovyan/work \
t985026/finlab-course start-notebook.sh \
--NotebookApp.ip='*' \
--NotebookApp.token=''
```

可添增參數
`--notebookApp.password='密碼'`