+++
title = 'Blog 開張!'
date = 2024-08-22T14:10:09+08:00
draft = true
tags = ["Hugo"]
categories = ["Blog"]
+++


# 前言

想搞個 blog 紀錄點東西很久了，常聽說的架站工具至少有 `WordPress`、`Hexo`、`Hugo`等。

久未開始動手的主因之一，就是感覺這些東西安裝起來應該會佔不少空間，尤其是 `WordPress`，要裝資料庫又要裝網頁伺服器等等，對於只用一台小筆電以及不想租用雲端主機的我而言，
顯然不適合。

又如 `Hexo`，看起來是要安裝 `Node.js` 才能用， 而 `Node.js` 是一套完整的框架，為了架個 blog 安裝一個框架，跟 `WordPress` 一樣使人感覺臃腫。

當然，也有現成的網頁版操作型 blog，以技術類來說，最常見的就是 `Medium`，不過好像不太能順暢地使用 Markdown、Latex、Mermaid 這些好用的語法，也不太能客製化頁面樣式。
又近來網民對於 `Medium` 之抱怨也越來越多(關鍵字搜尋一下應該可發現)，所以我也不打算用它。

看起來只剩 `Hugo` 了，但略有耳聞它是由 `Go` 語言編寫，想到為了寫 blog，可能要安裝及學習一套新語言，又有點望而卻步。

所幸，`Hugo` 有編譯好的程式(exe 檔)可以直接下載使用，下載解壓縮後僅 80 多 MB，相對前述的架站方法而言明顯輕量許多!

### 最終，我選擇了 `Hugo` + `GithubPage` 做為架 blog 之主要工具!

由於我除了 `Markdown` 外還希望可以有下列功能：

- Latex 撰寫數學式
- Mermaid 畫流程圖
- Disqus 簡易評論系統

難免需要進行微調，隨然 `Hugo` 由 `Go` 語言開發，但其實可以完全不用知道 `Go` 語法，稍微了解一下 `Hugo` 設計架構就可進行微調!

以下就簡要紀錄一下使用 `Hugo` 並達成上述要求來搭建 blog 一些需要留意的地方。

---

# Hugo notes

## 下載 Hugo binary for Windows

[Hugo Github Release 下載地址](https://github.com/gohugoio/hugo/releases)

## 建立一個 site

```
hugo new site MyBlog
```

這個命令會在當前資料夾下創建一個 `MyBlog` 的資料夾