# cp-time-expiry-core

Insert-only cron-based expiration core.  
（Insert-only型・cron駆動の失効コア）

This repository contains the minimal core logic for time-based expiration  
in the Contribution Protocol (CP).

本リポジトリは、Contribution Protocol（CP）における  
時間主権による失効の最小コアロジックを実装したものです。

---

## Concept / 概念

- No UPDATE（更新しない）
- No DELETE（削除しない）
- Insert-only state transition logging  
  （状態遷移は追加記録のみ）
- Time sovereignty  
  （失効は人の判断ではなく、DB時刻によって自動確定）

Expiration is not a mutation of state,  
but an append-only record of a state transition event.

失効とは状態の書き換えではなく、  
状態遷移イベントの追記記録である。

---

## What this is / これは何か

This is not the full accounting system.  
This is not the reserve logic.  
This is not the governance layer.

これは会計システム全体ではない。  
これは引当ロジックではない。  
これはガバナンス層でもない。

This is the minimal structural core  
that proves time-based irreversible expiration.

これは「時間による不可逆失効」を証明する  
最小構造カーネルである。

---

## Status / 状態

Experimental minimal kernel.  
（実験的ミニマルカーネル）

