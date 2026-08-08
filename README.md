# HITA 使用统计（公开聚合）

> 数据由 hita-api 每日自动生成并推送；本仓库只包含**聚合计数**。

## 隐私声明

- 不含学号、姓名、installation_id 等任何个人明细；
- 原始事件数据（JSONL）永不进入本仓库，仅存于私有服务器。

## 更新频率

- 每天约 UTC 00:10 生成当日聚合（daily）与本周累计（weekly）。

## 格式

- daily/YYYY/MM/YYYY-MM-DD.json：当日 DAU（按 app）与事件计数（含版本/工具维度），附平台/版本/错误/来源分布
- weekly/YYYY-Www.json：ISO 周累计
- 字段示例：{ "date": "2026-08-08", "dau": { "hita-android": 12 }, "events": { "app_foreground": { "count": 34, "by_version": { "2.5.5": 30 } } }, "platforms": { "android": 12 } }

_last updated: 2026-08-08T18:30:49Z UTC_
