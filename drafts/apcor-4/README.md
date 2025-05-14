# Dataset 'apcor-4'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-4/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-4/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Text | `div@text` | Automatically translated into named div |
| Part | `div@part` | Automatically translated into named div |
| Item | `pb` |  |
| Line | `lb` |  |

### Structural overview
```text
text (@xml:lang=und-Latn-x-glpt)
  body
    p (@xml:id)
      [lb (@n) (multiple)]
      [note (@xml:id, @xml:lang=por-Latn) (multiple)]
        [foreign (@xml:lang=und-Latn-x-glpt) (multiple)]
      [note (@xml:id)]
        [foreign (@xml:lang=por-Latn)]
      [pb (@n)]
    [pb (@n)]
```

### Structure Example

```xml
<pb xmlns="http://www.tei-c.org/ns/1.0" n="r."/>
```
