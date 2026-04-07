# Claude 利用開始手順

**作成日:** 2026年4月7日
**対象:** AIタスクフォース メンバー
**所要時間:** 約30〜45分（インストール含む）

---

## 利用開始フロー（全体像）

```
STEP 0: 利用規則の通読（必須）
   ↓
STEP 1: Claude Team シートの有効化確認
   ↓
STEP 2: claude.ai にログイン & User Preferences 設定
   ↓
STEP 3: 3つのProjectへのアクセス確認
   ↓
STEP 4: 各種ツールのインストール
   ↓
STEP 5: 動作確認
```

---

## STEP 0: 利用規則の通読【必須・最優先】

利用開始前に必ず以下を通読する。

- 📕 **LTS-ST_AI_TF_利用規則_禁止事項・注意事項_v1.0**
- 📘 **LTS-ST_AI_TF_利用環境設計仕様書_v1.3**
- 📄 **本ディレクトリの「Claude利用開始_認識事項まとめ.md」**

特に以下を理解してから利用を開始すること:
- 入力禁止情報（顧客情報・財務・人事・認証情報等）
- ハルシネーションのリスクと対処
- 各ツールのリリース段階（Beta / Experimental / Research Preview）

---

## STEP 1: Claude Team シートの有効化確認

1. 招待メール（Anthropic から届く）を開く
2. リンクから **claude.ai** にアクセス
3. LTS-ST のメールアドレス（**@softec-ic.co.jp**）でサインアップ
4. ワークスペース「**LTS-ST AI Task Force**」が表示されることを確認

> **トラブル時:** シートが有効化されていない場合は TF責任者に連絡

---

## STEP 2: User Preferences の設定【必須】

社長メールにある必須設定。**最初のセッション前に必ず実施**。

### 手順

1. claude.ai にログイン
2. 右下プロフィールアイコン → **Settings** をクリック
3. **Profile** タブを選択
4. **User Preferences** 欄に以下3点を記入

### 記入内容

| 項目 | 記入例 |
|---|---|
| **担当業務・役職** | Java エンジニア / PMO / IT コンサルタント など |
| **よく扱うドメイン** | 金融系システム / 製造業 DX など |
| **好みの回答スタイル** | 技術的詳細を重視 / 要点のみ簡潔に など |

5. **Save** をクリック

> **ポイント:** ここで設定した内容は全Project共通で適用され、Claudeの回答がパーソナライズされる。

---

## STEP 3: 3つのProjectへのアクセス確認【必須】

左サイドバーの **Projects** から以下3つにアクセスできることを確認する。

| Project | 役割 | 使うタイミング |
|---|---|---|
| **TF_Base** | 全会話の前提・日常業務支援 | 普段の業務支援はここから |
| **TF_Prompt_Library** | プロンプト資産の管理 | プロンプトを作る・改善する |
| **TF_Research** | 調査・分析・ナレッジ蓄積 | 調査・社内ナレッジ参照 |

> **トラブル時:** Project が表示されない場合は TF責任者に連絡

### 最初の試行

TF_Base を開いて、軽い業務質問（例: 「営業日報のフォーマットを提案して」）を入力し、System Prompt が適用された回答が返ることを確認する。

---

## STEP 4: ツールのインストール

### 4.1 Claude Desktop【必須・最優先】

- **入手先:** https://claude.ai/download
- **対象:** Windows / macOS
- **手順:** ダウンロード → インストーラ実行 → claude.ai と同じアカウントでログイン

### 4.2 モバイルアプリ【必須】

| OS | ストア |
|---|---|
| iOS | App Store で「Claude」検索 |
| Android | Google Play で「Claude」検索 |

> **メリット:** 外出先で音声入力により Project へ調査依頼を送れる

### 4.3 Claude for Excel【必須・Beta】

1. Excel を起動
2. **挿入** → **アドインの取得** → Microsoft Marketplace
3. 「**Claude for Excel**」を検索 → 追加
4. リボンに表示された Claude アイコンからログイン

### 4.4 Claude for PowerPoint【必須・Beta】

1. PowerPoint を起動
2. **挿入** → **アドインの取得** → Microsoft Marketplace
3. 「**Claude for PowerPoint**」を検索 → 追加
4. リボンに表示された Claude アイコンからログイン

### 4.5 Claude in Chrome【必須・Experimental】

1. Chrome ウェブストアで「**Claude**」拡張を検索
2. **Chrome に追加**
3. 拡張アイコンからログイン

> **注意:** 機密システム（社内管理・人事・財務）では使用禁止

### 4.6 音声入力の設定（推奨）

#### macOS の場合
1. **システム設定** → **キーボード** → **音声入力** をオン
2. Claude の入力欄をクリック
3. **Fnキー2回押し**（デフォルト）で音声入力開始

#### Windows の場合
1. **設定** → **時刻と言語** → **音声認識** をオン
2. Claude の入力欄をクリック
3. **Win + H** キーで音声入力開始

> **注意:** Voice Mode は英語のみ対応。日本語はディクテーションを使用

---

## STEP 5: 動作確認

以下の簡単なタスクで一通り動くか確認する。

| # | 確認項目 | 期待される動作 |
|---|---|---|
| 1 | claude.ai で TF_Base に質問 | User Preferences が反映された回答 |
| 2 | Claude Desktop で同じ質問 | 同じワークスペース・Projectが利用可能 |
| 3 | モバイルアプリで TF_Research を開く | Project が同期されている |
| 4 | Claude for Excel で簡単な数式生成 | リボンから呼び出し可能 |
| 5 | Claude for PowerPoint でスライド生成 | リボンから呼び出し可能 |
| 6 | MS365 Connector 経由で社内文書参照 | SharePoint/Teams の情報が引用される |

---

## 困ったときは

| 状況 | 対応 |
|---|---|
| Claude Team シートが有効化されていない | TF責任者に連絡 |
| Project にアクセスできない | TF責任者に連絡 |
| MS365 Connector が接続できない | IT管理者にテナント確認を依頼 |
| 入力してよい情報か判断に迷う | **入力しない**。匿名化して質問するか TF責任者に確認 |
| 禁止事項に違反した可能性 | **直ちに TF責任者に報告**（証跡保存・使用一時停止） |

---

## 利用開始 チェックリスト

- [ ] 利用規則 v1.0 を通読した
- [ ] 設計仕様書 v1.3 を通読した
- [ ] 認識事項まとめを読んだ
- [ ] claude.ai にログインできた
- [ ] User Preferences を設定した（役職・ドメイン・回答スタイル）
- [ ] TF_Base にアクセスできた
- [ ] TF_Prompt_Library にアクセスできた
- [ ] TF_Research にアクセスできた
- [ ] Claude Desktop をインストールした
- [ ] モバイルアプリをインストールした
- [ ] Claude for Excel をインストールした
- [ ] Claude for PowerPoint をインストールした
- [ ] Claude in Chrome をインストールした
- [ ] 音声入力をセットアップした（任意）
- [ ] 入力禁止情報（6カテゴリ）を理解した
- [ ] 生成物の品質確認チェックリストを把握した
