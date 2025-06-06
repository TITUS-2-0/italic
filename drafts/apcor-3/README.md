# Dataset 'apcor-3'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm?apcor003.htmapcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-3/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-3/, visited on <insert date>)
```

## TEI encoding
* footnotes are moved into inline `note` elements (for now)
* all content is wrapped in `p` elements
* fixes:

    * remove footnote numbers
    * fix language tags

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
text (@xml:lang=lat-Latn)
  body
    p (@xml:id)
      [lb (@n) (multiple)]
      [note (@xml:id, @xml:lang=por-Latn) (multiple)]
        [foreign (@xml:lang=lat-Latn)]
    [pb (@n)]
```

### Structure Example

```xml
<p xmlns="http://www.tei-c.org/ns/1.0" xml:id="p-1">
        <lb n="1"/>H(ec) [est] mentio de malefactoria q(ua)m rex donn(us) Sanci(us)fec(it) donno Laurëtio F(er)nandi (et)<note xml:id="p-1-note-1" xml:lang="por-Latn">Substitui o sinal tironiano / por (et) e transcrevi et, quando assim está expresso no texto.</note> p(re)cep(it) fac(er)e q(uo)d ei fecit
        <lb n="2"/>Velasc(us) Men(en)di. In p(ri)mis accepit ei LXX.a modios int(er) panë (et) uinũ et XXV int(er) archas (et)
        <lb n="3"/>cupas et X.a scutos et II.as(??) culcitres (et) II plumacios et int(er) scannos (et) lectos XI et calda-
        <lb n="4"/>rias (et) m(en)sas (et) scutellas (et) uasos multos (et) capellos de ferro (et) porcos decë (et) oues (et) capras
        <lb n="5"/>et XV m(o)r(a)b(itino)s, q(ui) leuauer(unt) de suis hominib(us) q(ui) spectauer(unt) et multa alia arma. Sup(er) hoc depo-
        <lb n="6"/>pulauer(unh) ei LXX.a casalia, unde est p(er)ditũ p(re)sentë fructũ q(uo)d in eis habebat (et) q(uo)d debet euenire.
        <lb n="7"/>(et) C homines d(e) maladia, q(ui) ita p(er)dider(unt). Deinde miser(unt) ignë in sua q(ui)ntana de Cuina (et) cre-
        <lb n="8"/>mauer(unt) eã totã q(uia) pre igne nichil ibi remansit. Et dir- ribauer(unt) de ipsa turre q(ua)ntã potuer(unt)
        <lb n="9"/>(et) q(uo)d n(on) potuer(unt) miser(unt) in eã ignë q(ui) eã findidit, q(uo)d nũq(ua)m potest e(ss)e em(en)data. Et etiã magis
        <lb n="10"/>custaret eã fac(er)e q(uo)d mille (et) D m(o)r(a)b(itino)s. (Et) q(ua)nta casalia habebat corã ipsa dicta q(ui)n-
        <lb n="11"/>tana cremauer(unt) ea. Sup(er) hoc acceper(unt) ei unũ sarracenũ bonũ.
  ...
```
