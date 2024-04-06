<p align="center">獻給想為 Glyphs 創作工具的人</p>

# 前言

這是字型設計軟體 [Glyphs](https://glyphsapp.com/) 工具程式撰寫相關的專案。
前陣子看到 [官網論壇](https://forum.glyphsapp.com/t/glyphs-python-interpreter/25481) 有人在討論在 VisualStudio Code（以下簡稱 VSCode）撰寫程式碼時，透過 .pyi 格式能產生懸浮視窗說明文字的效果。剛好自己也有這方面的需求，就想到將 [官方的 Python API 架構文件](https://docu.glyphsapp.com/) 翻譯成中文，並將它搬到 .pyi 檔案中。

<img width="1140" alt="image" src="https://github.com/yintzuyuan/GlyphsApp-Stubs_zh-tw/assets/83154914/5a5b9e8d-65ad-431b-b785-3cde8974e44a">

# 安裝方式

.pyi 檔案能支援大部分程式撰寫工具使用，每款安裝方法可能不同，這裡以 VSCode 舉例：
1. 在 VSCode 的延伸模組區安裝 Pylance。
2. 下載本專案資料夾的 .pyi 檔（可改名或放在其他資料夾）
3. 在 VSCode 中按`shift+cmd+P`搜尋`setting json`找到使用者設定的JSON檔。
4. 將以下程式碼加入JSON文件 `"python.analysis.stubPath": "pyi放的路徑位置",` 
5. 在你正在撰寫的腳本中加入`from 剛剛的pyi檔(不用副檔名) import *` 

# 附註
目前第一版內容已經大致完成，因為是一人作業，若有發現任何疏漏或是改進的建議（檔案格式、語句詞彙疏漏或是閱讀排版）都歡迎透過 [issues 分頁](https://github.com/yintzuyuan/GlyphsApp-Stubs_zh-tw/issues) 提出意見。
