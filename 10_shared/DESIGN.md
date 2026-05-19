# Design System — きょうすけブランド

最終更新：2026-05-18  
ベースカラー出典：[BRAND.md](BRAND.md)

---

## 1. Visual Theme & Atmosphere

このデザインシステムは **シンプル・ビジネスライク・清潔感** を体現する。  
キャンバスは白（`#FFFFFF`）を軸とし、ブランドカラーのターコイズグリーン（`#20B2AA`）が見出し・CTA・アクセント帯に登場することで、誠実さと信頼感を表現する。

ターコイズは4段階に調整して使い分ける（Brand / Accent / Deep / Mid）。装飾は最小限にとどめ、グラデーションは使わない。余白を大きく取り「呼吸するレイアウト」を保つ。

**主な特徴：**
- 4層ターコイズシステム（Brand / Accent / Deep / Mid）―それぞれ役割が固定
- 白キャンバスに清潔感のある構造：白 → ターコイズ帯 → 白 → Deep Turquoise帯（フッター）
- フォント：**Noto Sans JP**（太め・読みやすい）を基本書体として使用
- ボタンはすべて `50px` フルピル（角丸）
- アクティブ状態は `scale(0.95)` のプレスフィードバック
- カード角丸 `12px`、シャドウは2〜3層の低アルファ値を重ねる「囁くような立体感」

**色面構成のリズム：**  
白ヒーロー → 白コンテンツ → ターコイズ帯（Deep Turquoise `#0D6963`）→ 白ユーティリティ → Deep Turquoiseフッター

---

## 2. Color Palette & Roles

### Primary（ブランドカラー展開）

| 名前 | カラーコード | 役割 |
|------|------------|------|
| **Brand Turquoise** | `#20B2AA` | メイン見出し、ブランドの主役色 |
| **Accent Turquoise** | `#1AA39B` | CTAボタン塗り、フローティングボタン |
| **Deep Turquoise** | `#0D6963` | フッター、フィーチャー帯の背景 |
| **Mid Turquoise** | `#13807A` | 装飾アクセント、セカンダリーダーク要素 |
| **Light Turquoise** | `#B8E5E3` | フォーム有効状態のティント |

### Secondary & Accent

| 名前 | カラーコード | 役割 |
|------|------------|------|
| **Premium Gold** | `#C9A028` | プレミアム強調（特別な達成・実績表示のみ） |
| **Gold Light** | `#DFC49D` | プレミアム帯の背景ウォッシュ |
| **Gold Lightest** | `#F5F0E8` | プレミアムセクションのキャンバス |

> Gold はプレミアム・実績表示の場面のみ使用する。汎用アクセントとして使わない。

### Surface & Background

| 名前 | カラーコード | 役割 |
|------|------------|------|
| **White** | `#FFFFFF` | メインページキャンバス、カード背景 |
| **Off White** | `#FAFAFA` | ドロップダウン、フォームカード、ユーティリティ |
| **Turquoise Mist** | `#F0FAFA` | セクション区切り、薄いターコイズウォッシュ |

### Text

| 名前 | カラーコード | 役割 |
|------|------------|------|
| **Text Dark** | `rgba(33, 33, 33, 0.87)` | 明るい背景上のメイン本文・見出し |
| **Text Dark Soft** | `rgba(33, 33, 33, 0.58)` | サブテキスト・メタ情報 |
| **Text White** | `rgba(255, 255, 255, 1.0)` | ダーク帯上のメイン文字 |
| **Text White Soft** | `rgba(255, 255, 255, 0.70)` | ダーク帯上のサブテキスト・キャプション |

> 本文テキストには純黒を使わない。`rgba(33,33,33,0.87)` でキャンバス温度に馴染ませる。

### Semantic

| 名前 | カラーコード | 役割 |
|------|------------|------|
| **Error Red** | `#C82014` | エラー・破壊的操作 |
| **Warning Yellow** | `#FBBC05` | 警告 |
| **Valid Tint** | `rgba(184, 229, 227, 0.33)` | フォーム有効フィールド背景 |
| **Invalid Tint** | `rgba(200, 32, 20, 0.05)` | フォーム無効フィールド背景 |

### Black / White Alpha Ladders（オーバーレイ用）

- Dark overlay: `rgba(0,0,0,0.06)` 〜 `rgba(0,0,0,0.90)` （10%刻み）
- Light overlay: `rgba(255,255,255,0.10)` 〜 `rgba(255,255,255,0.90)` （10%刻み）

### グラデーションシステム

グラデーションは使用しない。すべてソリッドカラーブロックで構成する。

---

## 3. Typography Rules

### Font Family

| 役割 | フォント |
|------|---------|
| **Primary** | `"Noto Sans JP", "Hiragino Kaku Gothic ProN", "Meiryo", sans-serif` |
| **フォールバック** | `"Hiragino Kaku Gothic ProN", "Meiryo", sans-serif` |
| **英語見出し（必要な場合）** | `"Inter", "Helvetica Neue", Arial, sans-serif` |

### Type Hierarchy

| 役割 | サイズ | ウェイト | 行高 | 字間 | 用途 |
|------|------|---------|------|------|------|
| Display | 5.0rem / 80px | 700 | 1.2 | -0.03em | 最大ヒーロー見出し |
| H1 | 3.2rem / 32px | 700 | 1.3 | -0.02em | ページ主見出し（Brand Turquoise） |
| H2 | 2.4rem / 24px | 400 | 1.4 | -0.02em | セクション見出し（Text Dark） |
| H3 | 2.0rem / 20px | 700 | 1.4 | -0.01em | カード見出し |
| Body Large | 1.9rem / 19px | 400–700 | 1.75 | -0.01em | ヒーロー本文 |
| Body | 1.6rem / 16px | 400 | 1.6 | -0.01em | 標準本文 |
| Small | 1.4rem / 14px | 400–700 | 1.5 | -0.01em | ボタンラベル、メタ情報 |
| Micro | 1.3rem / 13px | 400 | 1.5 | -0.01em | キャプション、注記 |

**Letter-spacing tokens:**
- `--ls-default`: `-0.01em`（標準。全面適用）
- `--ls-loose`: `0.1em`（キャップス強調）

**Line-height tokens:**
- `--lh-normal`: `1.6`（本文）
- `--lh-compact`: `1.2`（見出し・ボタン）

### Principles

- **H1 と H2 はサイズではなくウェイト＋色で区別する。** H1は700 + Brand Turquoise、H2は400 + Text Dark。
- **字間を -0.01em にすることで、Noto Sans JPが引き締まった信頼感のある印象になる。**
- **本文は純黒ではなく `rgba(33,33,33,0.87)` を使い、白キャンバスと馴染ませる。**
- `1rem = 10px` を前提としたremスケール（`font-size: 62.5%` ルートトリック）。

---

## 4. Component Stylings

### Buttons

**1. Primary Filled（メインCTA）**
- Background: `#1AA39B`（Accent Turquoise）
- Text: `#FFFFFF`
- Border: `1px solid #1AA39B`
- Radius: `50px`（フルピル）
- Padding: `10px 24px`
- Font: Noto Sans JP, 16px, weight 700, letter-spacing `-0.01em`
- Active: `transform: scale(0.95)` / Transition: `all 0.2s ease`

**2. Primary Outlined（セカンダリーCTA）**
- Background: transparent
- Text: `#1AA39B`
- Border: `1px solid #1AA39B`
- 以下同上（radius / padding / active / transition）

**3. Dark Filled（強調アクション）**
- Background: `#212121`
- Text: `#FFFFFF`
- Border: `1px solid #212121`
- Radius: `50px`, Padding: `10px 24px`
- Font: 14px, weight 700

**4. Dark Outlined（サインイン等）**
- Background: transparent
- Text: `rgba(33, 33, 33, 0.87)`
- Border: `1px solid rgba(33, 33, 33, 0.87)`
- Radius: `50px`, Padding: `10px 24px`, Font: 14px, weight 700

**5. White-on-Dark Filled（ダーク帯上のプライマリ）**
- Background: `#FFFFFF`
- Text: `#1AA39B`
- Border: `1px solid #FFFFFF`
- ダーク帯（Deep Turquoise）上で使用する白ボタン

**6. Outlined on Dark（ダーク帯上のセカンダリ）**
- Background: transparent
- Text: `#FFFFFF`
- Border: `1px solid #FFFFFF`
- ダーク帯上でWhite-on-Darkと組み合わせるセカンダリ

**7. Floating Action Button（フローティングCTA）**
- Background: `#1AA39B`（Accent Turquoise）
- Icon: `#FFFFFF`
- Size: `56px`（直径）
- Radius: `50%`
- Fixed bottom-right, `-0.8rem` タッチオフセット
- Shadow: `0 0 6px rgba(0,0,0,0.24)` + `0 8px 12px rgba(0,0,0,0.14)`
- Active: ambient shadowをゼロに + `scale(0.95)`

### Cards & Containers

**Content Card（デフォルト）**
- Background: `#FFFFFF`
- Radius: `12px`
- Shadow: `0px 0px 0.5px 0px rgba(0,0,0,0.14), 0px 1px 1px 0px rgba(0,0,0,0.24)`

**Section Band（ターコイズフィーチャー帯）**
- Background: `#0D6963`（Deep Turquoise）
- Full-width
- Text: `#FFFFFF` / サブテキスト: `rgba(255,255,255,0.70)`
- CTAはWhite-on-Dark FilledとOutlined on Darkのペア

**Modal**
- Padding: `2.4rem`
- Top Padding: `8.8rem`
- Radius: `12px`

### Inputs & Forms

**フローティングラベル入力**
- Label デフォルト: `1.6rem`（アクティブ時 `1.3rem`）
- Field padding: `12px`
- Focus border: Accent Turquoise `#1AA39B`
- Valid tint: `rgba(184, 229, 227, 0.33)`
- Invalid tint: `rgba(200, 32, 20, 0.05)`
- アニメーション: `0.3s cubic-bezier(0.32, 2.32, 0.61, 0.27)`

### Navigation

**グローバルナビ**
- Fixed, progressive height: `64px` xs → `72px` md → `83px` tablet → `99px` desktop
- Shadow: `0 1px 3px rgba(0,0,0,0.1), 0 2px 2px rgba(0,0,0,0.06), 0 0 2px rgba(0,0,0,0.07)`
- 左: ロゴ
- 右: Sign in（outlined）+ 主CTA（dark filled）

---

## 5. Layout Principles

### Spacing Scale（`1rem = 10px` 前提）

| Token | Rem | px | 用途 |
|-------|-----|----|------|
| `--space-1` | 0.4rem | 4px | 最小インラインパディング |
| `--space-2` | 0.8rem | 8px | 小さいギャップ |
| `--space-3` | 1.6rem | 16px | デフォルト — カードパディング、外ガター(xs) |
| `--space-4` | 2.4rem | 24px | セクション内スペース |
| `--space-5` | 3.2rem | 32px | セクション間の主要スペース |
| `--space-6` | 4.0rem | 40px | 大きなギャップ、外ガター(lg) |
| `--space-7` | 4.8rem | 48px | セクション間 |
| `--space-8` | 5.6rem | 56px | 広い余白 |
| `--space-9` | 6.4rem | 64px | 最大セクションパディング |

**Gutter tokens:**
- `--outerGutter: 1.6rem`（16px、モバイル）
- `--outerGutterMedium: 2.4rem`（24px、タブレット）
- `--outerGutterLarge: 4.0rem`（40px、デスクトップ）

### Border Radius Scale

| 値 | 用途 |
|----|------|
| `12px` | カード・モーダル・タイル |
| `50px` | すべてのボタン（フルピル） |
| `50%` | 円形アイコン・フローティングボタン |
| `4px` | 入力フィールド・小さなUI要素 |

### Whitespace Philosophy

余白は「余裕と信頼感」を表す。セクションパディングは40〜64px。コンテンツブロックの区切りは罫線より余白で表現する。

---

## 6. Depth & Elevation

| レベル | シャドウ | 用途 |
|--------|---------|------|
| Card | `0 0 0.5px rgba(0,0,0,0.14), 0 1px 1px rgba(0,0,0,0.24)` | デフォルトカード |
| Nav | `0 1px 3px rgba(0,0,0,0.1), 0 2px 2px rgba(0,0,0,0.06), 0 0 2px rgba(0,0,0,0.07)` | 固定ナビ |
| FAB Base | `0 0 6px rgba(0,0,0,0.24)` | フローティングボタン ベースハロー |
| FAB Ambient | `0 8px 12px rgba(0,0,0,0.14)` | フローティングボタン 環境光 |

**シャドウ原則：** 単一の重いドロップシャドウは使わない。2〜3層の低アルファを重ねてリアルな奥行きを表現する。

---

## 7. Do's and Don'ts

### Do
- ページキャンバスは `#FFFFFF`（ブランド背景色）を基本とする
- ターコイズの4層を役割通りに使い分ける（Brand=見出し、Accent=CTA、Deep=帯/フッター）
- ボタンはすべて `50px` フルピル
- `transform: scale(0.95)` をすべてのボタンのアクティブ状態に適用する
- Premium Gold は実績・特別表示の場面のみ使用する
- シャドウは2〜3層の低アルファを重ねる
- 字間は `-0.01em` を全体に適用する

### Don't
- グラデーションを使わない（全面ソリッドカラーブロック）
- ボタンの角を四角にしない（50pxピルは例外なく適用）
- 本文に純黒を使わない（`rgba(33,33,33,0.87)` を使う）
- H1とH2をサイズで区別しない（ウェイト＋色で区別する）
- Premium Goldを汎用アクセントとして使わない
- `scale(0.95)` のアクティブフィードバックを省略しない
- 重い単一ドロップシャドウを使わない

---

## 8. Responsive Behavior

### Breakpoints

| 名前 | Width | 主な変化 |
|------|-------|---------|
| xs | < 480px | ナビ64px、ハンバーガーメニュー、1カラム |
| Mobile | 480–767px | ナビ72px、2カラムグリッド |
| Tablet | 768–1023px | ナビ83px、ヒーロー分割開始 |
| Desktop | 1024–1439px | ナビ99px、フル非対称ヒーロー |
| XLarge | 1440px+ | コンテンツ幅キャップ、余白最大 |

### Collapsing Strategy

- ヒーロー 40/60分割 → モバイルでは縦積み（画像上・テキスト下）
- フィーチャー帯 → フルワイドのまま、テキスト＋画像が縦積みに
- 外ガター: 16px → 24px → 40px
- フローティングボタン: すべてのスクロール面で右下に固定表示を維持

---

## 9. CSS Variables 早見表

```css
:root {
  /* === Brand Colors === */
  --color-brand:       #20B2AA;  /* Brand Turquoise — 見出し */
  --color-accent:      #1AA39B;  /* Accent Turquoise — CTA */
  --color-deep:        #0D6963;  /* Deep Turquoise — 帯/フッター */
  --color-mid:         #13807A;  /* Mid Turquoise — 装飾 */
  --color-light:       #B8E5E3;  /* Light Turquoise — フォーム有効 */

  /* === Premium Accent === */
  --color-gold:        #C9A028;
  --color-gold-light:  #DFC49D;
  --color-gold-faint:  #F5F0E8;

  /* === Surface === */
  --color-white:       #FFFFFF;
  --color-off-white:   #FAFAFA;
  --color-mist:        #F0FAFA;

  /* === Text === */
  --color-text:        rgba(33, 33, 33, 0.87);
  --color-text-soft:   rgba(33, 33, 33, 0.58);
  --color-text-on-dark:      rgba(255, 255, 255, 1.0);
  --color-text-on-dark-soft: rgba(255, 255, 255, 0.70);

  /* === Semantic === */
  --color-error:       #C82014;
  --color-warning:     #FBBC05;

  /* === Typography === */
  --font-primary: "Noto Sans JP", "Hiragino Kaku Gothic ProN", "Meiryo", sans-serif;
  --ls-default:   -0.01em;
  --ls-loose:      0.10em;
  --lh-normal:     1.6;
  --lh-compact:    1.2;

  /* === Spacing === */
  --space-1: 0.4rem;   /* 4px */
  --space-2: 0.8rem;   /* 8px */
  --space-3: 1.6rem;   /* 16px */
  --space-4: 2.4rem;   /* 24px */
  --space-5: 3.2rem;   /* 32px */
  --space-6: 4.0rem;   /* 40px */
  --space-7: 4.8rem;   /* 48px */
  --space-8: 5.6rem;   /* 56px */
  --space-9: 6.4rem;   /* 64px */

  --outerGutter:       1.6rem;
  --outerGutterMedium: 2.4rem;
  --outerGutterLarge:  4.0rem;

  /* === Components === */
  --cardBorderRadius:  12px;
  --cardBoxShadow:     0px 0px 0.5px 0px rgba(0,0,0,0.14), 0px 1px 1px 0px rgba(0,0,0,0.24);
  --buttonBorderRadius: 50px;
  --buttonActiveScale: scale(0.95);
  --buttonTransition:  all 0.2s ease;

  --expanderDuration:  300ms;
  --expanderEasing:    cubic-bezier(0.25, 0.46, 0.45, 0.94);
}
```

---

## 10. Agent Prompt Guide

### Quick Color Reference

| 役割 | カラー |
|------|-------|
| Primary CTA fill | Accent Turquoise `#1AA39B` |
| Primary CTA text | White `#FFFFFF` |
| Brand heading | Brand Turquoise `#20B2AA` |
| Feature band / Footer | Deep Turquoise `#0D6963` |
| Page canvas | White `#FFFFFF` |
| Card canvas | White `#FFFFFF` |
| Heading text on light | Text Dark `rgba(33,33,33,0.87)` |
| Body text on light | Text Dark Soft `rgba(33,33,33,0.58)` |
| Body text on dark | Text White Soft `rgba(255,255,255,0.70)` |
| Premium accent | Gold `#C9A028` |
| Error | Red `#C82014` |

### Example Component Prompts

1. **Primary CTA ボタン：**  
「Accent Turquoise（`#1AA39B`）背景、白テキスト、Noto Sans JP 16px weight700、`-0.01em` letter-spacing、`50px` border-radius、`10px 24px` padding。アクティブ状態は `scale(0.95)`、`0.2s ease` トランジション。」

2. **コンテンツカード：**  
「White（`#FFFFFF`）背景、`12px` border-radius、シャドウ `0 0 0.5px rgba(0,0,0,0.14), 0 1px 1px rgba(0,0,0,0.24)`。パディング `16〜24px`。White ページキャンバス上に配置。」

3. **フィーチャー帯：**  
「Deep Turquoise（`#0D6963`）背景の全幅セクション。左カラム：白 Noto Sans JP H2 24px weight700、続いて Text White Soft（`rgba(255,255,255,0.70)`）の本文、CTAはWhite-on-Dark FilledとOutlined on Darkのペア。右カラム：プロダクト画像。比率40/60、768px以下で縦積み。」

4. **フォーム入力（フローティングラベル）：**  
「フォーカス時にラベルが枠の上に浮き上がる。フォーカス border color: Accent Turquoise `#1AA39B`。有効フィールド背景 `rgba(184,229,227,0.33)` tint。無効フィールド背景 `rgba(200,32,20,0.05)` tint。アニメーション `0.3s cubic-bezier(0.32, 2.32, 0.61, 0.27)`。」