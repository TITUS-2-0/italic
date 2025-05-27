# Dataset 'oskum'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/oskumb/oskum.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/oskum/
* version: unreleased
* date: 2025-05-07

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/oskum/, visited on <insert date>)
```

## TEI encoding
* the unified latin transliteration is encoded as a `choice` with `orig` and `reg`
* lines are wrapped in `ab` elements with `type=line-wrapper`
* a `gap` element is inserted for missing text
* sources inside the text are deleted for now
* titles are removed, as they are encoded in the preceding `head@n`

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Inscription` (hierarchical) | `div@inscription` (hierarchical) | Automatically translated into named div |
| `Part` (hierarchical) | `div@part` (hierarchical) | Automatically translated into named div |
| `Line` (hierarchical) | `lb` (hierarchical) |  |

### Structural overview
```text
text (@xml:lang=osc-Ital)
  body
    div (@data-level=1, @n, @type=inscription-group, @xml:id) (multiple)
      head (@xml:lang=deu-Latn | eng-Latn) (multiple)
      div (@data-level=2, @n, @type=inscription, @xml:id) (multiple)
        ab (@type=line-wrapper, @xml:id) (multiple)
          choice (multiple)
            orig (multiple)
              [foreign (@xml:lang=osc-Grek-x-grkscrpt | osc-Ital-x-origscr | qbb-Latn | yib-Latn-x-latnscrp) (multiple)]
            reg (multiple)
              [foreign (@xml:lang=osc-Grek-x-grkscrpt | qbb-Latn-x-txl | xum-Latn | yib-Latn-x-latnscrp) (multiple)]
          [lb (@n) (multiple)]
        [milestone (@facs=#facs-2 | #facs-3 | #facs-4, @n, @unit=ref, @xml:id) (multiple)]
        [lb (@n) (multiple)]
      div (@data-level=2, @n, @type=inscription, @xml:id) (multiple)
      div (@data-level=2, @n, @type=inscription, @xml:id)
        ab (@type=line-wrapper, @xml:id) (multiple)
          choice (multiple)
            orig (multiple)
              [foreign (@xml:lang=osc-Ital-x-origscr) (multiple)]
            reg (multiple)
          [lb (@n) (multiple)]
        gap (@reason=missing)
      div (@data-level=2, @n, @type=inscription, @xml:id) (multiple)
        head (@xml:lang=eng-Latn) (multiple)
        ab (@type=line-wrapper, @xml:id) (multiple)
          choice (multiple)
            orig (multiple)
              [foreign (@xml:lang=osc-Ital-x-origscr | yib-Latn-x-latnscrp) (multiple)]
                [foreign (@xml:lang=yib-Latn-x-latnscrp)]
            reg (multiple)
          [lb (@n) (multiple)]
        [milestone (@facs=#facs-1, @unit=ref, @xml:id)]
      div (@data-level=2, @n, @type=inscription, @xml:id)
        head (@xml:lang=eng-Latn)
      div (@data-level=2, @n, @type=inscription, @xml:id)
        gap (@reason=missing)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="IT" xml:id="inscription-group-1" type="inscription-group" data-level="1">
        <head xml:lang="deu-Latn">Iguvinische Tafeln</head>
        <div n="Ia" xml:id="inscription-group-1-inscription-1" type="inscription" data-level="2">
          <milestone facs="#facs-4" unit="ref" n="Ia" xml:id="inscription-group-1-inscription-1-milestone-1"/>
          <ab type="line-wrapper" xml:id="inscription-group-1-inscription-1-ab-1">
            <lb n="1"/>
            <choice>
              <orig>
                <foreign xml:lang="osc-Ital-x-origscr">ESTE: PERSKLUM: AVES: ANZERIATES: ENETU:</foreign>
              </orig>
              <reg>
                <foreign xml:lang="xum-Latn">ESTE: PERSKLUM: AVES: ANZERIATES: ENETU:</foreign>
  ...
```
