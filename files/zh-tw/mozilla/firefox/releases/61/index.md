---
title: Firefox 61 技術變動摘要
slug: Mozilla/Firefox/Releases/61
translation_of: Mozilla/Firefox/Releases/61
---
{{FirefoxSidebar}}

此文章提供 Firefox 61 中與開發者較為相關之變動資訊。Firefox 61 預定於 [2018 年 6 月 26 日正式發表](https://wiki.mozilla.org/RapidRelease/Calendar#Future_branch_dates)。

## Web 開發相關變動

### 開發者工具

_無變動。_

### HTML

_無變動。_

### CSS

_無變動。_

### SVG

- {{SVGElement("a")}} 元素（{{domxref("SVGAElement")}}）新增 `ping`、`rel`、`referrerPolicy`、`relList`、`hreflang`、`type` 及 `text` 等屬性，以便與 HTML {{HTMLElement("a")}} 元素抱持一致。（{{bug("1451823")}}）
- {{SVGElement("textPath")}} 元素（{{domxref("SVGTextPathElement")}}）現在支援 SVG2 的 `path` 及 `side` 屬性。（{{bug("1446617")}} 與 {{bug("1446650")}}）
- 除 {{SVGElement("path")}} 之外，現在有更多元素支援{{domxref("SVGGeometryElement")}} 。（{{bug("1325320")}}）

### JavaScript

- 已實作 {{jsxref("String.prototype.trimStart()")}} 及 {{jsxref("String.prototype.trimEnd()")}} 方法（參考 {{bug(1434007)}}。為了確保相容性，將保留 `trimLeft` 和 `trimRight` 作為別名。

### API

#### 新 API

_無變動。_

#### DOM

- The {{domxref("Document.anchors", "anchors")}}, {{domxref("Document.applets", "applets")}}, {{domxref("Document.embeds", "embeds")}}, {{domxref("Document.forms", "forms")}}, {{domxref("Document.head", "head")}}, {{domxref("Document.images", "images")}}, {{domxref("Document.links", "links")}}, {{domxref("Document.plugins", "plugins")}}, and {{domxref("Document.scripts", "scripts")}} properties have been moved from the {{domxref("HTMLDocument")}} interface onto {{domxref("Document")}} ({{bug(1415588)}}).
- The {{domxref("Node.getUserData()")}} and {{domxref("Node.setUserData()")}} methods have been removed from the platform completely ({{bug(749981)}}).
- {{domxref("DOMTokenList.replace()")}} now returns a {{domxref("Boolean")}} to indicate whether the replacement occurred successfully, rather than void ({{bug(1444909)}}).

#### DOM 事件

_無變動。_

#### Service workers

_無變動。_

#### Media 及 WebRTC

{{domxref("AudioContext.AudioContext", "AudioContext()")}} 建構式現在可以選擇性傳入一個 {{domxref("AudioContextOptions")}} 型態的 `options` 參數，用以調整新的 AudioContext 下偏好的延遲時間及取樣率。

#### Canvas 及 WebGL

_無變動。_

### CSSOM

_無變動。_

### HTTP

- 已實作 cookie 管理中的 **`SameSite`**，見 [Set-Cookie](/en-US/docs/Web/HTTP/Headers/Set-Cookie) 及 [HTTP cookies](/en-US/docs/Web/HTTP/Cookies)。（{{bug(795346)}}）

### 安全性

_無變動。_

### 外掛程式

_無變動。_

### 其他

_無變動。_

## Web 平台中移除的項目

### HTML

_無變動。_

### CSS

_無變動。_

### APIs

_無變動。_

### SVG

- 從未良好實作且已為標準所廢棄的 {{domxref("SVGViewElement")}}`.viewTarget` 屬性已經移除。（{{bug(1455763)}}）
- 在標準規格中廢棄的下列屬性已經自 {{domxref("SVGSVGElement")}} 移除（{{bug(1133172)}}）：

  - `pixelUnitToMillimeterX`
  - `pixelUnitToMillimeterY`
  - `screenPixelToMillimeterX`
  - `screenPixelToMillimeterY`

- 不在標準規格內的 `SVGNumber()` 建構式已經移除。（{{bug("1455940")}}）

### 其他

_無變動。_

## 附加元件及 Mozilla 軟體開發相關變動

### WebExtensions

_無變動。_

## 請參見

- Firefox 61 網站相容資訊

## 舊版資訊

{{Firefox_for_developers(60)}}