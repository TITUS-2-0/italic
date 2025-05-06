# Dataset 'apcor-4'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ital/aport/apcorp/apcor.htm).

* URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-4/
* version: unreleased
* date: 2025-05-01

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/italic/tree/main/drafts/apcor-4/, visited on <insert date>)
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
    div (@data-level=1, @n, @type=item, @xml:id) (multiple)
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [note (@xml:id, @xml:lang=por-Latn) (multiple)]
          [foreign (@xml:lang=und-Latn-x-glpt) (multiple)]
        [note (@xml:id)]
          [foreign (@xml:lang=por-Latn)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="r." xml:id="item-1" type="item" data-level="1">
				<p xml:id="item-1-p-1">
					<lb n="1"/>D(e) noticia d(e) torto que fecer(um) a Laurëci(us) Fernãdiz por plazo que fec(e) Gõcauo<lb n="2"/>Ramiriz antre suos <note xml:id="item-1-p-1-note-1" xml:lang="por-Latn">Nesta palavra e em várias outras o <foreign xml:lang="und-Latn-x-glpt">s</foreign> final vem na entrelinha ou em expoente, assemelhando-se ao sinal abreviativo de <foreign xml:lang="und-Latn-x-glpt">er.</foreign>
					</note> filios e Lourëço Ferrnãdiz q(ua)le podedes saber e oue au(e)r <note xml:id="item-1-p-1-note-2" xml:lang="por-Latn">Na palavra <foreign xml:lang="und-Latn-x-glpt">au(e)r</foreign> ('=' haver) e em outras usa um sinal abreviativo parecido com um til em posição quase vertical, podendo indicar a falta de <foreign xml:lang="und-Latn-x-glpt">e</foreign> ou de outras letras e até silabas.</note> d(e) erdad(e)<lb n="3"/>e d'au(e)r tãto q(uo)me uno d(e) suos filios d(e) aq(uan)to podesë au(e)r d(e) bona d(e) seuo pater e fiolios seu<lb n="4"/>pater e sua mater. E d(e)pois fecer(um) plazo nouo e cõuë uos a saber q(ua)le in ille se&lt;e&gt;m<lb n="5"/>taes firmam(en)tos q(ua)les podedes saber <note xml:id="item-1-p-1-note-3" xml:lang="por-Latn">Segue-se uma palavra rasurada.</note> Ramiro Gõcaluiz e Gõcaluo Gõca[luiz]<lb n="6"/>Eluira Gõcaluiz forũ fiadores d(e) sua irmana que orgase aqu[e]le plazo come illos.<lb n="7"/>Sup(er) isto plazo ar fe(ce)r(um) suo plecto. E a maior aiuda que illos hic cõnocer(um) que les<lb n="8"/>acanocese Laurëzo Ferrnãdiz sa irdad(e) p(er) p(lec)to <note xml:id="item-1-p-1-note-4" xml:lang="por-Latn">Em rigor, a abreviatura desta palavra devia desdobrar-se em <foreign xml:lang="und-Latn-x-glpt">p(re)to,</foreign> mas prefiro <foreign xml:lang="und-Latn-x-glpt">p(lec)to,</foreign> porque é este o sentido e é assim que vem, por extenso, na linha 7.</note> que a teuese o abate d(e) S(an)c(t)o Martino<lb n="9"/>que como uëcesë <note xml:id="item-1-p-1-note-5" xml:lang="por-Latn">Seguem-se, raspadas, umas letras que parecem ser <foreign xml:lang="und-Latn-x-glpt">oct(ra)a.</foreign>
					</note> que asi les dese d(e) ista o abade. E que nunq(ua) illos lecxasë<lb n="10"/>daquela irdad(e) <note xml:id="item-1-p-1-note-6" xml:lang="por-Latn">No texto parece antes <foreign xml:lang="und-Latn-x-glpt">iertad(e) d(e).</foreign>
					</note> së seu mãdato. Se a lexarë itregarë ille d(e) oct(ra) que &lt;li&gt; plaza.<lb n="11"/>E d'au(e)r que ouer(um) d(e) seu pat(e)r nu[n]q(uam) <note xml:id="item-1-p-1-note-7" xml:lang="por-Latn">Neste caso e em outros idênticos, desdobrei a abreviatura em <foreign xml:lang="und-Latn-x-glpt">nunq(uam),</foreign> porque a haste do <foreign xml:lang="und-Latn-x-glpt">q</foreign> está cortada por um traço transversal a indicar falta de <foreign xml:lang="und-Latn-x-glpt">m</foreign> , neste termo, ou de <foreign xml:lang="und-Latn-x-glpt">n,</foreign> em <foreign xml:lang="und-Latn-x-glpt">q(uan)to.</foreign> Faltando o traço, desdobrei em <foreign xml:lang="und-Latn-x-glpt">numq(ua).</foreign>
					</note> se li id(e) der(um) parte. Deu <note xml:id="item-1-p-1-note-8" xml:lang="por-Latn">Seguem-se <foreign xml:lang="und-Latn-x-glpt">a Laurë</foreign> traçadas e um espaço em branco.</note> do Gõçauũ<lb n="12"/>o a Laurëco Fernãdiz e Marti Gõc[a]luiz  XII <note xml:id="item-1-p-1-note-9" xml:lang="por-Latn">Segue-se um <foreign xml:lang="und-Latn-x-glpt">a</foreign> traçado.</note> casaes por arras d(e) sua auóó.<lb n="13"/>E filar(um)li illos ind(e) VI casales <note xml:id="item-1-p-1-note-10" xml:lang="por-Latn">Seguem-se <foreign xml:lang="und-Latn-x-glpt">quanto er</foreign> traçadas.</note> c(um) torto. E podedes saber como man-<lb n="14"/>do dũ Gõcauo a sua morte. D(e) XVI casales d(c) Ueracin que &lt;d(e)&gt; fructar(um) e que li<lb n="15"/>nunq(uam) id(e) der[um]  q(ui)nnõ. E d(e) VII e medio casaes antre Coina e Bastuzio und(e) li<lb n="16"/>nunq(uam) der(um) q(ui)niõ. E d(e) tres i(n) Tesuosa und(e) li nu[n]q(ua)  ar der(um) nada. E IIos, i(n) Figeeree-<lb n="17"/>do unnd(e) nunq(uam) <note xml:id="item-1-p-1-note-11" xml:lang="por-Latn">No texto está: <foreign xml:lang="und-Latn-x-glpt">nu nada q(uam),</foreign> mas com a palavra <foreign xml:lang="und-Latn-x-glpt">nada</foreign> traçada.</note> li der(um) q(ui)nõ. E IIos i(n) Tamal ũd(e) li n(om) ar der(um) q(ui)nõ. E da sena-<lb n="18"/>ra d(e) Coina ũd(e) li n(om) ar der(um) q(ui)nõ. E d'uno casal d(e) Coina que leuar(um) id(e) III anos<lb n="19"/>o frouctu c(um) torto. E por istes tortos que li fecer(um) tem q(ua) a seu plazo quebrãtado<lb n="20"/>e q(ua) li o deuë por sanar. E d(e)pois ouer(um) seu mal e meteu o abad(e) paz a[n]tre  illes<lb n="21"/>i(n) no Carualio d(e) Laureedo. E rogou o abate tãto que beiso c(um) illes. E der(um)li<lb n="22"/>XVIIII morabitinos q(ui) li filar(um). E d(e)pos iste p(lec)to <note xml:id="item-1-p-1-note-12" xml:lang="por-Latn">siehe Nr. 3</note> pre[n]d(e)r(um)li <note xml:id="item-1-p-1-note-13" xml:lang="por-Latn">Segue-se <foreign xml:lang="und-Latn-x-glpt">on</foreign> traçado.</note> o seruical otro<lb n="23"/>om[ee]  d(e) sa casa e troser(um)no XVIIII dias p(er) mõtes e fecer(um)les tã máá prisõ<lb n="24"/>p(er) que leuar(um) deles q(uan)to poder(um) au(e)r. E d(e)pois li d(e)sũro Gõcauo Gõcauiz<lb n="25"/>sa fili[a] pechena <note xml:id="item-1-p-1-note-14">
						<foreign xml:lang="por-Latn">Por pequena.</foreign>
					</note> E irmar[um]li  XIII casales und(e) perdeu fructu. E isto<lb n="26"/>fui d(e)p&lt;ois&gt; que fur(um) fíídos ant'o abate. E d(e)pois que fur(um) ifiados por iuizo d(e) ilo<lb n="27"/>rec. <note xml:id="item-1-p-1-note-15" xml:lang="por-Latn">Por <foreign xml:lang="und-Latn-x-glpt">rex</foreign> (rei).</note> E nũq(ua) ille fez(e) neun mal por todo aqueste e fezeles taes agudas <note xml:id="item-1-p-1-note-16" xml:lang="por-Latn">Neste e cm casos idênticos, o <foreign xml:lang="und-Latn-x-glpt">g</foreign> tem valor fricative antes de <foreign xml:lang="und-Latn-x-glpt">a</foreign> , alternando, por isso, com <foreign xml:lang="und-Latn-x-glpt">i</foreign> consoante: <foreign xml:lang="und-Latn-x-glpt">aguda</foreign> e <foreign xml:lang="und-Latn-x-glpt">aiuda</foreign> (=ajuda).</note>
					<lb n="28"/>q(ua)les aqui ouireedes. Sup(er) sua aguda fez testiuigo c(um) Gõcauo Cebolano.<lb n="29"/>E sup(er) sa aiuda ar fuili a casa e filoli q(uan)to que li agou e deu a illes. E sup(er) sa<lb n="30"/>aiuda oue testifigo c(um) P(e)tro Gomez omezio q&lt;v&gt;e li custou maes ka C m(orabitinos).<lb n="31"/>E sup(er) sa aiud[a]  oue mal c(um) Goncaluo Gomez que li custou multo da au(e)r<lb n="32"/>e muita perda. E in <note xml:id="item-1-p-1-note-17" xml:lang="por-Latn">P Aqui e nos três casos análogos seguintes, em vez de <foreign xml:lang="und-Latn-x-glpt">E in,</foreign> poder-se-ia ler <foreign xml:lang="und-Latn-x-glpt">Emi.</foreign>
					</note> sa aiuda oue mal c(um) Go[n]caluo Suariz. E in sa aiuda<lb n="33"/>oue mal c(um) Ramiro Fernãdiz que li custov muito au(e)r muita perda.<lb n="34"/>E in sa aiuda fui IIas fezes a Coi[n]bra.  E in sa aiuda dixe mul[ta]s  uices<lb n="35"/>e ora in ista tregua fur(um) a Ueraci amazar(um)li os om(éé)s erma[rum]li  X casaes<lb n="36"/>seu torto al rec. <note xml:id="item-1-p-1-note-18" xml:lang="por-Latn">siehe Nr. 14</note> E sup(er) s'aiud[a]  mãdoe lidar seus om(éé)s c[um]  Mar-<lb n="37"/>tin <note xml:id="item-1-p-1-note-19" xml:lang="por-Latn">No texto: <foreign xml:lang="und-Latn-x-glpt">Marmtin.</foreign>
					</note> I(o)h(an)n(i)s que q(ui)ra <note xml:id="item-1-p-1-note-20" xml:lang="por-Latn">Por <foreign xml:lang="und-Latn-x-glpt">queria.</foreign>
  ...
```
