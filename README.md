# OBS Config Import Tool / OBS 配置导入工具

[English](#english) | [繁體中文](#繁體中文)

---

## English

### Overview

OBS Config Import Tool is a Windows utility that allows you to easily import OBS Studio configuration files directly from GitHub or Gitee repositories.

### Features

- **Multi-platform Support**: Import from both GitHub and Gitee
- **Branch Detection**: Automatically detect branches from URLs
- **Auto Language**: Automatically detect and display in your system language (Chinese/English)
- **Auto Backup**: Automatically backup your current OBS configuration before importing
- **Simple Operation**: Just paste the repository URL

### Supported URL Formats

**GitHub:**
```
https://github.com/username/repo
https://github.com/username/repo/tree/dev
```

**Gitee:**
```
https://gitee.com/username/repo
https://gitee.com/username/repo/tree/dev
```

### Usage

1. Download `obs_config_loader.exe` from the `dist_new` folder
2. Double-click to run the program
3. Paste your repository URL when prompted
4. Press Enter to confirm or type `y` to use a custom branch
5. Restart OBS Studio to apply the new configuration

### Example Output

```
============================================
OBS Config Import Tool
============================================

Enter GitHub or Gitee repository URL: https://github.com/yourusername/obs-settings
Parse Result:
  Platform: GitHub
  Username: yourusername
  Repository: obs-settings
  Branch: main
Use custom branch? (y/N): N

Fetching config from GitHub...
Repository: https://github.com/yourusername/obs-settings
Branch: main
Download successful, extracting...
OBS config path: C:\Users\Username\AppData\Roaming\obs-studio
Backed up current config to: C:\Users\Username\AppData\Roaming\obs-studio_backup_20260526_123456
Importing config...
✓ Config imported successfully!
Please restart OBS to apply new config

Press Enter to exit...
```

### Requirements

- Windows OS
- OBS Studio installed
- Internet connection

### Repository Structure

Your repository should contain the OBS configuration files in the root directory:

```
your-repo/
├── config/
│   └── obs-studio/
│       └── ...
└── ...
```

The tool will extract and merge the contents into `%APPDATA%\obs-studio`.

---

## 繁體中文

### 簡介

OBS 配置導入工具是一款 Windows 應用程式，可以讓您輕鬆地從 GitHub 或 Gitee 倉庫直接匯入 OBS Studio 設定檔。

### 功能特點

- **多平台支援**：支援從 GitHub 和 Gitee 匯入
- **分支自動檢測**：從 URL 自動檢測分支名稱
- **自動語言**：根據系統語言自動切換中文/英文介面
- **自動備份**：匯入前自動備份現有 OBS 設定
- **操作簡便**：只需貼上倉庫連結

### 支援的 URL 格式

**GitHub：**
```
https://github.com/使用者名稱/倉庫名
https://github.com/使用者名稱/倉庫名/tree/開發分支
```

**Gitee：**
```
https://gitee.com/使用者名稱/倉庫名
https://gitee.com/使用者名稱/倉庫名/tree/開發分支
```

### 使用方法

1. 從 `dist_new` 資料夾下載 `obs_config_loader.exe`
2. 雙擊執行程式
3. 出現提示時貼上您的倉庫連結
4. 按 Enter 確認，或輸入 `y` 使用自訂分支
5. 重新啟動 OBS Studio 以套用新設定

### 範例輸出

```
============================================
OBS 配置導入工具
============================================

請輸入GitHub或Gitee倉庫連結: https://github.com/yourusername/obs-settings
解析結果:
  平台: GitHub
  使用者名稱: yourusername
  倉庫名: obs-settings
  分支: main
是否使用自訂分支? (y/N): N

正在從 GitHub 拉取配置...
倉庫: https://github.com/yourusername/obs-settings
分支: main
下載成功，正在解壓...
OBS配置路徑: C:\Users\Username\AppData\Roaming\obs-studio
已備份當前配置到: C:\Users\Username\AppData\Roaming\obs-studio_backup_20260526_123456
正在匯入配置...
✓ 配置匯入成功！
請重啟OBS以應用新配置

按回車鍵退出...
```

### 系統需求

- Windows 作業系統
- 已安裝 OBS Studio
- 網路連線

### 倉庫結構

您的倉庫根目錄應包含 OBS 設定檔：

```
your-repo/
├── config/
│   └── obs-studio/
│       └── ...
└── ...
```

工具會將內容解壓縮並合併到 `%APPDATA%\obs-studio`。

---

## License / 授權條款

MIT License
