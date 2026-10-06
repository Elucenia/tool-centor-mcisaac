<!-- ELUCENIA technical documentation · centor-mcisaac · pt-BR · no clinical/professional/rights approval -->

# Escore de Centor modificado (McIsaac)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/centor-mcisaac)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Temperatura \> 38 °C

`febre`

### Ausência de tosse

`tosse`

### Linfonodos cervicais anteriores aumentados e dolorosos

`linfo`

### Edema ou exsudato amigdaliano

`amig`

### Idade

`idade`

- `0` — 15 a 44 anos
- `1` — 3 a 14 anos
- `-1` — ≥ 45 anos

## Edição do método

McIsaac 1998 / Fine 2012: quatro achados de 1 ponto e ajuste etário; soma preliminar −1 a 5, pontuação final limitada a 0 a 4

## Fórmula documentada

Soma preliminar: 1 ponto para cada um dos quatro achados — febre \> 38 °C, ausência de tosse, adenomegalia cervical anterior dolorosa, edema ou exsudato amigdaliano —, mais 1 ponto entre 3 e 14 anos, 0 entre 15 e 44 anos e −1 a partir de 45 anos. A soma preliminar varia de −1 a 5. Pontuação final: resultados preliminares abaixo de 0 são definidos como 0 e acima de 4 como 4, conforme McIsaac 1998 e Fine 2012. A soma preliminar é registrada separadamente; probabilidades e condutas não foram aprovadas clinicamente.

## Limites e população

O estudo McIsaac 1998 avaliou pessoas de 3–76 anos com sintomas respiratórios novos em medicina de família, comparando o escore com cultura de orofaringe. O total não estabelece certeza de estreptococo nem indicação automática de antibiótico. Pesos de idade, cortes e estratégia de teste devem seguir a tabela e a diretriz da versão utilizada. A edição original de 1998 e o método descrito por Fine em 2012 definem a pontuação final entre 0 e 4. A soma preliminar de −1 a 5 é informação de cálculo separada e não deve ser tratada como a pontuação final dessas edições. A conferência abrange apenas os pesos e essa normalização; não aprova observação dos sinais, desempenho diagnóstico, probabilidades, teste ou tratamento.

## Referências

- [McIsaac WJ et al. A clinical score to reduce unnecessary antibiotic use in patients with sore throat. CMAJ, 1998.](https://pubmed.ncbi.nlm.nih.gov/9475915/)

- [Centor RM et al. The diagnosis of strep throat in adults in the emergency room. Med Decis Making, 1981.](https://doi.org/10.1177/0272989X8100100304)

- [Shulman ST et al. Clinical practice guideline for the diagnosis and management of group A streptococcal pharyngitis: 2012 update by the Infectious Diseases Society of America. Clin Infect Dis, 2012.](https://doi.org/10.1093/cid/cis629)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Probabilidade de estreptococo de 1 a 2,5%

Sem teste e sem antibiótico.


### 2

Probabilidade de estreptococo de 11 a 17%

Teste rápido ou cultura; antibiótico só se positivo.


### 3

Probabilidade de estreptococo de 51 a 53%

Testar e tratar se positivo; na falta de teste, considerar antibiótico empírico.


### 4

Probabilidade de estreptococo de 28 a 35%

Teste rápido ou cultura; antibiótico só se positivo.

