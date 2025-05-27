# Dataset '1192 MARÇO -- Auto de partilhas entre Rodrigo Sanches e seus irmãos Vasco, Mendo e Elvira.'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm?apcor001.htmapcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-1/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of 1192 MARÇO -- Auto de partilhas entre Rodrigo Sanches e seus irmãos Vasco, Mendo e Elvira. (draft version). By: Gisella Ferraresi, Jost Gippert, Maria Goldbach, Florian Matter, Esther Rinke. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-1/, visited on <insert date>)
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
| Text (hierarchical) | `div@text (hierarchical)` | Automatically translated into named div |
| Part (linear) | `milestone@part (linear)` |  |
| Item (hierarchical) | `pb (linear)` |  |
| Line (hierarchical) | `lb (linear)` |  |

### Structural overview
```text
text (@xml:lang=und-Latn-x-glpt)
  body
    p (@xml:id)
      [lb (@n) (multiple)]
      [note (@xml:id, @xml:lang=por-Latn) (multiple)]
        [foreign (@xml:lang=und-Latn-x-glpt) (multiple)]
      [foreign (@xml:lang=lat-Latn) (multiple)]
        [foreign (@xml:lang=lat-Latn) (multiple)]
      [lb (@n, @xml:lang=lat-Latn) (multiple)]
    [pb (@n)]
```

### Structure Example

```xml
<p xmlns="http://www.tei-c.org/ns/1.0" xml:id="p-1">
        <lb n="1"/>In Ch(risti) n(omi)ne, am(en). Hec e(st) notitia de p(ar)tiçon(e)<note xml:id="p-1-note-1" xml:lang="por-Latn">Substituí o sinal tironiano 7 por (e), porque o texto traz a copulative <foreign xml:lang="und-Latn-x-glpt">e</foreign> nos outros casos.</note> de deuison que fazem(os)<note xml:id="p-1-note-2" xml:lang="por-Latn">Il Como o escriba usou quási indistintamente <foreign xml:lang="und-Latn-x-glpt">os e us: dos e dus</foreign> (linha 1), <foreign xml:lang="und-Latn-x-glpt">herdamentos</foreign> (linhas 5 e 9) e <foreign xml:lang="und-Latn-x-glpt">herdamentus</foreign> (linhas 1, 4 e 7), preferi desdobrar em <foreign xml:lang="und-Latn-x-glpt">os</foreign> o sinal tironiano de <foreign xml:lang="und-Latn-x-glpt">us</foreign> e <foreign xml:lang="und-Latn-x-glpt">os</foreign> , por esta última forma ser a usada no português.</note> antre nos des (her)dam(en)tus e dus cou[tos e]<note xml:id="p-1-note-3" xml:lang="por-Latn">Uma mancha no pergaminho torna ilegíveis as últimas quatro letras.</note> das onrras
        <lb n="2"/>e dou&lt;s&gt; padruadig(os) das eygreygas que forum de nossu padre e de nossa madre, en esta maneira q(ue) Rodrigo
        <lb n="3"/>Sanchiz ficar por sa p(ar)ticon na q(ui)nta do couto de Víítu- rio e na q(ui)nta do padroadigo dessa eygreyga en todol(os)
        <lb n="4"/>us h(er)dam(en)tus do couto e de fora do couto. Vu(a)sco Sanchiz ficar por sa p(ar)ticon na onrra d'Ulueira e no padroa-
        <lb n="5"/>digo dessa eygreyga en todol(os) h(er)dam(en)tos d'Olveira e en nu casal de Carapezus q(ue) chamam da Vluar e en outro
        <lb n="6"/>casal en Agiar que chamam Q(ui)ntáá. Meen Sanchiz ficar por sa p(ar)ticon na onrra de Carapezus e nus outr(os)
        <lb n="7"/>h(er)dam(en)tus e nas duas p(ar)tes do padroadigo dessa eygreyga e no padroadigo da eygreyga de Creysemil e
        <lb n="8"/>na onrra e no h(er)dam(en)to d'Arguiffi e no h(er)dam(en)to de Lauoradas e no padroadigo dessa eygreyga. Eluira
        <lb n="9"/>Sanchiz ficar por sa p(ar)ticon nos h(er)dam(en)tos de Cente- gaus e nas tres q(ua)rtas do padroadigo dessa eygreyga
        <lb n="10"/>e no h(er)dam(en)to de Creyximil assi us das Sestas come u outro h(er)dam(en)to. Estas p(ar)ticoens e diuisoes fazem(os) an-
        <lb n="11"/>tre nos q(ue) uallam por en s(e)c(u)la s(e)c(u)lor(um), am(en). <foreign xml:lang="lat-Latn">Facta karta m(en)sse M(a)rcíí E(ra) M. <foreign xml:lang="lat-Latn">a</foreign> CC. <foreign xml:lang="lat-Latn">a</foreign> XXX. <foreign xml:lang="lat-Latn">a</foreign> . Vaa&lt;s&gt;co</foreign>
  ...
```
