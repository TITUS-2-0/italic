# Dataset 'apcor-8'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-8/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-8/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Text | `div@text` | Automatically translated into named div |
| Part | `milestone@part` |  |
| Item | `pb` |  |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=und-Latn-x-glpt)
  body
    p (@xml:id)
      [lb (@n) (multiple)]
      [milestone (@n, @type=inline, @unit=part, @xml:id) (multiple)]
      [note (@xml:id) (multiple)]
        [foreign (@xml:lang=por-Latn) (multiple)]
          [foreign (@xml:lang=por-Latn) (multiple)]
      [pb (@n) (multiple)]
      [lb (@break=no, @n) (multiple)]
    [pb (@n)]
```

### Structure Example

```xml
<p xmlns="http://www.tei-c.org/ns/1.0" xml:id="p-1">
        <lb n="1"/>
        <milestone unit="part" n="1" type="inline" xml:id="p-1-milestone-1"/>Aquy se começa a vida de Tarssis molher que
        <lb n="2"/>foy muyto peccatriz
        <note xml:id="p-1-note-1">
          peccatriz:
          <foreign xml:lang="por-Latn">JJN</foreign>
          peccatrix.
        </note>
        <pb n="66v"/>
        <lb n="1"/>
        <milestone unit="part" n="2" type="inline" xml:id="p-1-milestone-2"/>Hũa mançeba
  ...
```
