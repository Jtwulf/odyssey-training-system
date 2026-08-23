# Odyssey Training System

Odyssey Running の **毎週火曜 Quality Session を設計・運用するための知識ベース**です。

このリポジトリに、毎月の実際のトレーニングメニューを保存するわけではありません。
ここで管理するのは、**「なぜその練習を行うのか」「どう設計・判断するのか」**という、今後も繰り返し使うルールと根拠です。

> **GitHub = WHY / HOW**  
> **Google Sheets = WHAT / WHEN**  
> **Strava = 参加者への告知**

---

## このリポジトリの役割

Odyssey の火曜練習を考えるときには、単に「今月は 400m × 10」のようにメニューを並べるだけではなく、次のような判断が必要です。

- 次のレースや時期に対して、何を鍛えるべきか
- Threshold、VO2max系、Speed、Hill などをどう使い分けるか
- 走力差のある参加者に、どう同じ目的の刺激を与えるか
- 距離ベースと時間ベースのどちらを使うか
- レストをどの程度にするか
- 暑さ、会場、60分という制約をどう考慮するか
- Google Sheets の PLAN にどう表現するか

このリポジトリは、こうした判断を **科学的エビデンス → Odyssey向けの判断ルール → 実際のPLAN** へつなぐためにあります。

```text
Scientific Evidence
        ↓
Odyssey Coaching Logic
        ↓
Workout / PLAN operating rules
        ↓
Google Sheets PLAN
        ↓
Strava announcement
```

---

## どこに何があるか

ファイル名は参照しやすいよう英語のままですが、役割は以下の4つに分かれています。

```text
README.md
│
└── knowledge/
    ├── evidence.md              # ① 科学的根拠を探すための入口
    ├── coaching-system.md       # ② 根拠をOdysseyの練習設計へ変換するルール
    ├── plan-operations.md       # ③ Google Sheets PLANの作成・運用ルール
    │
    └── evidence/                # ④ テーマ別の詳細な科学的根拠
        ├── methods.md
        ├── references.md
        ├── intensity-domains.md
        ├── training-distribution-periodization.md
        ├── threshold-aerobic-power.md
        ├── interval-programming-recovery.md
        ├── speed-economy-hills-warmup.md
        ├── race-demands.md
        ├── durability-marathon.md
        └── taper-environment.md
```

### ① `knowledge/evidence.md` — まずここを見る

**科学的エビデンスの目次・案内役**です。

すべての論文情報を読むためのファイルではなく、今回考えているWorkoutやレースに対して、`knowledge/evidence/` のどのファイルを読めばよいかを判断するために使います。

例:

- 1 km向けの練習を考える → intensity / aerobic power / interval / speed / race demands
- Marathon向けの練習を考える → periodization / threshold / durability / race demands
- Hillや短いSpeedを考える → speed / hills / interval programming

---

### ② `knowledge/coaching-system.md` — Odysseyとしてどう判断するか

**科学的な知見を、Odyssey Running の火曜練習へ変換するための中心ルール**です。

研究で分かっていることと、Odyssey固有の判断を混同しないよう、主に次の3種類を区別しています。

- **Evidence-based** — 研究による直接的な裏付けがあるもの
- **Inference** — 研究をOdysseyの条件へ合理的に応用したもの
- **Coaching judgment** — 会場・人数・60分枠などを踏まえた運用上の判断

実際のWorkoutを設計するときは、このファイルが **「Odysseyではどうするか」** の基準になります。

---

### ③ `knowledge/plan-operations.md` — PLANをどう作るか

**Google Sheets の `PLAN` をどう書き、どう維持するかの運用ルール**です。

例えば以下を管理します。

- 時間ベース / 距離ベースをどう選ぶか
- `Main Workout` / `Workout Details` / `Training Effect` の書き方
- Group A / B / C の扱い
- Recovery の記載方法
- 既に告知したWorkoutをどう扱うか
- PLANを更新した後に何を確認するか
- 今後も使うルール変更をどこへ保存するか

つまり、`coaching-system.md` が **練習設計の判断ルール**、`plan-operations.md` が **その判断をPLANへ落とし込むルール**です。

---

### ④ `knowledge/evidence/` — 科学的根拠の詳細

ここには、テーマごとの詳細なエビデンスを保存しています。

| File | 日本語でいうと | 主な内容 |
|---|---|---|
| `methods.md` | エビデンスの評価方法 | Evidence strength、OdysseyへのDirectness、Claimの書式 |
| `references.md` | 参考文献台帳 | 検証済み論文・Source ID |
| `intensity-domains.md` | 運動強度の考え方 | Moderate / Heavy / Severe、LT / VT / CS / MAV など |
| `training-distribution-periodization.md` | トレーニング配分と期分け | TID、Progression、Specificity |
| `threshold-aerobic-power.md` | Threshold・有酸素パワー | Tempo、Cruise Interval、VO2系Interval |
| `interval-programming-recovery.md` | IntervalとRecoveryの組み方 | Rep時間・距離、総量、Rest、Mixed abilityへの対応 |
| `speed-economy-hills-warmup.md` | Speed・Economy・Hill | Sprint、Running Economy、Hill、Warm-up |
| `race-demands.md` | レース別要求 | 1 km、3–5 km、10 km、Half、Marathon |
| `durability-marathon.md` | MarathonとDurability | 長時間走行での能力低下、Marathonとの関係 |
| `taper-environment.md` | Taperと環境 | レース前調整、暑熱、環境による負荷調整 |

これらは「この論文ではこうだった」という論文要約集ではなく、**Odysseyの判断に使えるClaim単位の知識ベース**として整理されています。

通常の月次PLAN作成で、毎回すべてを読む必要はありません。`knowledge/evidence.md` を入口に、必要なテーマだけ参照します。

---

## 実際に月間PLANを作るときの流れ

基本的には次の順番で使います。

```text
1. 次のレース / milestone を確認
        ↓
2. knowledge/evidence.md で必要なEvidenceを特定
        ↓
3. 必要な knowledge/evidence/*.md だけ確認
        ↓
4. coaching-system.md に従ってOdyssey向けWorkoutへ変換
        ↓
5. plan-operations.md に従ってGoogle Sheets PLANへ記載
        ↓
6. PLANを再確認
        ↓
7. 確定した内容をStrava等で参加者へ告知
```

重要なのは、**GitHubの内容をそのまま参加者へ見せることではなく、GitHubを判断の裏側として使うこと**です。

---

## GitHub / Google Sheets / Strava の分担

| 場所 | 役割 | 保存するもの |
|---|---|---|
| **GitHub** | WHY / HOW | 科学的根拠、Coaching Logic、今後も使う運用ルール |
| **Google Sheets `PLAN`** | WHAT / WHEN | 実際の日付、会場、Workout、Group別設定、Training Effect |
| **Strava** | Announcement | 参加者向けに確定した練習内容 |

**月間Workout PlanそのものはGitHubへコピーしません。**
Google Sheets とGitHubで同じPLANを二重管理すると、どちらが最新か分からなくなるためです。

また、今後も適用したいルール変更や修正は、チャット履歴やAIの記憶だけに残さず、対応するGitHubファイルへ保存します。

---

## このシステムが扱う範囲

### 扱うもの

- 毎週火曜 20:00–21:00 の Quality Session / Point Workout
- 通常5–10名程度の、走力差があるグループ
- 主に Yoyogi Park / Meiji Jingu Gaien での実施
- 月単位のWorkout設計
- レースやmilestoneを意識したProgression
- Evidenceに基づくWorkout設計
- Google Sheets `PLAN` の運用

### 扱わないもの

- 各参加者の週間走行距離の管理
- 睡眠、疲労、故障などの継続モニタリング
- 個人別の週間トレーニングプラン
- 全参加者のStrava / Intervals.icuデータ管理
- 月間PLANのGitHubへの保存
- Draft / Review / Approved などの複雑なworkflow管理

Odyssey Training System は、**火曜の1セッションを高品質に設計すること**に責任範囲を限定します。
