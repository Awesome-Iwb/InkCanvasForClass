<div align="center">

[![LOGO](icc.png "LOGO")](# "LOGO")

# InkCanvasForClass

本項目基於ICA開發，ICA又基於IC開發

[![UPSTREAM](https://img.shields.io/badge/UpStream-WXRIW%2FInk--Canvas-red.svg "LICENSE")](https://github.com/WXRIW/Ink-Canvas)
![Gitea Last Commit](https://img.shields.io/gitea/last-commit/kriastans/InkCanvasForClass?gitea_url=https%3A%2F%2Fgitea.bliemhax.com%2F)
[![LICENSE](https://img.shields.io/badge/License-GPL--3.0-red.svg "LICENSE")](https://gitea.bliemhax.com/kriastans/InkCanvasForClass/src/branch/master/LICENSE)
[![交流群](https://img.shields.io/badge/-%E4%BA%A4%E6%B5%81%E7%BE%A4%20617707731-blue?style=flat&logo=TencentQQ)](https://qm.qq.com/q/AC777tzmEw)

![Screenshot-1](./Images/Ink-Canvas-For-Annotation%20Screenshot.png)
![Screenshot-2](./Images/Ink-Canvas-For-Annotation%20Blackboard%20Screenshot.png)

</div>

## 👀 前言
使用和分發本軟體前，請您應當且務必知曉相關開源協議，本軟體基於 https://github.com/ChangSakura/Ink-Canvas 修改而成，而ICA又基於 https://github.com/WXRIW/Ink-Canvas 修改而成，增添了包括但不限於隱藏到側邊欄等功能，更改了相關UI和軟體操作邏輯。對於墨跡書寫功能以及ICA獨有功能的相關 issue 提出，應優先查閱 https://github.com/WXRIW/Ink-Canvas/issues 。

[直接下載](https://gitea.bliemhax.com/kriastans/InkCanvasForClass/releases "Latest Releases")
——該安裝包使用 NodeJs+NodeGUI打包，默認配置適配絕大多數紅外觸摸框的設置。

> ⚠️注意：此項目仍在開發中，只會在發佈正式發行版時提供Release。您可以自行使用VS2022編譯打包後自行使用

## 特性
1. Support Active Pen (支持壓感)
2. 工具欄顯示了每個功能的文字描述
3. 添加了調色盤的顏色
4. 修復了一些IC和ICA不願修復（或沒空修復）的Bug
5. 添加了一些新功能，新特性

## Roadmap
[] 暗色模式（Dark Mode）
[] 動態主題色切換
[] 修復WXRIW/Ink-Canvas已修復的Bug
[] 橡皮大小菜單
[] 全新的幾何畫圖功能
[] 多背景色白板+稿紙背景
[] 白板頁面管理
[] 內置的PPT頁面管理
[] PPT提示是否為自動播放
[] ...

## 提示
- 對新功能的有效意見和合理建議，開發者會適時回復並進行開發。本軟體並非商業性質軟體，請勿催促開發者，耐心才能讓功能更少 BUG、更加穩定。
- 此軟體僅用於私人使用，請勿商用。更新也不會很快，如果有能力請PR貢獻程式碼而不是在Issue裡面提問題。

## FAQ

### 點擊放映後一翻頁就閃退？
考慮是由於`Microsoft Office`未啟用導致的，請自行啟用

### 放映後畫板程序不會切換到PPT模式？
如果你曾經安裝過`WPS`且在卸載後發現此問題則是由於暫時未確定的問題所導致，可以嘗試重新安裝WPS
> “您好，關於您回饋的情況我們已經回饋技術同學進一步分析哈，辛苦您可以留意後續WPS版本更新哈~” --回復自WPS客服

另外，處在保護（只讀）模式的PPT不會被識別

若因安裝了最新版本的 WPS 而導致無法在 WPS 軟體內進入 PPT 模式，可以嘗試卸載 WPS 後，並清除電腦垃圾、註冊表垃圾、刪除電腦上所有帶 "kingsoft" 名稱的文件夾，重新安裝 WPS 2021 後，（以上步驟可能有多餘步驟），經測試在 WPS 內可以正常進入 PPT 模式。

不支援WPS純淨版！

### **安裝後**程序無法正常啟動？
請檢查你的電腦上是否安裝了 `.Net Framework 4.7.2` 或更高版本。若沒有，請前往官網下載  
如果仍無法運行，請檢查你的電腦上是否安裝了 `Microsoft Office`。若沒有，請安裝後重試