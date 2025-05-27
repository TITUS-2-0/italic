# Dataset 'apcor-4'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm?apcor004.htmapcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-4/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-4/, visited on <insert date>)
```

## TEI encoding
* footnotes are moved into inline `note` elements (for now)
* all content is wrapped in `p` elements
* fixes:

    * remove footnote numbers
    * fix language tags
    " adjacent strings are concatenated

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Text` (hierarchical) | `div@text` (hierarchical) | Automatically translated into named div |
| `Part` (linear) | `div@part` (linear) | Automatically translated into named div |
| `Item` (hierarchical) | `pb` (linear) |  |
| `Line` (hierarchical) | `lb` (linear) |  |

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
<p xmlns="http://www.tei-c.org/ns/1.0" xml:id="p-1">
        <lb n="1"/>D(e) noticia d(e) torto que fecer(um) a Laurëci(us) Fernãdiz por plazo que fec(e) Gõcauo
        <lb n="2"/>Ramiriz antre suos<note xml:id="p-1-note-1" xml:lang="por-Latn">Nesta palavra e em várias outras o <foreign xml:lang="und-Latn-x-glpt">s</foreign> final vem na entrelinha ou em expoente, assemelhando-se ao sinal abreviativo de <foreign xml:lang="und-Latn-x-glpt">er.</foreign>
        </note> filios e Lourëço Ferrnãdiz q(ua)le podedes saber e oue au(e)r<note xml:id="p-1-note-2" xml:lang="por-Latn">Na palavra <foreign xml:lang="und-Latn-x-glpt">au(e)r</foreign> ('=' haver) e em outras usa um sinal abreviativo parecido com um til em posição quase vertical, podendo indicar a falta de <foreign xml:lang="und-Latn-x-glpt">e</foreign> ou de outras letras e até silabas.</note> d(e) erdad(e)
<lb n="3"/>e d'au(e)r tãto q(uo)me uno d(e) suos filios d(e) aq(uan)to podesë au(e)r d(e) bona d(e) seuo pater e fiolios seu
<lb n="4"/>pater e sua mater. E d(e)pois fecer(um) plazo nouo e cõuë uos a saber q(ua)le in ille se&lt;e&gt;m
<lb n="5"/>taes firmam(en)tos q(ua)les podedes saber<note xml:id="p-1-note-3" xml:lang="por-Latn">Segue-se uma palavra rasurada.</note> Ramiro Gõcaluiz e Gõcaluo Gõca[luiz]
<lb n="6"/>Eluira Gõcaluiz forũ fiadores d(e) sua irmana que orgase aqu[e]le plazo come illos.
<lb n="7"/>Sup(er) isto plazo ar fe(ce)r(um) suo plecto. E a maior aiuda que illos hic cõnocer(um) que les
<lb n="8"/>acanocese Laurëzo Ferrnãdiz sa irdad(e) p(er) p(lec)to<note xml:id="p-1-note-4" xml:lang="por-Latn">Em rigor, a abreviatura desta palavra devia desdobrar-se em <foreign xml:lang="und-Latn-x-glpt">p(re)to,</foreign> mas prefiro <foreign xml:lang="und-Latn-x-glpt">p(lec)to,</foreign> porque é este o sentido e é assim que vem, por extenso, na linha 7.</note> que a teuese o abate d(e) S(an)c(t)o Martino
<lb n="9"/>que como uëcesë<note xml:id="p-1-note-5" xml:lang="por-Latn">Seguem-se, raspadas, umas letras que parecem ser <foreign xml:lang="und-Latn-x-glpt">oct(ra)a.</foreign>
        </note> que asi les dese d(e) ista o abade. E que nunq(ua) illos lecxasë
  ...
```
