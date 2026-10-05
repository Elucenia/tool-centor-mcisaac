<!-- ELUCENIA technical documentation · centor-mcisaac · it · no clinical/professional/rights approval -->

# Punteggio di Centor modificato (McIsaac)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/centor-mcisaac)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Temperatura \> 38 °C

`febre`

### Assenza di tosse

`tosse`

### Linfonodi cervicali anteriori ingrossati e dolenti

`linfo`

### Edema o essudato tonsillare

`amig`

### Età

`idade`

- `0` — 15 a 44 anni
- `1` — 3 a 14 anni
- `-1` — ≥ 45 anni

## Edizione del metodo

McIsaac 1998 / Fine 2012: quattro reperti da 1 punto e aggiustamento per età; somma preliminare da −1 a 5, punteggio finale limitato da 0 a 4

## Formula documentata

Somma preliminare: 1 punto per ciascuno dei quattro reperti — febbre \> 38 °C, assenza di tosse, linfoadenopatia cervicale anteriore dolente ed edema o essudato tonsillare —, più 1 punto tra 3 e 14 anni, 0 tra 15 e 44 anni e −1 a partire dai 45 anni. La somma preliminare varia da −1 a 5. Punteggio finale: i risultati preliminari inferiori a 0 vengono portati a 0 e quelli superiori a 4 a 4, secondo McIsaac 1998 e Fine 2012. La somma preliminare viene registrata separatamente; le probabilità e le decisioni di gestione non hanno ricevuto approvazione clinica.

## Limiti e popolazione

Lo studio McIsaac 1998 ha valutato persone di 3–76 anni con nuovi sintomi respiratori in medicina di famiglia, confrontando il punteggio con la coltura faringea. Il totale non stabilisce la certezza di un’infezione streptococcica né un’indicazione automatica agli antibiotici. Pesi per l’età, soglie e strategia dei test devono seguire la tabella e la linea guida della versione utilizzata. L’edizione originale del 1998 e il metodo descritto da Fine nel 2012 definiscono il punteggio finale tra 0 e 4. La somma preliminare da −1 a 5 è un’informazione di calcolo separata e non deve essere trattata come il punteggio finale di queste edizioni. La verifica riguarda solo i pesi e questa normalizzazione; non approva la valutazione dei segni, le prestazioni diagnostiche, le probabilità, i test o il trattamento.

## Riferimenti

- [McIsaac WJ et al. A clinical score to reduce unnecessary antibiotic use in patients with sore throat. CMAJ, 1998.](https://pubmed.ncbi.nlm.nih.gov/9475915/)

- [Centor RM et al. The diagnosis of strep throat in adults in the emergency room. Med Decis Making, 1981.](https://doi.org/10.1177/0272989X8100100304)

- [Shulman ST et al. Clinical practice guideline for the diagnosis and management of group A streptococcal pharyngitis: 2012 update by the Infectious Diseases Society of America. Clin Infect Dis, 2012.](https://doi.org/10.1093/cid/cis629)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
