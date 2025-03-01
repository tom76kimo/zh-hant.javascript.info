# 現代化 JavaScript 教程繁體中文版

這個 repository 存放網站 <https://zh-hant.javascript.info> 的繁體中文翻譯版

**貢獻流程:**

- 查看 [繁體中文翻譯進度 issue (Chinese Traditional Translation Progress)](https://github.com/javascript-tutorial/zh-hant.javascript.info/issues/1)。
- 選一篇 **尚未 (正在/完成) 翻譯** 的文章。
- 在 [繁體中文翻譯進度 issue (Chinese Traditional Translation Progress)](https://github.com/javascript-tutorial/zh-hant.javascript.info/issues/1) 底下留言該文章的標題，例如 `An Introduction to JavaScript`。
    - **記得你的留言內容只要留文章標題就好！** 。
    - Bot 將會在此 issue 內該篇文章之後標示你的 id，讓大家都知道你正在翻譯該文章。
    - Fork 此 repository，完成翻譯文章後發一個 PR。
    - PR 標題要與文章標題一致，bot 將會把該 PR 連結至 issue 之中。

請等待維護者審核，將會請你修改或合併你的翻譯。

如果維護者沒有回應，或是你想成為維護者之一，請至 [主要 repository](https://github.com/javascript-tutorial/en.javascript.info/issues/new) 聯繫。

**讓其他人知道你正在翻譯這份教程，甚至可以邀請他們一起加入！**

🎉 感激不盡！

你的名字和貢獻量將會在翻譯釋出後，出現在 "[關於本計畫](https://zh-hant.javascript.info/about)" 頁面上。

註：完整的多國語言翻譯列表可以在 <https://javascript.info/translate> 之中找到

## 文件結構

每個章節、文章、或課題都在專屬的檔案夾中。

該檔案夾會以 `N-url` 的方式命名，其中 `N` 代表序號 (文章有經過排序)，而 `url` 是該網站上對應的 *URL-slug*。

檔案夾中會有以下其中一種檔案：

- `index.md` 對應一個章節,
- `article.md` 對應一篇文章,
- `task.md` 對應一個課題 (若有解答就也會有 `solution.md` 這個檔案)

一個檔案將以 `# 標題` 開始，然後內文以類 Markdown 的格式用簡單編輯器即可編輯。

文章與課題需要的額外資源和範例也可以在同一個檔案夾中找到。

## 翻譯提示

請保持原始的斷行與段落，不要加入或移除任何行或段落，這將有助於整合未來英文版的改動。

如果你看到英文版可以加強的部分，很好，請送 PR 給[英文版](https://github.com/javascript-tutorial/en.javascript.info/pulls)。

### 詞彙

- 一些特定的詞彙不需要翻譯，例如 "Function Declaration"。

- 其他詞彙像是 `resolved promise`, `slash`, `regexp` 等等，請先找找本 repository wiki 內的[「英文－繁中」用語對照表](https://github.com/javascript-tutorial/zh-hant.javascript.info/wiki/%E3%80%8C%E8%8B%B1%E6%96%87%EF%BC%8D%E7%B9%81%E4%B8%AD%E3%80%8D%E7%94%A8%E8%AA%9E%E5%B0%8D%E7%85%A7%E8%A1%A8)是否已有對應的詞彙，若沒有近似的詞彙，則尋找其他教程 (如：[MDN](https://developer.mozilla.org/en-US/)) 的翻譯。

- 專有詞彙翻譯完，在其後方空一格半形空白並補上原詞彙，例如：同源政策 (Same Origin Policy) 或轉譯 (transpile)，等等。
    - 若一篇文章出現兩次以上相同專有詞彙，則在第一次之後補上原詞彙即可。

- 若都無法找到對應的詞彙翻譯，請直接留下原文詞彙。

### 詞彙含義

在英文中很多詞彙有明顯的含義在內，但對於一個不瞭解英文的人來說，該含義會被忽略。

請謹記有必要時可以多加解釋或增加額外的翻譯，例如：

```md
`ReadableStream` objects allows to read data chunk-by-chunk.
```

```md
`ReadableStream` objects 允許一個個資料塊 (chunk) 地讀取資料
```

### 標點符號

- 本翻譯教程以使用中文符號為主，除了空白 ` `、括號 `(`、引號 `'` / `"`。例如：`"strict data typing"` -> `"強型態確認 (strict data typing)"`

- **強調***語句* 、半型符號和原文，前/後若為全型文字則需留一空白，若為全型標點符號則不需留空白。

- 英語一句話只能有一個逗號，但中文無此限制，可依據語氣通順程度將一些英文句點轉為逗號。

- 列舉項目後的文字須加句點。<- 像這樣


### 內文中的程式區塊

**本翻譯教程以不翻譯語法和對應的圖片為原則。**

- 只翻譯註解與範例字串
- 不要翻譯變數 (variables)、類別 (classes) 和識別符 (identifiers)
- 確保程式在翻譯後可以正確執行 :)

例如:

```js
// Example
const text = "Hello, world";
document.querySelector('.hello').innerHTML = text;
```

✅ 請這樣翻 (翻譯註解):

```js
// 範例
const text = 'Hello, world';
document.querySelector('.hello').innerHTML = text;
```

❌ 別翻成 (不要翻譯類別):

```js
// 範例
const text = 'Hello, world';
// ".hello" 是一個類別
// 別翻成這樣
document.querySelector('.嗨').innerHTML = text;
```

請注意，有時候程式區塊之後會接著圖片，若你在程式區塊中翻譯了 `Hello` 成 `嗨`，那你必須也修改圖片中的字。

所以在這種情況下不翻譯該文字是更好的選擇。

### 外部連結

**本翻譯教程以維持原本外部連結為原則。**

若一個外部連結是連到 Wikipedia，如：`https://en.wikipedia.org/wiki/JavaScript`，且該文章有你使用語言的優良版本，可以將連結連到該版本。

例如:

```md
[JavaScript](https://en.wikipedia.org/wiki/JavaScript) is a programming language.
```

✅ OK (en -> zh):

```md
[JavaScript](https://zh.wikipedia.org/wiki/JavaScript) 是一種程式語言。
```

MDN 的連結可以使用部分翻譯的版本。

若一個外部連結的文章沒有翻譯過的版本，則維持原本連結。

### 詮釋資料

一些檔案，通常是課題，頂端會有 YAML 的詮釋資料 (metadata) 並以 `---` 分隔：

```md
importance: 5

---
...
```

請不要翻譯 "importance" (和其他放在頂端的詮釋資料)。

### Anchors

有些標題接著 `[#anchor]`，如：

```md
## Spread 運算子 [#spread-operator]
```

請不要翻譯或移除該 `[#...]` 部分，這是 URL anchors 用的。

## 本地運行

你可以在本地運行此教程的伺服器來看看翻譯得如何。

伺服器安裝指南請參考 <https://github.com/javascript-tutorial/server>

---
繁體中文版的維護者們 🚀

- Arvin Huang [@arvin0731](https://github.com/arvin0731)
- Jason Huang [@kaddopur](https://github.com/kaddopur)
- Len Chen [@lenchen1112](https://github.com/lenchen1112)
- Tom Wu [@tom76kimo](https://github.com/tom76kimo)

