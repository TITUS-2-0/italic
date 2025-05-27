# Dataset 'apcor-5'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm?apcor005.htmapcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-5/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-5/, visited on <insert date>)
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
text (@xml:lang=und-Latn-x-glpt)
  body
    p (@xml:id)
      [lb (@n) (multiple)]
      [note (@xml:id, @xml:lang=por-Latn) (multiple)]
        [foreign (@xml:lang=und-Latn-x-glpt) (multiple)]
      [foreign (@xml:lang=lat-Latn)]
        [foreign (@xml:lang=lat-Latn) (multiple)]
    [pb (@n)]
```

### Structure Example

```xml
<p xmlns="http://www.tei-c.org/ns/1.0" xml:id="p-1">
        <lb n="1"/>En'o<note xml:id="p-1-note-1" xml:lang="por-Latn">Só resta a parte inferior do <foreign xml:lang="und-Latn-x-glpt">E.</foreign>
        </note> nome de Deus. Eu rei don Afonso pela gracia de Deus rei de Portugal, seendo sano e saluo, temëte o dia de mia morte, a saude de mia alma e a proe de mia molier raina dona Orraca e de me(us) filios e de me(us) uassalos e de todo meu reino fiz mia mãda p(er) q(ue) de-
<lb n="2"/>pos mia morte mia molier e me(us) filios e meu reino e me(us) uassalos e todas aq(ue)las cousas q(ue) De(us) mi deu en poder sten en paz e en folgãcia. P(ri)meiram(en)te mãdo q(ue) meu filio infante don Sancho q(ue) ei da raina dona Orraca agia meu reino enteg(ra)- m(en)te e en paz. E ssi este for
<lb n="3"/>morto sen semmel, o maior filio q(ue) ouuer da raina dona Orraca agia o reino entegram(en)te e en paz. E ssi filio barõ nõ ouuer- mos, a maior filia q(ue) ouuermos agia'o. E ssi no tëpo de mia morte meu filio ou mia filia q(ue) deuier a reinar nõ ouuer reuora, segia en poder
<lb n="4"/>da raina sa madre e meu reino segia en poder da raina e de me(us) uassalos ata q(uan)do agia reuora. E ssi eu for morto, rogoo apostoligo<note xml:id="p-1-note-2" xml:lang="por-Latn">O papa.</note> come padre e senior e beigio a t(er)ra ante seus pees q(ue) el recebia en sa comëda e so seu difindemëto a raina e me(us) filios e o reino. E ssi eu
<lb n="5"/>e a raina formos mortos, rogoli e pregoli q(ue) os me(us) filios e o reino segiã en sa comëda. E mãdo da dezima dos morauidiis e dos dieiros q(ue) mi remaserũ de parte de meu padre q(ue) sũ en Alcobaza e do outr'auer mouil q(ue) i posermos pora esta dezima q(ue) segia partido pelas manus
<lb n="6"/>do arcebispo de Bragaa e do arcebispo de Santiago e do bispo do Portu e de Lixbona e de Coibria e de Uiseu e de Lamego e da Idania e d'Euora e de Tui e do tesoureiro de Bragaa. E out(ro)ssi mãdo das dezimas das luctosas e das armas e dout(ra)s dezimas q(ue) eu tenio apartadas en te-
<lb n="7"/>souros per meu reino, q(ue) eles as departiã assi como uirë por derecto. E mãdo q(ue) o abade d'Alcobaza lis de aq(ue)sta dezima q(ue) el ten ou teiuer e eles as departiã segũdo De(us) como uirë por derecto. E mãdo q(ue) a raina dona Orraca agia a meiadade de todas aq(ue)lias cousas mouils q(ue) eu ouuer
<lb n="8"/>a mia morte, exetes aq(ue)stas dezimas q(ue) mãdo dar por mia alma e as out(ra)s q(ue) tenio en uoontade por dar por mia alma e non'as uiier a dar. Et mãdo q(ue) si a raina morrer en mia uida q(ue) de todo meu auer mouil agia ende a meiadade. Da out(ra) meiadade solten ende p(ri)meiram(en)te
<lb n="9"/>todas mias devidas e do q(ue) remaser fazam en[de]  t(re)s partes e as duas partes agiã me(us) filios e mias filias e departiãse ent(r'e)les igualm(en)te. Da t(er)ceira o arcebispo de Bragaa e o arce- bispo de Santiago e o bispo do Portu e o de Lixbona e o de Coibria e o de Uiseu e o d'Euora fazã desta
<lb n="10"/>guisa: q(ue) u q(ue)r q(ue) eu moira q(ue)r en meu reino q(ue)r fora de meu regno fazam aduzer meu corpo p(er) mias custasa Alcobaza. E mãdo q(ue) den a meu senior o papa III m(o)r(auidiis)<note xml:id="p-1-note-3" xml:lang="por-Latn">Desdobrei a abreviatura mr. em <foreign xml:lang="und-Latn-x-glpt">morauidiis</foreign> e não em <foreign xml:lang="und-Latn-x-glpt">morabitnos,</foreign> por ser a primeira forma a que vem por extenso em A e em A', respectivamente, nas linhas 5 e 6. Nos casos seguintes mantive a abreviatura, por o desdobramento ser o mesmo.</note> a Alcobaza II mr. por meu añiu(er)sario, a Santa Maria de Rocamador II mr. por meu añiu(er)sario
  ...
```
