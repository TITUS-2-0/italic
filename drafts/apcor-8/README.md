# Dataset 'apcor-8'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm?apcor008.htmapcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-8/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-8/, visited on <insert date>)
```

## TEI encoding
* footnotes are moved into inline `note` elements (for now)
* all content is wrapped in `p` elements
* linebreaks marked with "/" are translated into "-" + `lb@break="no"`
* fixes:

    * remove footnote numbers
    * fix language tags
    * brackets are removed from line breaks
    * various wrong encodings in the notes
    * adjacent strings are concatenated

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Text` (hierarchical) | `div@text` (hierarchical) | Automatically translated into named div |
| `Part` (linear) | `milestone@part` (linear) |  |
| `Item` (hierarchical) | `pb` (linear) |  |
| `Line` (hierarchical) | `lb` (linear) |  |

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
        <lb n="2"/>foy muyto peccatriz<note xml:id="p-1-note-1">peccatriz: <foreign xml:lang="por-Latn">JJN</foreign> peccatrix.</note>
        <pb n="66v"/>
        <lb n="1"/>
        <milestone unit="part" n="2" type="inline" xml:id="p-1-milestone-2"/>Hũa mançeba<note xml:id="p-1-note-2">mançeba: <foreign xml:lang="por-Latn">JJN</foreign> manceba  <foreign xml:lang="por-Latn">(comportamento sistemático em Nunes, que deixo de anotar).</foreign>
        </note> foy do mundo que chamavã<note xml:id="p-1-note-3">chamavã: <foreign xml:lang="por-Latn">JJN</foreign> chamavam  <foreign xml:lang="por-Latn">(comportamento sistemático em Nunes, que deixo de anotar).</foreign>
        </note>
        <lb n="2"/>Tarsis e era de tamanha fremosura que muitos
        <lb n="3"/>venderõ os beës<note xml:id="p-1-note-4">beës: <foreign xml:lang="por-Latn">JJN</foreign> bëes  <foreign xml:lang="por-Latn">(comportamento sistemático em Nunes, que deixo de anotar).</foreign>
        </note> que avyam por ella e veerom a
  ...
```
