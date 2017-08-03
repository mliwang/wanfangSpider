# wanfangSpider
该项目用于爬取万方数据库文献摘要数据，爬虫文件在万方文件夹里面，爬取数据在data1里面，目前data1里面有一份数据可供参考

# 使用方法
  ## 1 需要安装scrapy爬虫框架
  ## 2 git改项目
  ## 3 修改wanfang/wanfang/spiders/wanfang.py 的关键字
  ## 4 使用 scrapy crawl wanfang 进行爬取
# 关键字修改说明
  ## 主要修改该两个地方
  
* 1 目录url抓取起始页 讲中医修改为你需要爬取的关键字
```
start_urls = [
        'http://s.wanfangdata.com.cn/Paper.aspx?q=中医&f=top&p=1'
    ]

```
* 2 摘要抓取url 讲self.key 修改为你需要爬取的关键字
```
def __init__(self):
    self.key = '彙º罃½计签W'
    self.count = 0
    self.url_1 = 'http://s.wanfangdata.com.cn/Paper.aspx?q='+ self.key +'&f=top&p='
```
> 注意： 两个关键字必须一样

# 格式说明
```
```

# 结果展示
```
```
