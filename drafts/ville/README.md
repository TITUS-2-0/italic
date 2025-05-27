# Dataset 'ville'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/afr/villehar/ville.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/ville/
* version: unreleased
* date: 2025-04-21

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/ville/, visited on <insert date>)
```

## TEI encoding
* no modifications were necessary

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Paragraph` (hierarchical) | `p` (hierarchical) |  |
| `Sentence` (hierarchical) | `s` (hierarchical) |  |

### Structural overview
```text
text (@xml:lang=fro-Latn)
  body
    p (@n, @xml:id) (multiple)
      s (@n, @xml:id) (multiple)
    p (@n, @xml:id) (multiple)
      [lb (@n) (multiple)]
      [foreign (@xml:lang=und-Latn-x-general) (multiple)]
```

### Structure Example

```xml
<p xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="p-1">
        <s n="1" xml:id="p-1-s-1">Seigneur sachiez que mil anz et cent et quatre vinz et XVII anz Aprés l'incarnacion jhesucrist.</s>
        <s n="2" xml:id="p-1-s-2">Au tans innocent apostele de ronme.</s>
        <s n="3" xml:id="p-1-s-3">et phelippe roy de france. et richart roy d'engleterre ot I saint home qui ot a non forques de nuelli.</s>
        <s n="4" xml:id="p-1-s-4">Ce nuelli siet entre laigni sus marne et paris.</s>
        <s n="5" xml:id="p-1-s-5">Et il iert prestres et tenoit la parroisse de la vile.</s>
        <s n="6" xml:id="p-1-s-6">et cil fourques dont je vous di comenca a parler de dieu par france et par les autres pais d'entour.</s>
        <s n="7" xml:id="p-1-s-7">Et sachiez que nostre sires fist maintes miracles pour lui.</s>
      </p>
```
