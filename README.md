> 這是一個運行在 Cloudflare Workers 上的部落格程式，使用 Cloudflare KV 作為資料庫，無其他依賴。
> 兼容靜態部落格的速度，以及動態部落格的靈活性，方便搭建不折騰。很穩定
> 演示地址: [https://blog.gezhong.vip](https://blog.gezhong.vip 'cf-blog演示站點')

### TG 討論群: [@CloudflareBlog](https://t.me/cloudflareblog)

# 主要特點

- 使用 Workers 提供的 KV 作為資料庫
- 使用 Cloudflare 快取 HTML 來降低 KV 的讀寫
- 所有 HTML 頁面均為快取，可達到靜態部落格的速度
- 使用 KV 作為資料庫，可達到 WordPress 的靈活性
- 後台使用 Markdown 語法，方便快捷
- 一鍵發布 (頁面重構 + 快取清理)

# 承載能力

- KV 基本不存在瓶頸，因為使用了快取，讀寫很少
- 唯一瓶頸是 Workers 的日訪問量 10 萬，大約能承受 2 萬 IP / 日
- 文章數：1G 儲存空間，幾萬篇問題不大

# 部署步驟

這裡沒有即時預覽真難受，一系列坑會慢慢填到部落格，敬請關注 [https://blog.gezhong.vip](https://blog.gezhong.vip)

# 更新日誌

> [持續更新地址 https://blog.gezhong.vip/article/009000/update-log.html](https://blog.gezhong.vip/article/009000/update-log.html '更新日誌')

## 最近更新 (2020-12-31)

- 2020-12-31: 加入 sitemap.xml
- 2020-12-24: 本次更新，主要針對 SEO 和閱讀次數，以及多項細節優化

### 前端演示: [https://blog.gezhong.vip](https://blog.gezhong.vip '演示站點')

![](https://s3.ax1x.com/2020/12/22/rrP81S.png)

### 後端演示:

![](https://s3.ax1x.com/2020/12/22/rrAWrD.png)

## 捐贈

如果你覺得本專案幫到你了，還請支持一下作者

- [捐贈](https://afdian.net/@zhaopp '愛發電')
