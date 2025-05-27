# Dataset 'apcor-6'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm?apcor006.htmapcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-6/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-6/, visited on <insert date>)
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
```

### Structure Example

```xml
<p xmlns="http://www.tei-c.org/ns/1.0" xml:id="p-1">
        <lb n="1)"/>En'o nome de Deus. Eu rei don Afonso pela gracia de Deus rei de Portugal, seendo sano e saluo, tem(en)te o dia de mia morte a saude de mia alma e a proe de mia molier reina dona Vrr(aca) e de meus filios e de meus uassalos
        <lb n="2"/>e de todo meu reino fiz mia mãda p(er) q(ue) de- pois mia morte mia molier e meus filios e meus uassalos e meu reino e todas aq(ue)las cousas q(ue) Deus mi deu en poder sten en paz e en folgãcia. P(ri)meiram(en)te mã\do
        <lb n="3"/>q(ue) meu filio ifan[te]  don Sãcio q(ue) ei da reina dona Vrr(aca) aia meu reino enteiram(en)te e en paz. E sse este for morto sen semel, o maior filio q(ue) ouuer da reina dona Vrr(aca) aia o reino enteg(ra)mëte e en paz.
        <lb n="4"/>E sse filio baron nũ ouu(er)m(os), a maior filia q(ue) ouu(er)m(os) aia'o. E sse no tëpo d(e) mia morte meu filio ou mia filia q(ue) deuier a reinar nũ ouuer reuora, seia en poder da reina sua madre e meu reino
        <lb n="5"/>seia en poder da reina e de meus uassalos ata cãdo aia reuora. E sse eu for morto, rogo o ap(osto)ligo como padre e senior e beio a t(er)ra an(te) seus pees q(ue) el receba en sa com(en)da e so seu defendim(en)to a reina
        <lb n="6"/>e meus filios e o reino. E sse eu e [a]  reina formos mortos, rogoli e p(re)goli q(ue) os meus filios e o reino seiam en sa com(en)da. E mãdo da dezima dos morauidiis e dos dineiros q(ue) mi remas(er)um da parte de
        <lb n="7"/>meu padre q(ue) sũ en Alcobacia e do outr'auer mouil q(ue) i pos(er)m(os) pora esta d(e)zima q(ue) seia partido pelas manos do arcebispo d(e) Bragaa e do de Santiago e do bispo do Porto e de Lisbona e de Coinbra e de
        <lb n="8"/>Uiseu e de Lamego e da Idania e d'Euora e de Tui e do tesoureiro de Bragaa. Out(ri)ssi mando das d(e)zimas das luitosas e das armas e doutras dezimas q(ue) eu tenio apartadas en te- souros per meu rei\no
        <lb n="9"/>q(ue) eles as departan assi<note xml:id="p-1-note-1" xml:lang="por-Latn">Parece mais <foreign xml:lang="und-Latn-x-glpt">al si</foreign> do que <foreign xml:lang="und-Latn-x-glpt">assi.</foreign>
        </note> como uiren por guisado. E mãdo q(ue) o abade d'Alcobacia lis de aq(ue)sta d(e)zima q(ue) el ten ou teiu(er) e eles as departan segũdo Deus como uiren por dereito. E mãdo
<lb n="10"/>q(ue) a reina dona Vrr(aca) aia a meia- dade de todas aq(ue)las cousas mouils q(ue) eu ouu(er) a mia morte, exetes estas d(e)zimas q(ue) mãdo dar por mia alma e as outras q(ue) tenio en uoontade por dar por mia alma
  ...
```
