# 🍏 macOS 開發環境配置

這個檔案是我的 Homebrew 設定 (`Brewfile`)，可以幫助我快速建立 macOS 開發環境，包括常用的指令工具、應用程式，以及 VS Code 擴充功能。

---

## 📌 **安裝指南**

### **1️⃣ 安裝 Homebrew**
如果你的 macOS 尚未安裝 Homebrew，請先執行以下指令：
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### **2️⃣ 設定 Homebrew**
執行以下指令來安裝 `Brewfile` 中的所有套件：
```sh
brew bundle --file="~/.config/brew_seed/Brewfile"
```

如果沒有指定 `--file`，`brew bundle` 會預設使用當前目錄下的 `Brewfile`。

---

## 🛠️ **安裝內容**

### 🍺 **Homebrew 安裝的工具**
| 類別         | 軟體名稱       | 說明 |
|-------------|--------------|-------------|
| CLI 工具    | `bat`        | 進階版 `cat`，支援語法高亮 |
| CLI 工具    | `fd`         | 更快速、更直覺的 `find` 替代方案 |
| CLI 工具    | `tree`       | 以樹狀結構顯示目錄 |
| 開發工具    | `neovim`     | 現代化 Vim 編輯器 |
| 開發工具    | `ripgrep`    | 高效文字搜尋工具（類似 `grep`） |
| Git 工具    | `lazygit`    | 直覺的 Git 介面 |
| 影像處理    | `imagemagick` | 圖片轉換與處理工具 |
| 影音工具    | `ffmpeg`     | 播放、錄製、轉換音訊與影片 |
| 影像工具    | `chafa`      | ASCII/ANSI 圖片轉換工具 |
| 編譯工具    | `autoconf`   | 生成 `configure` 腳本 |
| 編譯工具    | `automake`   | 生成 GNU 標準 `Makefile` |
| 編譯工具    | `pkgconf`    | 編譯與連結工具 |
| 檔案管理    | `viu`        | 在終端顯示圖片 |
| 系統工具    | `mas`        | Mac App Store CLI 工具 |
| 安裝工具    | `makensis`   | 建立 Windows 安裝包 |
| 簽章工具    | `osslsigncode` | OpenSSL Authenticode 簽署 |
| 依賴管理    | `libtool`    | 通用函式庫管理工具 |

---

### 🖥️ **VS Code 擴充功能**
這些擴充功能將透過 `vscode` 指令安裝，以提升開發體驗。

#### **🔧 開發與格式化**
- `dbaeumer.vscode-eslint` - ESLint 程式碼檢查
- `esbenp.prettier-vscode` - Prettier 程式碼格式化
- `rvest.vs-code-prettier-eslint` - Prettier & ESLint 整合
- `stylelint.vscode-stylelint` - CSS / SCSS / LESS 格式檢查
- `standard.vscode-standard` - JavaScript Standard 樣式檢查

#### **🛠️ 版本控制 & Git**
- `eamodio.gitlens` - 增強 Git 支援
- `mhutchie.git-graph` - Git 視覺化歷史
- `donjayamanne.githistory` - 查看檔案的 Git 變更記錄

#### **💻 語言與框架**
- `infeng.vscode-react-typescript` - React & TypeScript 支援
- `styled-components.vscode-styled-components` - Styled Components 支援
- `ms-playwright.playwright` - Playwright 測試框架支援

#### **📦 其他工具**
- `bierner.markdown-mermaid` - Markdown Mermaid 圖表支援
- `simonsiefke.svg-preview` - SVG 圖片預覽
- `pkief.material-icon-theme` - Material Design 圖標主題
- `equinusocio.vsc-material-theme` - Material Theme UI 主題

---

## 🔄 **如何更新這些工具**
### **更新 Homebrew 及所有套件**
```sh
brew update && brew upgrade && brew cleanup
```

---

