# Special Item Lock

**English** | [繁體中文](README.zh-TW.md)

Protects reward and event items: items whose custom name contains a banned keyword can't be used for crafting or put into an anvil, and normal items can't be renamed to look like them.

> This repository has two editions of the same script: **繁體中文 (zh-TW)** is the original used on the author's Traditional Chinese server, and **English** is a full translation (commands, messages and variable names) with the same features.

## Features

- Editable keyword list (Parkour, Trophy, Event, VIP, Admin, Test, …)
- Cancels crafting when any ingredient has a protected name
- Blocks taking an item out of the anvil when the new name contains a keyword
- Blocks putting special items into the anvil (click and shift-click)
- Feedback through chat, action bar and sound

## Requirements

- [Paper](https://papermc.io/) server (developed on Paper 26.2 / Minecraft 26.2)
- [Skript](https://github.com/SkriptLang/Skript) (developed on 2.16.2)

## Installation

1. Install the plugins listed under [Requirements](#requirements).
2. Download **one** edition:

   | Edition | File(s) |
   |---|---|
   | English | [`en/special-item-lock.sk`](en/special-item-lock.sk) |
   | 繁體中文 (original) | [`zh-TW/特殊物品封鎖系統.sk`](zh-TW/%E7%89%B9%E6%AE%8A%E7%89%A9%E5%93%81%E5%B0%81%E9%8E%96%E7%B3%BB%E7%B5%B1.sk) |

3. Copy the `.sk` file(s) into `plugins/Skript/scripts/` on your server.
4. Run `/sk reload special-item-lock` (use the file name you copied) or restart the server.

> [!IMPORTANT]
> Install **only one** edition. Both editions are the same script in different languages - loading both makes them clash or run twice.

## Commands

This script has no commands - it runs automatically.

## Configuration

- Edit the list in the `on script load` block. Matching is a case-insensitive “name contains keyword”, so short English words can also match longer ones (e.g. `Test` also matches `Contest`).

## Notes

- Only items with a custom name are checked.
- Keep the keywords in sync with the reward item names used by your other scripts, e.g. [skript-parkour-reward-chest-refill](https://github.com/Im-Tim-mI/skript-parkour-reward-chest-refill).
- The English edition uses its own English keyword list.

## Related projects

- [skript-parkour-reward-chest-refill](https://github.com/Im-Tim-mI/skript-parkour-reward-chest-refill) - Parkour Reward Chest Refill
- [skript-achievement-display](https://github.com/Im-Tim-mI/skript-achievement-display) - Achievement Display
- [skript-tester-thank-you-kit](https://github.com/Im-Tim-mI/skript-tester-thank-you-kit) - Tester Thank-You Kit
- [skript-test-gear-distribution](https://github.com/Im-Tim-mI/skript-test-gear-distribution) - Test Gear Distribution

## License

**MIT + Commons Clause** - see [LICENSE](LICENSE) for the full text.

- ✅ You may use, copy, modify and share this script.
- ✅ You **may** install and run it - including modified versions - on Minecraft servers that charge money or are run for profit.
- ❌ You may **not** sell the script itself or modified versions of it, directly or indirectly, or require payment to obtain its files or source code.

Copyright (c) 2026 廷廷小教室、廷廷的家（Tim945）
