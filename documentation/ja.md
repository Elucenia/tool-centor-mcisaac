<!-- ELUCENIA technical documentation · centor-mcisaac · ja · no clinical/professional/rights approval -->

# 修正Centorスコア（McIsaac）

[条件・出典・許諾](https://elucenia.org/ja/tools/centor-mcisaac)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 体温 \> 38 °C

`febre`

### 咳なし

`tosse`

### 前頸部リンパ節の腫大・圧痛

`linfo`

### 扁桃腫脹または滲出物

`amig`

### 年齢

`idade`

- `0` — 15 ～ 44 歳
- `1` — 3 ～ 14 歳
- `-1` — ≥ 45 歳

## 方法の版

McIsaac 1998 / Fine 2012：各1点の4所見と年齢補正。暫定合計は−1～5、最終スコアは0～4に制限

## 記載された計算式

暫定合計：4つの所見（発熱\>38 °C、咳がないこと、圧痛を伴う前頸部リンパ節腫大、扁桃腫脹または滲出）にそれぞれ1点を与え、年齢が3～14歳なら1点、15～44歳なら0点、45歳以上なら−1点を加えます。暫定合計の範囲は−1～5です。最終スコア：McIsaac 1998およびFine 2012に従い、暫定結果が0未満なら0、4を超えるなら4とします。暫定合計は別に記録されます。確率や対応方針について、臨床的な承認は行われていません。

## 限界・対象集団

McIsaac 1998の研究は、家庭医療で新たな呼吸器症状のある3–76歳の人を評価し、スコアを咽頭培養と比較しました。合計点は連鎖球菌感染を確実に示すものではなく、抗菌薬の自動的な適応にもなりません。年齢の重み、閾値、検査方針は、使用する版の表とガイドラインに従う必要があります。 1998年の原版とFineが2012年に記述した方法では、最終スコアを0～4と定義しています。−1～5の暫定合計は別の計算情報であり、これらの版の最終スコアとして扱ってはいけません。今回の確認は重みとこの正規化だけを対象とし、徴候の評価、診断性能、確率、検査、治療を承認するものではありません。

## 参考文献

- [McIsaac WJ et al. A clinical score to reduce unnecessary antibiotic use in patients with sore throat. CMAJ, 1998.](https://pubmed.ncbi.nlm.nih.gov/9475915/)

- [Centor RM et al. The diagnosis of strep throat in adults in the emergency room. Med Decis Making, 1981.](https://doi.org/10.1177/0272989X8100100304)

- [Shulman ST et al. Clinical practice guideline for the diagnosis and management of group A streptococcal pharyngitis: 2012 update by the Infectious Diseases Society of America. Clin Infect Dis, 2012.](https://doi.org/10.1093/cid/cis629)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
