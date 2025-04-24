# Dataset 'La Rettorica (1261)'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aital/latrett/latre.htm).

* URL: https://titus2.uni-frankfurt.de/dataset/latre
* version: 0.1.0
* date: 2025-04-23

## Citation
```text
Digital version of La Rettorica (1261) by Brunetto Latini (v0.1.0). By: Gisella Ferraresi, Jost Gippert, Maria Goldbach, Florian Matter, Esther Rinke. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://titus2.uni-frankfurt.de/dataset/latre, visited on <insert date>)
```

## TEI encoding
* the body of the original dataset is split into a ``<front>`` and a ``<body>``
* there are numbered ``<p>`` from TITUS, as well as unnumbered ones to satisfy TEI requirements

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Section | `part` | a more neutral term |
| Paragraph | `p` |  |
| Chapter | `milestone@chapter` | The chapters of Tullio's original are represented linearly, not hierarchically. |
| Page | `Page` |  |
| Line | `Line` |  |

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="part-1" type="part" data-level="1">
				<milestone unit="chapter" n="I" xml:id="part-1-milestone-1"/>
				<p xml:id="part-1-p-2">
					<lb n="6"/>Sovente e molto ò io pensato in me medesimo<lb n="7"/>se lla copia del dicere e lo sommo studio della
<lb n="8"/>eloquenzia àe fatto più bene o più male agli uomini
<lb n="9"/>et alle cittadi; però che quando io considero li dannaggii
<lb n="10"/>del nostro comune e raccolgo nell' animo l' antiche
<lb n="11"/>aversitadi delle grandissime cittadi, veggio che
<lb n="12"/>non picciola parte di danni v' è messa per uomini
<lb n="13"/>molto parlanti sanza sapienza.
<lb n="14"/>Qui parla lo sponitore.</p>
				<p n="1" xml:id="part-1-p-3">
  ...
```
