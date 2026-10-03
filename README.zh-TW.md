# 特殊物品封鎖系統

[English](README.md) | **繁體中文**

保護獎勵與活動道具：名稱含禁用關鍵字的物品不能用於合成、不能放進鐵砧，一般物品也不能被改名成這類名稱。

> 本儲存庫包含同一個腳本的兩個版本：**繁體中文（zh-TW）** 是作者伺服器實際使用的原始版本；**English** 為完整英文翻譯版（指令、訊息與變數名稱皆為英文），功能相同。

## 功能特色

- 可自行編輯的關鍵字清單（跑酷、獎杯、活動、VIP、管理、測試……）
- 合成材料中只要有受保護名稱的物品就取消合成
- 在鐵砧中把物品命名成含關鍵字的名稱時，無法取出
- 禁止把特殊物品放進鐵砧（一般點擊與 Shift 點擊）
- 以聊天訊息、動作列與音效提示玩家

## 需求

- [Paper](https://papermc.io/) 伺服器（開發環境 Paper 26.2 / Minecraft 26.2）
- [Skript](https://github.com/SkriptLang/Skript)（開發環境 2.16.2）

## 安裝

1. 先安裝[需求](#需求)中列出的插件。
2. 下載**其中一個**版本：

   | 版本 | 檔案 |
   |---|---|
   | 繁體中文（原始版本） | [`zh-TW/特殊物品封鎖系統.sk`](zh-TW/%E7%89%B9%E6%AE%8A%E7%89%A9%E5%93%81%E5%B0%81%E9%8E%96%E7%B3%BB%E7%B5%B1.sk) |
   | English（英文） | [`en/special-item-lock.sk`](en/special-item-lock.sk) |

3. 把 `.sk` 檔案放進伺服器的 `plugins/Skript/scripts/`。
4. 執行 `/sk reload 特殊物品封鎖系統`（請換成你放入的檔名），或重新啟動伺服器。

> [!IMPORTANT]
> **只能安裝其中一個版本。** 兩個版本是同一個腳本的不同語言，同時載入會互相衝突或重複執行。

## 指令

本腳本沒有指令，會自動執行。

## 設定

- 在 `on script load` 區塊修改清單。比對方式為「名稱包含關鍵字」且不分大小寫。

## 注意事項

- 只會檢查有自訂名稱的物品。
- 關鍵字請與其他腳本使用的獎勵物品名稱保持一致，例如 [skript-parkour-reward-chest-refill](https://github.com/Im-Tim-mI/skript-parkour-reward-chest-refill)。
- 英文版使用另一份英文關鍵字清單。

## 相關專案

- [skript-parkour-reward-chest-refill](https://github.com/Im-Tim-mI/skript-parkour-reward-chest-refill)－主世界跑酷獎勵寶箱填充
- [skript-achievement-display](https://github.com/Im-Tim-mI/skript-achievement-display)－成就顯示
- [skript-tester-thank-you-kit](https://github.com/Im-Tim-mI/skript-tester-thank-you-kit)－測試人員感謝套裝發放
- [skript-test-gear-distribution](https://github.com/Im-Tim-mI/skript-test-gear-distribution)－測試裝備發放系統

## 授權

**MIT + Commons Clause**，完整條款請見 [LICENSE](LICENSE)。

- ✅ 可自由使用、複製、修改與分享本腳本。
- ✅ 本授權明確允許在收費或營利的 Minecraft 伺服器上安裝與運行本插件（含修改版）。
- ❌ 禁止的僅限於直接或間接販售本插件本體、修改版本，或以付費方式取得其檔案或原始碼。

Copyright (c) 2026 廷廷小教室、廷廷的家（Tim945）
