
### 功能

- [x] 载入动画
- [x] 站点简介
- [x] Hitokoto 一言
- [x] 日期及时间
- [x] 实时天气
- [x] 时光进度条
- [x] 音乐播放器
- [x] 移动端适配

* [ ] 去除 jQuery 依赖
* [ ] VUE 重构

### 第三方配置

- 配置 高德地图天气API配置   申请api-key

![image-20250717154341141](E:\program\blog-home\README.assets\image-20250717154341141.png)

<!-- ### 配置

本项目采用 `json` 文件来配置站点内容，该配置不受版本更新影响，可将自定义配置写入 `setting.json` 以更改页面内容

<details>
<summary>配置说明</summary>

```json
{
    "title": "网页标题",
    "description": "网页简短介绍",
    "keywords": "网页关键词",
    "author": "网页作者",
    "logo_img": "Logo图片路径",
    "logo_text_1": "域名前缀",
    "logo_text_2": "域名后缀",
    "des_title": [
        "Hello World !", //站点介绍标题
        "一个建立于 21 世纪的小站，存活于互联网的边缘" //站点介绍内容
    ],
    "des_title_change": [
        "Oops !", //站点介绍标题点击后文字
        "哎呀，这都被你发现了 ( 再点击一次可关闭 )" //站点介绍内容点击后文字
    ],
    "github": "imsyy", //Github 用户名
    "qq": "1539250352", //QQ
    "email": "one@imsyy.top", //Email电子邮件
    "telegram": "bottom_user", //Telegram 用户名
    "twitter": "iimmsyy", //Twitter用户名
    "weather_api": "https://www.yiketianqi.com", //天气 API
    "link_1": [
        "https://blog.imsyy.top/", //链接地址
        "fa-solid fa-blog", //图标类名
        "博客" //链接文字
    ],
    "link_2": [
        "https://drive.imsyy.top/",
        "fa-solid fa-cloud",
        "网盘"
    ],
    "wallpaper_api": [
        [
            "每日一图", //壁纸设置项名称
            "https://api.dujin.org/bing/1920.php" //壁纸图片链接
        ]
    ],
    "Copyright_year": "2020", //站点起始年份
    "Copyright_text": "無名" //版权
}
```

</details> -->

### 音乐

```
https://api.wuenci.com/meting/api/?server=netease&type=playlist &id=156934569
```

```
# 歌曲 API 地址
## 请参照 https://github.com/xizeyoupan/Meting-API#deno-deploy 进行 API 服务部署
## 此处提供的服务可能会超量从而无法访问，请自行部署
## 若使用 QQ 音乐歌单，歌曲数量最好不要超出 50 首
## 备用：https://api.wuenci.com/meting/api/
VITE_SONG_API = "https://api-meting.imsyy.top/api"
# 歌曲服务器 ( netease-网易云, tencent-qq音乐 )
VITE_SONG_SERVER = "netease"
# 播放类型 ( song-歌曲, playlist-播放列表, album-专辑, search-搜索, artist-艺术家 )
VITE_SONG_TYPE = "playlist"
# 播放 ID ( 若无需播放器，请设为空即可 )
VITE_SONG_ID = "9379831714"
```



>本项目采用了基于 `MetingJS` 的 `Aplayer` 音乐播放器，可实现快速自定义歌单  
>*仅支持 **中国大陆地区**，其他区域请将 [以下内容](https://cdn.jsdelivr.net/gh/imsyy/file/js/music/music-other.js) 替换 `music.js` 以实现音乐播放器的正常使用

更改 `music.js` 的参数即可实现自定义歌单列表

```js
let server = "netease"; //netease: 网易云音乐; tencent: QQ音乐; kugou: 酷狗音乐; xiami: 虾米; kuwo: 酷我
let type = "playlist"; //song: 单曲; playlist: 歌单; album: 唱片
let id = "7452421335"; //封面 ID / 单曲 ID / 歌单 ID
```

### 问题

>由于 CDN 缓存原因，查看最新效果可能需要 `Ctrl` + `F5` 强制刷新浏览器缓存

- [acmakbの主页](http://www.acmakb.top)

