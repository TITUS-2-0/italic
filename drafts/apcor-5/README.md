# Dataset 'apcor-5'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-5/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-5/, visited on <insert date>)
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
      [foreign (@xml:lang=lat-Latn)]
        [foreign (@xml:lang=lat-Latn) (multiple)]
    [pb (@n)]
```

### Structure Example

```xml
<p xmlns="http://www.tei-c.org/ns/1.0" xml:id="p-1">
        <lb n="1"/>En'o
        <note xml:id="p-1-note-1" xml:lang="por-Latn">
          Só resta a parte inferior do
          <foreign xml:lang="und-Latn-x-glpt">E.</foreign>
        </note>
        nome de Deus. Eu rei don Afonso pela gracia de Deus rei de Portugal, seendo sano e saluo, temëte o dia de mia morte, a saude de mia alma e a proe de mia molier raina dona Orraca e de me(us) filios e de me(us) uassalos e de todo meu reino fiz mia mãda p(er) q(ue) de-
        <lb n="2"/>pos mia morte mia molier e me(us) filios e meu reino e me(us) uassalos e todas aq(ue)las cousas q(ue) De(us) mi deu en poder sten en paz e en folgãcia. P(ri)meiram(en)te mãdo q(ue) meu filio infante don Sancho q(ue) ei da raina dona Orraca agia meu reino enteg(ra)- m(en)te e en paz. E ssi este for
        <lb n="3"/>morto sen semmel, o maior filio q(ue) ouuer da raina dona Orraca agia o reino entegram(en)te e en paz. E ssi filio barõ nõ ouuer- mos, a maior filia q(ue) ouuermos agia'o. E ssi no tëpo de mia morte meu filio ou mia filia q(ue) deuier a reinar nõ ouuer reuora, segia en poder
        <lb n="4"/>da raina sa madre e meu reino segia en poder da raina e de me(us) uassalos ata q(uan)do agia reuora. E ssi eu for morto, rogoo apostoligo
        <note xml:id="p-1-note-2" xml:lang="por-Latn">O papa.</note>
        come padre e senior e beigio a t(er)ra ante seus pees q(ue) el recebia en sa comëda e so seu difindemëto a raina e me(us) filios e o reino. E ssi eu
  ...
```
