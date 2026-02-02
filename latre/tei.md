* the body of the original dataset is split into a ``<front>`` and a ``<body>``
* there are numbered ``<p>`` from TITUS, as well as unnumbered ones to satisfy TEI requirements

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Section` (hierarchical) | `part` (hierarchical) | a more neutral term |
| `Paragraph` (hierarchical) | `p` (hierarchical) |  |
| `Chapter` (linear) | `milestone@chapter` (linear) | The chapters of Tullio's original are represented linearly, not hierarchically. |
| `Page` (linear) | `pb` (linear) |  |
| `Line` (linear) | `lb` (linear) |  |

### Structural overview
```text
text (@xml:lang=ita-Latn-x-old)
  front (@xml:id)
    p (@xml:id)
      [pb (@n)]
      [lb (@n) (multiple)]
  body
    div (@data-level=1, @n, @type=part, @xml:id) (multiple)
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [pb (@n) (multiple)]
      p (@n, @xml:id) (multiple)
        [lb (@n) (multiple)]
        [pb (@n) (multiple)]
      [milestone (@n, @unit=chapter, @xml:id) (multiple)]
      [pb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="part-1" type="part" data-level="1">
        <milestone unit="chapter" n="I" xml:id="part-1-milestone-1"/>
        <p xml:id="part-1-p-2">
          <lb n="6"/>Sovente e molto ò io pensato in me medesimo
          <lb n="7"/>se lla copia del dicere e lo sommo studio della
          <lb n="8"/>eloquenzia àe fatto più bene o più male agli uomini
          <lb n="9"/>et alle cittadi; però che quando io considero li dannaggii
          <lb n="10"/>del nostro comune e raccolgo nell' animo l' antiche
          <lb n="11"/>aversitadi delle grandissime cittadi, veggio che
          <lb n="12"/>non picciola parte di danni v' è messa per uomini
          <lb n="13"/>molto parlanti sanza sapienza.
          <lb n="14"/>Qui parla lo sponitore.</p>
  ...
```
