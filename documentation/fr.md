<!-- ELUCENIA technical documentation · centor-mcisaac · fr · no clinical/professional/rights approval -->

# Score de Centor modifié (McIsaac)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/centor-mcisaac)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Température \> 38 °C

`febre`

### Absence de toux

`tosse`

### Ganglions cervicaux antérieurs augmentés de volume et douloureux

`linfo`

### Gonflement ou exsudat amygdalien

`amig`

### Âge

`idade`

- `0` — 15 à 44 ans
- `1` — 3 à 14 ans
- `-1` — ≥ 45 ans

## Édition de la méthode

McIsaac 1998 / Fine 2012 : quatre signes valant 1 point chacun et ajustement selon l’âge ; somme préliminaire de −1 à 5, score final limité de 0 à 4

## Formule documentée

Somme préliminaire : 1 point pour chacun des quatre signes — fièvre \> 38 °C, absence de toux, adénopathies cervicales antérieures douloureuses et gonflement ou exsudat amygdalien —, plus 1 point entre 3 et 14 ans, 0 entre 15 et 44 ans et −1 à partir de 45 ans. La somme préliminaire varie de −1 à 5. Score final : les résultats préliminaires inférieurs à 0 sont ramenés à 0 et ceux supérieurs à 4 à 4, conformément à McIsaac 1998 et Fine 2012. La somme préliminaire est enregistrée séparément ; les probabilités et les décisions de prise en charge n’ont pas reçu d’approbation clinique.

## Limites et population

L’étude McIsaac 1998 a évalué des personnes de 3–76 ans présentant de nouveaux symptômes respiratoires en médecine de famille, en comparant le score à une culture oropharyngée. Le total ne confirme pas avec certitude une infection streptococcique ni une indication automatique d’antibiotique. Les pondérations d’âge, seuils et stratégie de test doivent suivre le tableau et la recommandation de la version utilisée. L’édition originale de 1998 et la méthode décrite par Fine en 2012 définissent le score final entre 0 et 4. La somme préliminaire de −1 à 5 constitue une information de calcul distincte et ne doit pas être considérée comme le score final de ces éditions. La vérification porte uniquement sur les pondérations et cette normalisation ; elle n’approuve ni l’évaluation des signes, ni les performances diagnostiques, ni les probabilités, ni les tests, ni le traitement.

## Références

- [McIsaac WJ et al. A clinical score to reduce unnecessary antibiotic use in patients with sore throat. CMAJ, 1998.](https://pubmed.ncbi.nlm.nih.gov/9475915/)

- [Centor RM et al. The diagnosis of strep throat in adults in the emergency room. Med Decis Making, 1981.](https://doi.org/10.1177/0272989X8100100304)

- [Shulman ST et al. Clinical practice guideline for the diagnosis and management of group A streptococcal pharyngitis: 2012 update by the Infectious Diseases Society of America. Clin Infect Dis, 2012.](https://doi.org/10.1093/cid/cis629)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
