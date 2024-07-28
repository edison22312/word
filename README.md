# v2board 潮汐客戶端
打包構建 WIN 客戶端 和 MAC 客戶端
![image](https://github.com/edison22312/word/blob/main/Screenshot%202024-07-28%20222918.png)

所需環境依賴
nodejs
electron
lectron-builder


環境搭建教程 以debian11 為列

打包環境安裝
nodejs安裝

```
sudo apt update

```

sudo apt install nodejs npm
node --version
npm --version


electron安裝

```
npm install electron --save-dev
```

electron-builder安裝

```
npm install electron-builder --save-dev
```

## 使用

在 srx/disk文件夾fake.js 修改您的網址名稱域名和登錄圖片

```
// 机场的地址url
var wangzhangurl = "你机场网址";
// 登录页面背景图
var loginBackgroundImageUrl = '图片url';
// 登录后的背景图
var headBackgroundImageUrl = '图片url';
```

index.html 修改app名稱
如果需要修改app的icon請在 package.json 裏面icon添加圖片路徑

自動打包在主目錄裏面 找到 build.sh 文件 ,請給與執行權限
`chmod +x build.sh`

```
bash build.sh
```





1、搜索 `$api-url$`、`$title$`、`$license$` 分别替换为你的站点地址、标题、授权码，授权码通过对 `站点地址` 做sha1运算然后加上 `1145141919` 再做sha1运算取得。
2、在 `res` 路径下放置你的图标文件。
3、安装 `Electron-builder`，执行 `bash build.sh`。

## 声明

本项目仅用于学习交流，使用者造成的一切问题均由使用者本人负责，与项目发起者、维护者、贡献者无任何关系。

