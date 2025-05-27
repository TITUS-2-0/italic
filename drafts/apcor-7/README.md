# Dataset 'apcor-7'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm?apcor007.htmapcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-7/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-7/, visited on <insert date>)
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
          [foreign (@xml:lang=und-Latn-x-glpt)]
      [pb (@n) (multiple)]
      [lb (@break=no, @n) (multiple)]
    [pb (@n)]
```

### Structure Example

```xml
<p xmlns="http://www.tei-c.org/ns/1.0" xml:id="p-1">
        <lb n="1"/>
        <milestone unit="part" n="1" type="inline" xml:id="p-1-milestone-1"/>Aquy se comeca<note xml:id="p-1-note-1">comeca: <foreign xml:lang="por-Latn">JJN</foreign> começa.</note> a vida d'hũa<note xml:id="p-1-note-2">d'hüa: dhüa, <foreign xml:lang="por-Latn">JJN</foreign> de hüa.</note> muy sancta mõja<note xml:id="p-1-note-3">mõja: <foreign xml:lang="por-Latn">JJN</foreign> monja <foreign xml:lang="por-Latn">(comportamento sistemático em Nunes, que deixo de anotar).</foreign>
        </note>
        <pb n="73v"/>
        <lb n="1"/>
        <milestone unit="part" n="2" type="inline" xml:id="p-1-milestone-2"/>Contou hũu padre santo, dizendo que era hũa
        <lb n="2"/>virgem que aproveytara muito ë no<note xml:id="p-1-note-4">? no: <foreign xml:lang="por-Latn">JJN</foreign> em no.</note> amor
        <lb n="3"/>de Deos, e em seu temor. E preguntey-a que quem<note xml:id="p-1-note-5">preguntey-a que quem: pgunteya q quem, <foreign xml:lang="por-Latn">JJN</foreign> preguntey-a (que) quem.</note>
        <lb n="4"/>a trouvera a tam boa conversaçom de vyda. E
        <lb n="5"/>ella (me) disse<note xml:id="p-1-note-6">ella (me) disse: me <foreign xml:lang="por-Latn">em letra e tinta diferentes, sobre rasura ilegível.</foreign>
        </note> ? Ô homë<note xml:id="p-1-note-7">hom?: <foreign xml:lang="por-Latn">JJN</foreign> homem <foreign xml:lang="por-Latn">(comportamento sistemático em Nunes, que deixo de anotar).</foreign>
  ...
```
