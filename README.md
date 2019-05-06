本项目可以将备份好的朋友圈在网页浏览(截至2019.3.6共457条朋友圈)

## 使用说明
目录结构如下：
```
- assets
- outputs
- datas
 - xxx图片
 - xxx图片
 - ......
 - data.json
index.html
serve.sh
word.py
......
```

启动服务器，然后打开 `http://localhost:8000`
```
go run serve.go
或者php -S localhost:8000
```
![](./assets/朋友圈.png)

## 生成词云
简单地做一个词频分析，生成词云

```
pip install jieba imageio wordcloud
python word.py
```

然后 `outputs` 目录下生成 `word.png`
![](./outputs/word.png)
### 问题
摇一摇分享的歌曲无法打开，小视频无法打开。

### 感谢
[👉不知道朋友圈备份文件哪来？](https://mp.weixin.qq.com/s?__biz=Mzg4MDExMTUwMw==&mid=2247483679&idx=1&sn=12f73bf7f92f94b12ec057e64913b0f8&chksm=cf7b7bfff80cf2e9afa369117e5da5733854f4823e70dddce64a5537a7de3c24bb1b121727cb&token=1469653834&lang=zh_CN#rd)

[WechatSnsViewer](https://github.com/coolzilj/WechatSnsViewer)