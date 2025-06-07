# rime-jyutsp-loengfan
jyutsp-goi - 粵語雙拼+两分輔助碼輸入法方案。 / 粤语双拼 + 两分码 方案 / Rime Cantonese mixed leongfan two-key per character(Double Pinyin) input schema

基於[rime-jyutsp-real jyutsp-real 粵語雙拼輸入法（純雙拼真雙拼方案）](https://github.com/yuOpghH/rime-jyutsp-real)的改進，在雙拼基礎上添加以[粵語兩分](https://github.com/CanCLID/rime-loengfan)的輔助碼。

 兩分即是將字拆為兩部通過輸入

 基於兩分輔助碼下，幾乎即見即拆輸出輔助碼，在入門成本大降情況下，大大加強單字輸入、組詞分別的能力（但由於不存在固頂字詞、對輔助碼重複部份無特別優化排重固定作序。）。
 
 默認輸出台灣標準正體、僅提供最基礎單字快碼。極簡配置：無有固定字詞、無簡拼、最簡詞表。
 
 反查：`Q:`倉頡反查 `W:`粵拼反查 `E:`普拼反查（假如有選用的話）

#### 兩分是何物？
 - 例：蒜 = 艹 (cou2) + 示 (si6)
   - in jyutsp-leongfan：`蒜 = s + r(yun) + c (艹cou2) + s(示si6) = srcs`
 - 注意（與原兩分的差異）：
   <br>為了降低重碼率，<br>兩分拆分字音作以下調整：`gw > x`， `kw > q` ， `ng > r`
    - 例：`啩（gwaa） = x(gw) + a(aa) + h(口hau) + <b>x(卦gwaa)</b> = xahx`


##### 感興趣的話歡迎瀏覽其他方案版本：

| 粵語雙拼方案 | 學習成本 | 揀字率 | 連續雙碼長句輸出 | 單字快碼 | 輔助碼篩選字詞 | 字詞固頂 | 簡拼輸出
| :------- | ------: | -------: |  -------: |  -------: |  -------: |  -------: |  -------: | 
| [jyutsp-real <br>粵語雙拼<br>純雙拼](https://github.com/yuOpghH/rime-jyutsp-real)  | 低。僅需記憶鍵位映射 | 大量重複音節 | ✓ | ✓ |  |  | 
| [jyutsp-loengfan<br>粵語雙拼<br>兩分輔助碼](https://github.com/yuOpghH/rime-jyutsp-loengfan)   | 較低。幾乎可見可拆 | 能初步篩選同部首 | ✓ | ✓ | ✓ |  | 
| [jyutsp-real<br>粵語雙拼<br>倉頡輔助碼](https://github.com/yuOpghH/rime-jyutsp-goi)  | 較高。120個倉頡字母 | 三千字內5.8% | ✓ | ✓ | ✓ | ✓ | ✓ |

 ## 使用
下載安裝[Rime](https://rime.im/)，部署到“用户文件夾”，“輸入法設定”選中本方案，部署即可
   
## 致謝
- 感謝以下項目的無私貢獻及項目成果。可能有遺漏敬請原諒。
 - 鍵盤設置來源：[jyutsp粵語雙拼](https://github.com/MrCorn0-0/jyutsp/)
 - 輔助碼：[粵語兩分](https://github.com/CanCLID/rime-loengfan)

# 輸入編碼
## 碼表

[![zhihu]](https://www.zhihu.com/question/54691506/answer/1022245649)

[zhihu]:https://github.com/yuOpghH/rime-jyutsp-goi/blob/main/%E5%B1%95%E7%A4%BA/keyboard.jpg "碼表"

- 鍵位與原雙拼方案碼表的差異：
  - j鍵開頭的音節變成以y鍵輸出為主
  - j鍵兼容y鍵聲母輸出(而非兼容z鍵)
  - v鍵兼容z鍵聲母輸出

# 學習文檔
沿用[jyutsp_goi粵語雙拼倉頡輔助碼輸入法](https://github.com/yuOpghH/rime-jyutsp_goi)的說明文檔：

[極速跟打器學習文檔下載](https://github.com/yuOpghH/rime-jyutsp_goi/blob/main/%E6%A5%B5%E9%80%9F%E8%B7%9F%E6%89%93%E5%99%A8.rar)

[木易跟打器學習文檔下載](https://github.com/yuOpghH/rime-jyutsp_goi/tree/main/%E6%9C%A8%E6%98%93%E8%B7%9F%E6%89%93%E5%99%A8)

- 4，（學習文檔）
  - 4.1 此法適合從零開始用家。配置文檔兼有雙拼鍵位、倉頡字根學習練習，用家可自擇自行下載部署好[極速跟打器](http://www.jsxiaoshi.com/)後，下載極速跟打器.rar按照路徑部署相關檔案，在設置內更換好”編碼文件“。即可使用“練習→字根練習”“發文→文章→繁體常用單字”等相關教程學習。(注：該程序不兼容粵字，練習請用繁體常用單字)
  - 4.2 此法適合有基礎用家。無需安裝程式線上使用。用家可打開雲端 [木易跟打器](https://typer.owenyang.top/) ，然後[學習資料](https://github.com/yuOpghH/rime-jyutsp_goi/tree/main/%E6%9C%A8%E6%98%93%E8%B7%9F%E6%89%93%E5%99%A8) 資料夾內的資料配置進去，將 “jyutspgoi 3500字粵音常用字試驗方案.txt”文本拖進 功能/設置/碼表設置中保存，在同頁面打開“編碼提示”，然後在“跟打”複製貼上“粵音常用字%203500字順序.txt”，即可練習。
 
