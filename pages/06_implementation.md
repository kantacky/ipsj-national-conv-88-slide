---
layout: content
transition: none
title: 提案手法
subtitle: 実装
---

- Python と Google GenAI SDK を使用（並行処理で大量生成）
- モデル選定：**フォトウォークデータの制約を遵守できるか**で比較

<div class="text-sm my-2">

| モデル | 周回性 | 地理的整合性 | 結果 |
|---|:---:|:---:|:---:|
| Gemini 2.5 Flash Lite | ❌ | ❌ | 不採用 |
| Gemini 2.5 Flash | ✅ | ❌ | 不採用 |
| **Gemini 3 Flash Preview** | **✅** | **✅** | **採用** |

</div>

<!--
次に実装について説明します。

Python と Google GenAI SDK を使用し、並行処理で大量のセッションを効率的に生成しました。

モデルの選定では、先ほど説明したフォトウォークデータ固有の制約、つまり周回性と地理的整合性を遵守できるかを基準に比較しました。
Gemini 2.5 Flash Lite は周回性を、Gemini 2.5 Flash は地理的整合性を遵守できなかったため、
両方の制約を最もよく遵守できた Gemini 3 Flash Preview を採用しました。
-->
