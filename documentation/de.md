<!-- ELUCENIA technical documentation · centor-mcisaac · de · no clinical/professional/rights approval -->

# Modifizierter Centor-Score (McIsaac)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/centor-mcisaac)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Temperatur \> 38 °C

`febre`

### Kein Husten

`tosse`

### Vergrößerte, druckschmerzhafte vordere Halslymphknoten

`linfo`

### Tonsillenschwellung oder -exsudat

`amig`

### Alter

`idade`

- `0` — 15 bis 44 Jahre
- `1` — 3 bis 14 Jahre
- `-1` — ≥ 45 Jahre

## Fassung der Methode

McIsaac 1998 / Fine 2012: vier Befunde mit jeweils 1 Punkt und Alterskorrektur; vorläufige Summe −1 bis 5, endgültiger Score auf 0 bis 4 begrenzt

## Dokumentierte Formel

Vorläufige Summe: 1 Punkt für jeden der vier Befunde — Fieber \> 38 °C, fehlender Husten, schmerzhafte vordere zervikale Lymphadenopathie und Tonsillenschwellung oder -exsudat —, zusätzlich 1 Punkt im Alter von 3 bis 14 Jahren, 0 im Alter von 15 bis 44 Jahren und −1 ab 45 Jahren. Die vorläufige Summe reicht von −1 bis 5. Endgültiger Score: Vorläufige Ergebnisse unter 0 werden auf 0 und Ergebnisse über 4 auf 4 gesetzt, entsprechend McIsaac 1998 und Fine 2012. Die vorläufige Summe wird getrennt erfasst; Wahrscheinlichkeiten und Entscheidungen zur Behandlung oder zum weiteren Vorgehen wurden klinisch nicht freigegeben.

## Grenzen und Population

McIsaac 1998 untersuchte Personen von 3–76 Jahren mit neu aufgetretenen Atemwegssymptomen in der Hausarztversorgung und verglich den Score mit einer Oropharynxkultur. Die Summe bestätigt weder eine Streptokokkeninfektion mit Gewissheit noch automatisch eine Antibiotikaindikation. Altersgewichtungen, Schwellen und Teststrategie müssen Tabelle und Leitlinie der verwendeten Version folgen. Die Originalfassung von 1998 und die von Fine 2012 beschriebene Methode definieren den endgültigen Score zwischen 0 und 4. Die vorläufige Summe von −1 bis 5 ist eine separate Recheninformation und darf nicht als endgültiger Score dieser Fassungen behandelt werden. Die Prüfung umfasst nur die Gewichtungen und diese Normalisierung; sie bestätigt weder die Erhebung der Zeichen noch die diagnostische Leistung, Wahrscheinlichkeiten, Tests oder Behandlung.

## Referenzen

- [McIsaac WJ et al. A clinical score to reduce unnecessary antibiotic use in patients with sore throat. CMAJ, 1998.](https://pubmed.ncbi.nlm.nih.gov/9475915/)

- [Centor RM et al. The diagnosis of strep throat in adults in the emergency room. Med Decis Making, 1981.](https://doi.org/10.1177/0272989X8100100304)

- [Shulman ST et al. Clinical practice guideline for the diagnosis and management of group A streptococcal pharyngitis: 2012 update by the Infectious Diseases Society of America. Clin Infect Dis, 2012.](https://doi.org/10.1093/cid/cis629)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
