<!-- ELUCENIA technical documentation · centor-mcisaac · es · no clinical/professional/rights approval -->

# Puntuación de Centor modificada (McIsaac)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/centor-mcisaac)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Temperatura \> 38 °C

`febre`

### Ausencia de tos

`tosse`

### Ganglios cervicales anteriores aumentados y dolorosos

`linfo`

### Edema o exudado amigdalar

`amig`

### Edad

`idade`

- `0` — 15 a 44 años
- `1` — 3 a 14 años
- `-1` — ≥ 45 años

## Edición del método

McIsaac 1998 / Fine 2012: cuatro hallazgos de 1 punto y ajuste por edad; suma preliminar de −1 a 5, puntuación final limitada de 0 a 4

## Fórmula documentada

Suma preliminar: 1 punto por cada uno de los cuatro hallazgos — fiebre \> 38 °C, ausencia de tos, adenopatía cervical anterior dolorosa y edema o exudado amigdalar —, más 1 punto entre los 3 y los 14 años, 0 entre los 15 y los 44 años y −1 a partir de los 45 años. La suma preliminar varía de −1 a 5. Puntuación final: los resultados preliminares inferiores a 0 se fijan en 0 y los superiores a 4 en 4, conforme a McIsaac 1998 y Fine 2012. La suma preliminar se registra por separado; las probabilidades y las decisiones de manejo no han recibido aprobación clínica.

## Límites y población

El estudio McIsaac 1998 evaluó a personas de 3–76 años con síntomas respiratorios nuevos en medicina de familia, comparando la puntuación con el cultivo faríngeo. El total no establece certeza de infección estreptocócica ni una indicación automática de antibióticos. Los pesos de edad, los puntos de corte y la estrategia de pruebas deben seguir la tabla y la guía de la versión utilizada. La edición original de 1998 y el método descrito por Fine en 2012 definen la puntuación final entre 0 y 4. La suma preliminar de −1 a 5 es información de cálculo separada y no debe tratarse como la puntuación final de esas ediciones. La comprobación abarca solo los pesos y esta normalización; no aprueba la evaluación de los signos, el desempeño diagnóstico, las probabilidades, las pruebas ni el tratamiento.

## Referencias

- [McIsaac WJ et al. A clinical score to reduce unnecessary antibiotic use in patients with sore throat. CMAJ, 1998.](https://pubmed.ncbi.nlm.nih.gov/9475915/)

- [Centor RM et al. The diagnosis of strep throat in adults in the emergency room. Med Decis Making, 1981.](https://doi.org/10.1177/0272989X8100100304)

- [Shulman ST et al. Clinical practice guideline for the diagnosis and management of group A streptococcal pharyngitis: 2012 update by the Infectious Diseases Society of America. Clin Infect Dis, 2012.](https://doi.org/10.1093/cid/cis629)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
