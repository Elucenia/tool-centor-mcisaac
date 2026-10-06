<!-- ELUCENIA technical documentation · centor-mcisaac · en · no clinical/professional/rights approval -->

# Modified Centor score (McIsaac)

[conditions, sources and permissions](https://elucenia.org/en/tools/centor-mcisaac)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Temperature \> 38 °C

`febre`

### Absence of cough

`tosse`

### Enlarged, tender anterior cervical lymph nodes

`linfo`

### Tonsillar swelling or exudate

`amig`

### Age

`idade`

- `0` — 15 to 44 years
- `1` — 3 to 14 years
- `-1` — ≥ 45 years

## Method edition

McIsaac 1998 / Fine 2012: four findings worth 1 point each and an age adjustment; preliminary sum −1 to 5, final score bounded from 0 to 4

## Documented formula

Preliminary sum: 1 point for each of the four findings — fever \> 38 °C, absence of cough, tender anterior cervical lymphadenopathy, and tonsillar swelling or exudate —, plus 1 point at ages 3 to 14 years, 0 at ages 15 to 44 years, and −1 at age 45 years or older. The preliminary sum ranges from −1 to 5. Final score: preliminary results below 0 are set to 0 and those above 4 are set to 4, as described by McIsaac 1998 and Fine 2012. The preliminary sum is recorded separately; probabilities and management decisions have not received clinical approval.

## Limits and population

McIsaac’s 1998 study assessed people aged 3–76 years with new respiratory symptoms in family medicine, comparing the score with throat culture. The total does not establish certainty of streptococcal infection or an automatic indication for antibiotics. Age weights, cutoffs and testing strategy must follow the table and guideline for the version used. The original 1998 edition and the method described by Fine in 2012 define the final score from 0 to 4. The preliminary sum from −1 to 5 is separate calculation information and must not be treated as the final score of these editions. The review covers only the weights and this normalization; it does not approve ascertainment of the signs, diagnostic performance, probabilities, testing or treatment.

## References

- [McIsaac WJ et al. A clinical score to reduce unnecessary antibiotic use in patients with sore throat. CMAJ, 1998.](https://pubmed.ncbi.nlm.nih.gov/9475915/)

- [Centor RM et al. The diagnosis of strep throat in adults in the emergency room. Med Decis Making, 1981.](https://doi.org/10.1177/0272989X8100100304)

- [Shulman ST et al. Clinical practice guideline for the diagnosis and management of group A streptococcal pharyngitis: 2012 update by the Infectious Diseases Society of America. Clin Infect Dis, 2012.](https://doi.org/10.1093/cid/cis629)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Probability of streptococcus from 1 to 2.5%

No test and no antibiotic.


### 2

Probability of streptococcus from 11 to 17%

Rapid test or culture; antibiotic only if positive.


### 3

Probability of streptococcus from 51 to 53%

Test and treat if positive; if no test is available, consider empiric antibiotic.


### 4

Probability of streptococcus from 28 to 35%

Rapid test or culture; antibiotic only if positive.

