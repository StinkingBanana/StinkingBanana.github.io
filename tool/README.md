# OBS 直播時間 觀眾人數 顯示器

## 預覽"
<p><img src="twitchVC_preview.png"></p>

## 工具網址
[https://stinkingbanana.github.io/tool/twitchVC.html](https://stinkingbanana.github.io/tool/twitchVC.html)


## 參數
* ```login``` = {你的Twitch登入帳號}
* ```clientID``` = {你的用戶端 ID}
* ```flag``` = {國家代碼}

## 使用方式

#### 以下設置是假設你的OBS的畫布大小是1920x1080為前提

如果你只是需要日期與時間
* 打開你的OBS Studio
* 加入瀏覽器來源
    * 網址: ```https://stinkingbanana.github.io/tool/twitchVC.html```
    * 寬度: 440
    * 高度: 22

如果除了日期時間你還需要觀看人數與直播時間
* 從Twitch開發人員網站取得你自己的**用戶端 ID** ```https://glass.twitch.tv/console/apps```
* 從APP頁面註冊您的應用程式
    * 名稱: ```Yourname's ViewerCount Display``` (任何名稱只要不跟他人的重複，不是很重要)
    * OAuth 重新導向網址: ```https://127.0.0.1``` (不會使用到重新導向，所以我們直接導向回localhost就可以了)
    * 分類: ```Analytics Tool```
* 新增完新的APP之後點進去複製**用戶端 ID** (請勿與他人分享自己的用戶端ID)
* 打開你的OBS Studio
* 加入瀏覽器來源
    * 網址: ```https://stinkingbanana.github.io/tool/twitchVC.html?login={你的Twitch登入帳號}&clientID={你的用戶端 ID}```
    * 寬度: 645
    * 高度: 22

如果除了日期時間你還需要直播時間，但是不想要顯示觀看人數
* 從Twitch開發人員網站取得你自己的**用戶端 ID** ```https://glass.twitch.tv/console/apps```
* 從APP頁面註冊您的應用程式
    * 名稱: ```Yourname's ViewerCount Display``` (任何名稱只要不跟他人的重複，不是很重要)
    * OAuth 重新導向網址: ```https://127.0.0.1``` (不會使用到重新導向，所以我們直接導向回localhost就可以了)
    * 分類: ```Analytics Tool```
* 新增完新的APP之後點進去複製**用戶端 ID** (請勿與他人分享自己的用戶端ID)
* 打開你的OBS Studio
* 加入瀏覽器來源
    * 網址: ```https://stinkingbanana.github.io/tool/twitchVC.html?login={你的Twitch登入帳號}&clientID={你的用戶端 ID}&vc=0```
    * 寬度: 580
    * 高度: 22

如果你需要顯示國旗
* 如果網址裡面**沒有**使用過問號"```?```" 請在網址後面添加 ```?flag={國家代碼}```
    * 舉例: 臺灣 
    * 修改前: ```https://stinkingbanana.github.io/tool/twitchVC.html```
    * 修改後: ```https://stinkingbanana.github.io/tool/twitchVC.html?flag=tw```
* 如果網址裡面**有**使用過問號"```?```"  請在網址後面添加 ```&flag={國家代碼}```
    * 舉例: 臺灣
    * 修改前: ```https://stinkingbanana.github.io/tool/twitchVC.html?login={你的Twitch登入帳號}&clientID={你的用戶端 ID}```
    * 修改後: ```https://stinkingbanana.github.io/tool/twitchVC.html?login={你的Twitch登入帳號}&clientID={你的用戶端 ID}&flag=tw```
* 國家代碼請參照 [ISO 3166-1 alpha-2](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
* 請在原來的寬度再加上 ```35``` 或是 足夠的寬度直到你看見國旗顯示出來

# OBS Twitch Viewer Count, Uptime, Date and Time Display

## TO USE

#### This setup assumes your OBS is using canvas size of 1920x1080

If you just need the date and clock,  
* Open your OBS Studio
* Add Browser Source
    * URL: ```https://stinkingbanana.github.io/tool/twitchVC.html```
    * Width: 440
    * Height: 22

If you need viewer count and uptime,
* Get your cliendID through Twitch Dev Console ```https://glass.twitch.tv/console/apps```
* Register New App
    * Name: ```Yourname's ViewerCount Display``` (Any unique name, does not really matter since you are the only user.)
    * OAuth redirect: ```https://127.0.0.1``` (Not gonna use redirect, so setting it to localhost is enough.)
    * Category: ```Analytics Tool```
* Copy your Client ID (Do NOT share your client ID with anyone else)
* Open your OBS Studio
* Add Browser Source
    * URL: ```https://stinkingbanana.github.io/tool/twitchVC.html?login={your twitch login ID}&clientID={your Client ID}```
    * Width: 645
    * Height: 22

If you need uptime, but does NOT need viewer count
* Get your cliendID through Twitch Dev Console ```https://glass.twitch.tv/console/apps```
* Register New App
    * Name: ```Yourname's ViewerCount Display``` (Any unique name, does not really matter since you are the only user.)
    * OAuth redirect: ```https://127.0.0.1``` (Not gonna use redirect, so setting it to localhost is enough.)
    * Category: ```Analytics Tool```
* Copy your Client ID (Do NOT share your client ID with anyone else)
* Open your OBS Studio
* Add Browser Source
    * URL: ```https://stinkingbanana.github.io/tool/twitchVC.html?login={your twitch login ID}&clientID={your Client ID}&vc=0```
    * Width: 580
    * Height: 22

If you need to display country flag
* Add ```?flag={country code}``` after the url if "```?```" was NOT previously used in the url
    * For example: United States
    * Before: ```https://stinkingbanana.github.io/tool/twitchVC.html```
    * After: ```https://stinkingbanana.github.io/tool/twitchVC.html?flag=us```
* Add ```&flag={country code}``` after the url if "```?```" was previously used in the url
    * For example: United States 
    * Before: ```https://stinkingbanana.github.io/tool/twitchVC.html?login={your twitch login ID}&clientID={your Client ID}```
    * After: ```https://stinkingbanana.github.io/tool/twitchVC.html?login={your twitch login ID}&clientID={your Client ID}&flag=us```
* The country code is in the format of [ISO 3166-1 alpha-2](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
* Add ```35``` to the original width or enough width util you see the flag