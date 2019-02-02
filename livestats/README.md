# OBS 直播時間 觀眾人數 顯示器

## 公告
**因應Twitch更新強制OAuth認證流程, 請改用新版本顯示器**
[https://github.com/StinkingBanana/StinkingBanana.github.io/tree/master/livestats2](https://github.com/StinkingBanana/StinkingBanana.github.io/tree/master/livestats2)

## 預覽
<p><img src="./preview.png"></p>

## 工具網址
[https://stinkingbanana.github.io/livestats/livestats.html](https://stinkingbanana.github.io/livestats/livestats.html)

## 參數
* ```login``` = {你的Twitch登入帳號}
* ```clientID``` = {你的用戶端 ID}
* ```flag``` = {國家代碼}

## 使用方式
以下設置是假設你的OBS的畫布大小是1920x1080為前提

#### 顯示 "日期", "時間"
1. 打開你的OBS Studio
1. 加入瀏覽器來源
    * 網址: ```https://stinkingbanana.github.io/livestats/livestats.html```
    * 寬度: 440
    * 高度: 22


#### <strike>顯示 "日期", "時間", "觀看人數", "直播時間"</strike>
1. 從Twitch開發人員網站取得你自己的**用戶端 ID** ```https://glass.twitch.tv/console/apps```
1. 從APP頁面註冊您的應用程式
    * 名稱: ```Yourname's ViewerCount Display``` (任何名稱只要不跟他人的重複，不是很重要)
    * OAuth 重新導向網址: ```https://127.0.0.1``` (不會使用到重新導向，所以我們直接導向回localhost就可以了)
    * 分類: ```Analytics Tool```
1. 新增完新的APP之後點進去複製**用戶端 ID** (請勿與他人分享自己的用戶端ID)
1. 打開你的OBS Studio
1. 加入瀏覽器來源
    * 網址: ```https://stinkingbanana.github.io/livestats/livestats.html?login={你的Twitch登入帳號}&clientID={你的用戶端 ID}```
    * 寬度: 645
    * 高度: 22

#### <strike>顯示 "日期", "時間", "直播時間" ; 不顯示 "觀看人數"</strike>
1. 從Twitch開發人員網站取得你自己的**用戶端 ID** ```https://glass.twitch.tv/console/apps```
1. 從APP頁面註冊您的應用程式
    * 名稱: ```Yourname's ViewerCount Display``` (任何名稱只要不跟他人的重複，不是很重要)
    * OAuth 重新導向網址: ```https://127.0.0.1``` (不會使用到重新導向，所以我們直接導向回localhost就可以了)
    * 分類: ```Analytics Tool```
1. 新增完新的APP之後點進去複製**用戶端 ID** (請勿與他人分享自己的用戶端ID)
1. 打開你的OBS Studio
1. 加入瀏覽器來源
    * 網址: ```https://stinkingbanana.github.io/livestats/livestats.html?login={你的Twitch登入帳號}&clientID={你的用戶端 ID}&vc=0```
    * 寬度: 580
    * 高度: 22

#### 附加顯示 "國旗"
* 如果網址裡面**沒有**使用過問號"```?```" 請在網址後面添加 ```?flag={國家代碼}```
    * 舉例: 臺灣 
    * 修改前: ```https://stinkingbanana.github.io/livestats/livestats.html```
    * 修改後: ```https://stinkingbanana.github.io/livestats/livestats.html?flag=tw```
* 如果網址裡面**有**使用過問號"```?```"  請在網址後面添加 ```&flag={國家代碼}```
    * 舉例: 臺灣
    * 修改前: ```https://stinkingbanana.github.io/livestats/livestats.html?login={你的Twitch登入帳號}&clientID={你的用戶端 ID}```
    * 修改後: ```https://stinkingbanana.github.io/livestats/livestats.html?login={你的Twitch登入帳號}&clientID={你的用戶端 ID}&flag=tw```
* 國家代碼請參照 [ISO 3166-1 alpha-2](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
* 請在原來的寬度再加上 ```35``` 或是 足夠的寬度直到你看見國旗顯示出來

## 備註
* "**直播時間**" 與 "**觀看人數**" 需要開台後約1~2分鐘才會刷新
<br>
<br>  

# OBS Twitch Viewer Count, Uptime, Date and Time Display

## Parameters
* ```login``` = {your twitch login ID}
* ```clientID``` = {your Client ID}
* ```flag``` = {country code}

## TO USE

#### This setup assumes your OBS is using canvas size of 1920x1080

Display "date",  "current time" 
1. Open your OBS Studio
1. Add Browser Source
    * URL: ```https://stinkingbanana.github.io/livestats/livestats.html```
    * Width: 440
    * Height: 22

<strike>Display "date",  "current time" , "uptime", "viewer count"</strike>
1. Get your cliendID through Twitch Dev Console ```https://glass.twitch.tv/console/apps```
1. Register New App
    * Name: ```Yourname's ViewerCount Display``` (Any unique name, does not really matter since you are the only user.)
    * OAuth redirect: ```https://127.0.0.1``` (Not gonna use redirect, so setting it to localhost is enough.)
    * Category: ```Analytics Tool```
1. Copy your Client ID (Do NOT share your client ID with anyone else)
1. Open your OBS Studio
1. Add Browser Source
    * URL: ```https://stinkingbanana.github.io/livestats/livestats.html?login={your twitch login ID}&clientID={your Client ID}```
    * Width: 645
    * Height: 22

<strike>Display "date",  "current time" , "uptime" ; NOT Display "viewer count"</strike>
1. Get your cliendID through Twitch Dev Console ```https://glass.twitch.tv/console/apps```
1. Register New App
    * Name: ```Yourname's ViewerCount Display``` (Any unique name, does not really matter since you are the only user.)
    * OAuth redirect: ```https://127.0.0.1``` (Not gonna use redirect, so setting it to localhost is enough.)
    * Category: ```Analytics Tool```
1. Copy your Client ID (Do NOT share your client ID with anyone else)
1. Open your OBS Studio
1. Add Browser Source
    * URL: ```https://stinkingbanana.github.io/livestats/livestats.html?login={your twitch login ID}&clientID={your Client ID}&vc=0```
    * Width: 580
    * Height: 22

Additonal Display "country flag"
* Add ```?flag={country code}``` after the url if "```?```" was NOT previously used in the url
    * For example: United States
    * Before: ```https://stinkingbanana.github.io/livestats/livestats.html```
    * After: ```https://stinkingbanana.github.io/livestats/livestats.html?flag=us```
* Add ```&flag={country code}``` after the url if "```?```" was previously used in the url
    * For example: United States 
    * Before: ```https://stinkingbanana.github.io/livestats/livestats.html?login={your twitch login ID}&clientID={your Client ID}```
    * After: ```https://stinkingbanana.github.io/livestats/livestats.html?login={your twitch login ID}&clientID={your Client ID}&flag=us```
* The country code is in the format of [ISO 3166-1 alpha-2](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
* Add ```35``` to the original width or enough width util you see the flag

## Note
* "**current time**" and "**uptime**" take about 1~2 minutes to refresh / update after the stream started