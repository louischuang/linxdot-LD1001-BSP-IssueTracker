# Linxdot LD-1001 BSP Issue Tracker

本 Repo 是 LD-1001 測試者的溝通與追蹤入口，用於回報 bug、討論新增功能、記錄修復更新與規劃。內容以可公開的功能與測試資訊為限。

## 三條開發線

| 項目 | 已確認的最新版本 | 現況與重點 |
| --- | --- | --- |
| [OpenWrt 5.x](openwrt-5.x/README.md) | 2.0.0.16-OPEN / Linux 5.15.173 | 既有功能維護；整合 NPU 穩定性修正 |
| [OpenWrt 6.x](openwrt-6.x/README.md) | V3.0 Beta-2026.09.28（r4） / OpenWrt 25.12.5 / Linux 6.12.94 | Beta；攝影機 Dashboard、A/B 更新及設定保存、SFTP |
| [Android](android/README.md) | Android 11 BSP v0.6.1 / Rockchip 4.19 系列核心 | AOSP 開發板測試候選；維修主控台與 USB 相機方向修正 |

資料核對日：**2026-11-23**。最新已確認更新分別為 2026-08-31、2026-09-28、2026-08-31；本次整理未重新執行硬體測試。Beta／測試候選仍有待驗收項目，詳見各線文件。

## 閱讀 HTML 簡介

[HTML 總覽](index.html) 提供簡介及三條開發線導覽。GitHub 檔案頁通常顯示 HTML 原始碼；將此 Repo 下載或 clone 至本機後，以瀏覽器開啟 `index.html` 即可閱讀，無需安裝套件。所有頁面使用本地樣式，不依賴外部字型或腳本。

## 目錄

```text
index.html                 HTML 總覽
assets/                    共用文件樣式
openwrt-5.x/               既有 OpenWrt 維護線
openwrt-6.x/               新版 OpenWrt Beta 線
android/                   Android AOSP 開發板線
```

每條線皆有 `README.md`、`index.html`（簡介）、`technical.html`（技術與測試說明）、`updates.html`（修復與更新）、`patches/`（經審核可公開的修補）及 `features/`（功能提案）。目前沒有放入實際 patch；功能規劃不代表已交付或已承諾時程。

## 協作方式

- Bug：使用 [Bug 回報](https://github.com/louischuang/linxdot-LD1001-BSP-IssueTracker/issues/new?template=bug_report.yml)，一個 Issue 聚焦一項問題。
- 功能：使用 [功能提案](https://github.com/louischuang/linxdot-LD1001-BSP-IssueTracker/issues/new?template=feature_request.yml)，描述使用情境與可驗收結果。
- 驗收：回報修復版本、重測步驟及結果，由維護者確認後結案。

請先閱讀 [CONTRIBUTING.md](CONTRIBUTING.md)。勿張貼內部開發 Repo、主機、登入資訊、環境配置、內部路徑或產物細節；紀錄與截圖請先去識別化。本 Repo 不提供內部開發、建置或部署資訊。
