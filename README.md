# Odyssey Training System

Odyssey Running の毎週火曜 Quality Session を、科学的エビデンス、参加者の走力差、会場制約、レースマイルストーンを踏まえて月単位で設計するための Knowledge Base です。

## Scope

- 毎週火曜 20:00–21:00 の Quality Session / Point Workout
- 通常 5–10 名程度の幅広い走力の参加者
- 主会場: Yoyogi Park / Meiji Jingu Gaien
- カレンダー月単位でのセッション設計
- Evidence と Coaching Logic の明文化
- Google Sheets PLAN の安定した運用・表示ルール

## Non-scope

- 個人の週間走行距離・疲労・故障・睡眠の継続管理
- 個人コーチングや週間トレーニングプラン
- 全参加者の Strava / Intervals.icu 同期
- 月間 Workout Plan の GitHub 保存
- Draft / Review / Approved / Locked 等の workflow 管理

## Source of Truth

- **GitHub = WHY / HOW** — Evidence + Coaching Logic + persistent PLAN operating rules
- **Google Sheets = WHAT / WHEN** — 実際の月間 Workout Plan
- **Strava = Announcement** — 一般参加者への最終告知

GitHub は Knowledge Base のみを保持し、月間PLANを Google Sheets と二重管理しません。

継続的に適用すべきルールやユーザーからの修正は、チャット履歴やアシスタントの記憶だけに依存せず、GitHub の該当ルールファイルへ永続化します。Google Sheets `SYSTEM` は運用上のクイックリファレンスとして使えますが、永続ルールの正本は GitHub です。

## Repository structure

```text
README.md
knowledge/
  evidence.md
  coaching-system.md
  plan-operations.md
```

- `evidence.md` — 研究エビデンス
- `coaching-system.md` — Odysseyへのコーチング上の翻訳
- `plan-operations.md` — PLANの書き方・時間/距離選択・表示・変更・ルール永続化

必要性が明確になるまで、plans / state / reviews / automation 等は追加しません。
