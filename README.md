**程式目的**

這隻爬蟲程式是用來抓取 Ptt/Macshop 版的文章資訊，用以分析特定二手品的價格、年份、販售者以及相關資訊，讓買方可以快速知道目前板上該商品的二手價位情形。計畫以下列功能逐步實現爬蟲程式內涵。

**功能規劃**

1. 特定網頁連接
2. 文章列表抓取
3. 文章列表欄位分析
4. 文章內文抓取
5. 文章內文欄位分析
6. 資料庫環境建置
7. 文章內文欄位儲存至資料庫
8. 統計分析
9. 簡易API介面操作

**功能細節**

1. 特定網頁連接
```
def fetch(url):
    ''' Step-1: send a request and fetch the web page.
    '''
    response = requests.get(url)
    return response
```

**來源參考**
- leVirve/CrawlerTutorial: https://github.com/leVirve/CrawlerTutorial/blob/master/src/basic_crawler.py
