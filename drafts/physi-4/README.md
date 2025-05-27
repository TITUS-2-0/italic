# Dataset 'Physiologus: The Latin Version'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/lat/physioll/physi.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/physi-4/
* version: unreleased
* date: 2025-01-13

## Citation
```text
Digital version of Physiologus: The Latin Version (draft version). By: Jost Gippert, Thomas Klein, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/physi-4/, visited on <insert date>)
```

## TEI encoding
* hardcoded text numbers are removed from titles, as they are encoded in the `head@n` attribute
* inline corrections/readings are transformed into <choice> elements with <corr> and <sic> sub-elements
* everything is wrapped in <p> elements

* fixes:
    * duplicate <pb> elements are removed

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Text` (hierarchical) | `div@text` (hierarchical) | Automatically translated into named div |
| `Page of ed.` (hierarchical) | `pb@edition` (linear) |  |
| `Line` (hierarchical) | `lb` (linear) |  |

### Structural overview
```text
text (@xml:lang=lat-Latn)
  body
    div (@data-level=1, @n, @type=text, @xml:id) (multiple)
      head (@n) (multiple)
      p (@xml:id) (multiple)
        choice (multiple)
          corr (multiple)
          sic (multiple)
        [lb (@n) (multiple)]
        [pb (@n, @type=edition) (multiple)]
        [foreign (@xml:lang=und-Latn-x-general) (multiple)]
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [pb (@n, @type=edition)]
      [pb (@n, @type=edition) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="text-1" type="text" data-level="1">
        <pb type="edition" n="124"/>
        <head n="1">De leone.</head>
        <p xml:id="text-1-p-1">
          <lb n="2"/>* Igitur Jacob benedicens filium suum Juda dicebat »Catulus leonis
          <lb n="3"/>Juda filius ....« Tres naturas habet leo: prima, cum ambulat in
          <lb n="4"/>montibus vel silvis, si evenerit, ut queratur a venatoribus, et veniet
          <lb n="5"/>ei odor venatoris ad nares, statim cum cauda delet post se vestigia sua
          <lb n="6"/>quocumque ierit, ut non secutus venator vestigia capiat eum. Sic et
          <lb n="7"/>dominus noster ... missus a sempiterno patre cooperuit intelligibilia
          <lb n="8"/>deitatis sue vestigia. ... Cum dormierit leo, vigilant oculi ejus.
          <lb n="9"/>In aperiendo * sicut et in cantico canticorum testatur sponsus de se
  ...
```
