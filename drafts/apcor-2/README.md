# Dataset 'apcor-2'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-2/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-2/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Text | `div@text` | Automatically translated into named div |
| Item | `div@item` | Automatically translated into named div |
| Line | `lb` |  |
| Part | `div@part` | Automatically translated into named div |

### Structural overview
```text
text (@xml:lang=und-Latn-x-glpt)
  body
    div (@data-level=1, @n, @type=item, @xml:id)
      p (@xml:id)
        [lb (@n) (multiple)]
        [note (@xml:id, @xml:lang=por-Latn) (multiple)]
          [foreign (@xml:lang=und-Latn-x-glpt) (multiple)]
        [foreign (@xml:lang=lat-Latn) (multiple)]
        [lb (@n, @xml:lang=lat-Latn) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="r." xml:id="item-1" type="item" data-level="1">
				<p xml:id="item-1-p-1">
					<lb n="1"/>In Ch(risti) n(omi)ne, am(en). Eu Eluira Sanchiz offeyro o meu corpo aas virtudes de Sam Saluador do mo(c)n(steyro) de Vayram (e) <note xml:id="item-1-p-1-note-1" xml:lang="por-Latn">Substituí o sinal tironiano 7 por (e), porque foi a copulativa <foreign xml:lang="und-Latn-x-glpt">e</foreign> que o notário usou na segunda linha: «e as tres...»</note>  offeyro com o meu corpo<lb n="2"/>todo o h(er)damento que eu ey en Centegãus e as tres quartas do padroadigo dessa eygleyga (e) todo hu h(er)dam(en)to d(e) Crexe- mil assy<lb n="3"/>us das Sestas como todo u outro h(er)dam(en)to que uaia <note xml:id="item-1-p-1-note-2" xml:lang="por-Latn">Deve ser <foreign xml:lang="und-Latn-x-glpt">uala</foreign> (= valha para o mosteiro...), porque no«Auto de partilhas» de 1192 há uma expressão equivalente: « <foreign xml:lang="und-Latn-x-glpt">que uallam por en secula seculorum, amen</foreign> », ou, então, «que vão para o mosteiro».</note>  u moensteyro de Vayram por en s(e)c(u)la s(e)c(u)lor(um), am(en). <foreign xml:lang="lat-Latn">F(a)c(t)a karta m(en)se S(ep)t(em)b(e)r E(ra)</foreign>
					<lb n="4" xml:lang="lat-Latn"/>M <foreign xml:lang="lat-Latn">a</foreign> CC <foreign xml:lang="lat-Latn">a</foreign> XXX. I. <foreign xml:lang="lat-Latn">a</foreign> . M(e)n(en)d(us) Sanchiz ts., Steph(a)m Suariz ts., Vermuíí Ordoniz ts., <note xml:id="item-1-p-1-note-3" xml:lang="por-Latn">As duas últimas testemunhas subscreveram também o «Auto de partilhas» de 1192.</note>  Sancho Diaz ts., Gonsaluu Diaz testes. Ego<lb n="5" xml:lang="lat-Latn"/>Gonsalu(us) Pet(ri) p(res)b(iter)r notauit.</p>
			</div>
```
