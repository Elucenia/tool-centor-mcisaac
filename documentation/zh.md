<!-- ELUCENIA technical documentation · centor-mcisaac · zh · no clinical/professional/rights approval -->

# 改良 Centor 评分（McIsaac）

[条件、来源与许可](https://elucenia.org/zh/tools/centor-mcisaac)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 体温 \> 38 °C

`febre`

### 无咳嗽

`tosse`

### 前颈淋巴结肿大伴压痛

`linfo`

### 扁桃体肿胀或渗出物

`amig`

### 年龄

`idade`

- `0` — 15 至 44 岁
- `1` — 3 至 14 岁
- `-1` — ≥ 45 岁

## 方法版本

McIsaac 1998 / Fine 2012：四项表现各计1分并按年龄调整；初步总和−1至5，最终评分限定为0至4

## 已记录的公式

初步总和：四项表现各计1分——发热\>38 °C、无咳嗽、前颈淋巴结肿大伴压痛、扁桃体肿胀或渗出——并按年龄加分：3至14岁加1分，15至44岁加0分，45岁及以上减1分。初步总和范围为−1至5。最终评分：按照McIsaac 1998和Fine 2012的描述，初步结果低于0时设为0，高于4时设为4。初步总和单独记录；概率和处置决策尚未获得临床批准。

## 限制与适用人群

McIsaac 1998研究在家庭医学中评估了有新发呼吸道症状的3–76岁人群，将评分与咽拭子培养比较。总分不能确定链球菌感染，也不能自动构成抗生素使用指征。年龄权重、阈值和检测策略须遵循所用版本的表格及指南。 1998原版和Fine在2012年描述的方法将最终评分定义为0至4。−1至5的初步总和是单独的计算信息，不应视为这两版的最终评分。本次核对仅涉及权重和这一规范化处理，不代表对体征评估、诊断性能、概率、检测或治疗的批准。

## 参考文献

- [McIsaac WJ et al. A clinical score to reduce unnecessary antibiotic use in patients with sore throat. CMAJ, 1998.](https://pubmed.ncbi.nlm.nih.gov/9475915/)

- [Centor RM et al. The diagnosis of strep throat in adults in the emergency room. Med Decis Making, 1981.](https://doi.org/10.1177/0272989X8100100304)

- [Shulman ST et al. Clinical practice guideline for the diagnosis and management of group A streptococcal pharyngitis: 2012 update by the Infectious Diseases Society of America. Clin Infect Dis, 2012.](https://doi.org/10.1093/cid/cis629)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

链球菌概率为 1 至 2.5%

不检测且不使用抗生素。


### 2

链球菌概率为 11 至 17%

快速检测或培养；仅在阳性时使用抗生素。


### 3

链球菌概率为 51 至 53%

如阳性则检测并治疗；若无检测条件，可考虑经验性使用抗生素。


### 4

链球菌概率为 28 至 35%

快速检测或培养；仅在阳性时使用抗生素。

