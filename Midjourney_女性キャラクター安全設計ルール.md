# Midjourney女性キャラクター生成・安全設計ルール

## 目的

ファンタジー世界の女性キャラクターを、モデルやファッションイラストのように美しく表現する。

衣装によって肩・腕・脚などが見える場合でも、性的・挑発的・フェティッシュな表現にはせず、ファッション、物語上の役割、文化的背景、活動性を中心に描写する。

本ルールはMidjourneyのモデレーション回避を目的とするものではなく、安全で非性的なキャラクターデザインを一貫して作るためのものである。

## 1. 年齢表現

- 肌の露出を含む女性キャラクターは、必ず明確な成人として設定する。
- `girl`、`teenage girl`、`young girl`など、未成年と解釈され得る表現を使用しない。
- `princess`だけでは年齢が不明なため、必要に応じて`adult princess`または`adult royal woman`とする。
- 若々しさを表現する場合も、原則として`adult woman in her mid-twenties`など、成人であることを明確にする。
- 18～19歳の人物に露出、体型、身体的魅力を組み合わせない。
- 年齢が画像表現上重要でなければ、具体的な年齢数字を記載せず、`adult woman`とする。
- 「少女のような」「幼い」「あどけない」など、成人性を曖昧にする表現を加えない。

## 2. 美しさと体型の表現

性的な身体評価ではなく、シルエット、姿勢、衣装との調和で美しさを定義する。

### 推奨表現

- `model-like elegance`
- `fashion-editorial presence`
- `tall and graceful silhouette`
- `long elegant proportions`
- `refined posture`
- `balanced feminine proportions`
- `poised and self-assured`
- `athletic and graceful`
- `dignified bearing`
- `runway-inspired character design`

### 避ける表現

- 胸、尻、腰、太ももなど、一部分だけを強調する身体評価
- `busty`
- `voluptuous`
- `seductive body`
- `sexy figure`
- `narrow waist`を他の性的な体型指定と組み合わせること
- 胸や脚の大きさ・形状に対する詳細指定
- `perfect body`など、身体そのものを鑑賞対象にする表現

「モデル風」は身体の露出や体型強調ではなく、姿勢、衣装、構図、表情、洗練性で表現する。

## 3. 肌の露出

肌の露出は、衣装デザインとして必要な範囲に限定する。

### 比較的安全な表現

- 肩が見えるイブニングドレス
- 袖のない夏服
- 膝丈または適度なスリットのドレス
- 背中の一部が開いた礼装
- 軽量な舞踏衣装
- 活動しやすい冒険者衣装
- 暑い地域の文化に適した衣装
- ファッションショー風の礼装

### 記述方法

露出自体を強調せず、衣装全体の構造として記述する。

- `an elegant off-shoulder court gown`
- `a sleeveless summer dress with a structured bodice`
- `a formal gown with an asymmetric neckline`
- `a flowing dress designed for a warm southern climate`
- `a tasteful side opening integrated into the layered skirt`
- `editorial fantasy fashion, elegant rather than provocative`

### 避ける構成

- 露出している身体部分を繰り返し強調する
- 胸元と脚と腰を同時に強調する
- 極端に深いネックラインと極端に高いスリットを併用する
- 透ける素材を胸部や腰部の主要素材として指定する
- 濡れた衣装、下着風衣装、寝室、ベッドなどを組み合わせる
- 挑発的なポーズや表情と露出衣装を組み合わせる
- 衣装より身体そのものが主題になる構図

## 4. 表情とポーズ

### 推奨表現

- `calm and self-assured expression`
- `gentle closed-lip smile`
- `composed and dignified`
- `confident editorial pose`
- `relaxed natural standing pose`
- `upright posture`
- `arms resting naturally`
- `formal three-quarter stance`
- `direct but neutral gaze`

### 避ける表現

- `seductive gaze`
- `inviting expression`
- `bedroom eyes`
- `provocative pose`
- 唇、胸、腰、脚を強調するポーズ
- 背中を極端に反らす姿勢
- 不自然に脚を開いた姿勢
- 身体を鑑賞させることが主目的のローアングル

## 5. 構図

全身像では、キャラクターデザイン資料またはファッションイラストとして構成する。

### 推奨表現

- `full-length character design`
- `head-to-toe view`
- `entire figure visible`
- `centered character-sheet composition`
- `fashion editorial composition`
- `eye-level camera`
- `neutral three-quarter view`
- `generous space above the head and below the feet`

極端なローアングル、胸部のクローズアップ、腰や脚だけの切り取りは避ける。

## 6. 衣装の記述

身体ではなく、次の要素を具体的に定義する。

- シルエット
- 素材
- 色
- 袖
- 襟
- スカート丈
- レイヤー構造
- 刺繍
- 装飾品
- キャラクターの身分や職業
- 地域の気候
- 動きやすさ
- 儀礼性

例：

`a fitted structured bodice flowing into a layered floor-length skirt, lightweight silk and linen, restrained gold embroidery, elegant court tailoring`

## 7. `--no`の使用

- 人物プロンプトでは、原則として`--no`を最小限にする。
- 欲しくない状態は、可能な限り肯定形で置き換える。
- Midjourneyは`--no`以下を単語単位で読むため、複数語の意味が分解される可能性がある。
- `--no modern clothing`は`no clothing`と誤解される可能性があるため使用しない。
- センシティブな身体用語を`--no`に入れない。
- 肌の色や民族的特徴を`--no`で除外しない。
- `--no`には、武器、追加人物、ロゴ、文字など、非センシティブな物体だけを指定する。

### 悪い例

`--no modern clothing, busty, cleavage, dark skin, thigh slit`

### 改善例

本文で以下のように肯定的に記述する。

- `wearing a complete Western fantasy court gown`
- `a continuous layered skirt from waist to hem`
- `modest structured neckline`
- `restrained and dignified styling`

必要な場合の`--no`：

`--no weapon, armor, additional characters, text, watermark`

## 8. 参照画像・Omni Reference

- テキストが安全でも、参照画像自体がモデレーション対象になる。
- 参照画像に若く見える人物、大きなスリット、下着風衣装、強い身体強調がある場合、生成意図と無関係でも拒否される可能性がある。
- 顔と髪型だけを維持したい場合は、参照画像を頭頂から胸または腰までにトリミングする。
- 不要な露出部分、脚、深いスリット、背景人物などは参照画像から外す。
- 参照画像は、可能であれば「明確に成人」「自然な姿勢」「通常の衣装」「非性的な構図」のものを使用する。
- Midjourneyの入力欄に以前の参照画像が固定されていないか確認する。
- Omni Reference、Image Prompt、Style Referenceを混同しない。
- URLは山括弧や説明文を含めず、実際の画像URLだけを指定する。

例：

`--oref https://s.mj.run/XXXXXXXXXXX --ow 75`

## 9. エラー発生時の切り分け

生成が拒否された場合、言葉を無作為に変更し続けず、次の順で原因を確認する。

1. `--oref`、画像プロンプト、スタイル参照をすべて外す。
2. `--no`を完全に削除する。
3. `--style raw`を一度外す。
4. 年齢、体型、肌の露出に関する記述を外す。
5. 人物なしの背景プロンプトが通るか確認する。
6. `adult woman`を含む最小人物プロンプトを試す。
7. 衣装、髪、背景を一項目ずつ戻す。
8. 最後に参照画像を追加する。
9. 参照画像を追加した時点で拒否された場合は、画像を安全な範囲にトリミングまたは変更する。

## 10. 推奨プロンプト構造

1. 明確な成人女性であること
2. キャラクターの役割・身分
3. 表情と人格
4. 髪、瞳、顔立ち
5. 衣装全体の構造
6. 非性的な立ち姿
7. 背景と物語世界
8. ファッション／キャラクターイラストとしての画風
9. 最小限のパラメーター
10. 必要な場合のみ安全な`--no`

## 11. 安全な基本テンプレート

```text
full-length stylized fantasy character illustration of an adult woman,
[role and social position],
[hair, eyes and distinctive facial features],
calm and self-assured expression,
graceful model-like presence and refined posture,

wearing [complete description of the fantasy outfit],
[materials, colors, silhouette and decorative details],
elegant fashion-oriented character design,
tasteful and dignified styling,

standing in a natural eye-level full-body composition,
entire figure visible from head to footwear,
[fantasy environment and lighting],

contemporary fantasy novel cover aesthetics,
polished semi-realistic digital illustration,
fashion-editorial elegance,
non-provocative presentation

--ar 2:3 --v 7
```

## 11-2. 写実版テンプレート（リアル寄り）

第11節のテンプレートはイラスト前提の構成であり、そのまま使うとアニメ調に寄る。実写寄りの画風を求める場合は本テンプレートを使用する。

### アニメ調に引く語（写実路線では使用しない）

| 語 | 作用 |
|---|---|
| `stylized` | 「様式化」＝実写から離せという直接の指示。最大の要因 |
| `character illustration` | キャラ絵の学習データに強く結びつき、アニメ・ゲーム系の絵柄を呼び込む |
| `semi-realistic` | 「完全なリアルではない」という明示 |
| `digital illustration` | 同上 |
| `fantasy novel cover aesthetics` | 近年のファンタジー小説表紙はライトノベル系イラストの比率が高い |
| `large eyes` | **アニメ絵の最大の特徴量。**写実路線では致命的 |
| `fantasy`（衣装・世界の修飾として多用した場合） | イラスト方向に寄与する |

### 置換対応表

| イラスト版 | 写実版 |
|---|---|
| `stylized fantasy character illustration` | `cinematic photograph` |
| `large deep amber eyes` | `deep amber eyes`（`large` を削除） |
| `polished semi-realistic digital illustration` | `photorealistic, historical drama film still` |
| `contemporary fantasy novel cover aesthetics` | `naturalistic color grading` |
| `fashion-editorial elegance` | `shot on 85mm lens, shallow depth of field` |
| `fantasy day dress` | `historical day dress` |
| （追加） | `natural skin texture with visible pores and fine detail` |
| （追加） | `--style raw` |

### 写実版基本テンプレート

```text
full-length cinematic photograph of an adult woman in her mid-twenties,
[role and social position],
[hair, eyes and distinctive facial features],
natural skin texture with visible pores and fine detail,
calm and self-assured expression,
refined posture and graceful bearing,

wearing [complete description of the historical outfit],
[materials, colors, silhouette and decorative details],
understated and dignified styling,

standing in a natural eye-level full-body composition,
entire figure visible from head to footwear,
[environment and lighting],

shot on 85mm lens, shallow depth of field,
photorealistic, historical drama film still,
naturalistic color grading,
non-provocative presentation

--ar 2:3 --v 7 --style raw --no weapon, additional characters, text, watermark
```

### 調整の指針

- まだ絵っぽさが残る場合：`--style raw` の効きを確認 → `fantasy` 系の語を全削除 → 照明を具体化、の順で触る
- リアルすぎて世界観が消えた場合：`historical drama film still` を `epic fantasy film still` に戻すと、写実性を保ったまま幻想寄りに調整できる
- 安全要件（成人明示・体型強調の回避・`--no` の扱い）は第1〜7節をそのまま適用する。**写実版であっても要件は緩まない**

------

## 12. 出力前チェック

ClaudeはMidjourney用プロンプトを出力する前に、次を確認する。

- 人物が明確な成人か
- `girl`など年齢が曖昧な表現がないか
- 若年表現と身体的魅力の強調が混在していないか
- 露出箇所を過度に反復していないか
- 表情やポーズが挑発的になっていないか
- 身体ではなく衣装と人物像が主題になっているか
- `--no`にセンシティブな単語が入っていないか
- `--no modern clothing`のような誤分解される表現がないか
- 参照画像自体に不要な露出や曖昧な年齢表現がないか
- 露出を削除した結果、ユーザーが求めるファッション性まで失われていないか
- 安全性を保証すると断言していないか

## 運用上の原則

露出をすべて禁止するのではなく、「身体を見せるための衣装」ではなく、「ファンタジー世界の気候・身分・職業・ファッションとして設計された衣装」として記述する。

安全判定はMidjourney側の更新や参照画像によって変動するため、このルールに従っても生成が必ず承認されるとは保証しない。拒否された場合は、上記の切り分け手順で文章と参照画像を個別に確認する。

## 参考

- Midjourney公式「No Parameter」：`--no`以下の各語が独立して解釈される点に注意する。
- URL: https://docs.midjourney.com/hc/en-us/articles/32173351982093-No
