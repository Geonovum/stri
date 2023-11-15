# Bestandstype {#647D7D66}

In dit hoofdstuk is aangegeven welke bestandstypen moeten worden gehanteerd. Tevens worden er in dit hoofdstuk nadere regels gesteld aan het gebruik van HTML en XHTML.

## Bestandsextensies en toegestane formaten {#647D7D68}

Voor ieder onderdeel worden in <a href='#T001'>Tabel 1</a> en <a href='#T002'>Tabel 2</a> eisen gesteld aan de mogelijke bestandstypen. De bestandstypes met toegestane extensies en MIME types worden gegeven in <a href='#T003'>Tabel 3</a>.<br/>
<table style='width: 100%;' id='T003'><caption>Tabel 3 Toegestane extensies en MIME types</caption>
<colgroup><col id='col1' style='width: 24.075358298659268%;'>
<col id='col2' style='width: 33.33333333333333%;'>
<col id='col3' style='width: 42.5913083680074%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Bestandstype<br/>
</th>
<th align='left'>Extensie<br/>
</th>
<th align='left'>MIME type<br/>
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'>XML<br/>
</td>
<td align='left'>.xml<br/>
</td>
<td align='left'>text/xml<br/>
</td>
</tr>
<tr><td align='left'>GML<br/>
</td>
<td align='left'>.gml<br/>
</td>
<td align='left'>text/xml<br/>
</td>
</tr>
<tr><td align='left'>HTML<br/>
</td>
<td align='left'>.htm, .html<br/>
</td>
<td align='left'>text/html<br/>
</td>
</tr>
<tr><td align='left'>XHTML<br/>
</td>
<td align='left'>.htm, .html, .xhtml<br/>
</td>
<td align='left'>application/xhtml+xml<br/>
</td>
</tr>
<tr><td align='left'>PDF<br/>
</td>
<td align='left'>.pdf<br/>
</td>
<td align='left'>application/pdf<br/>
</td>
</tr>
<tr><td align='left'>JPEG<br/>
</td>
<td align='left'>.jpeg, .jpg<br/>
</td>
<td align='left'>image/jpeg<br/>
</td>
</tr>
<tr><td align='left'>PNG<br/>
</td>
<td align='left'>.png<br/>
</td>
<td align='left'>image/png <br/>
</td>
</tr>
</tbody>
</table>

Ten gevolge van extern beleid zijn er voor ieder van de in <a href='#T003'>Tabel 3</a> genoemde bestandstypes veelal aanvullende specificaties van toepassing met betrekking tot de exact toegestane bestandsformaten. De specificaties zijn niet opgenomen in deze standaard, omdat deze aan wijzigingen onderhevig zijn die een andere dynamiek kunnen hebben dan de voorliggende standaard.<br/>
## Gebruik van HTML en XHTML {#647D7D97}

Een aantal onderdelen van de verschillende ruimtelijke instrumenten kan beschikbaar gesteld worden in HTML of XHTML formaat. Bij het gebruik van deze formaten is een aantal aanvullende regels van kracht:

<ol><li>het invoegen van de illustraties die onderdeel uitmaken van het ruimtelijk instrument is toegestaan. De URL van de illustratie die in het src attribuut van het &lt;img&gt; element wordt gespecificeerd is een relatieve URL zonder directory elementen. Dit is mogelijk omdat alle bestanden in één virtuele directory beschikbaar worden gesteld. Door het specificeren van een relatieve URL voor de &lt;img&gt; elementen blijft het ruimtelijk instrument bruikbaar indien het in zijn geheel in een andere raadpleegomgeving wordt getoond;</li>
<li>het invoegen van illustraties die geen onderdeel uitmaken van het ruimtelijk instrument is niet toegestaan;</li>
<li>gebruik van separate <a href='https://www.w3.org/Style/CSS/' target='_blank'>Cascading Style Sheets (CSS bestanden)</a> voor de opmaak van HTML en XHTML bestanden is toegestaan. CSS bestanden maken geen onderdeel uit van het ruimtelijk instrument, maar referenties naar CSS bestanden die bij het tonen van het instrument beoogd zijn door de bronhouder kunnen zowel in &lt;link&gt; elementen alsook in het geleideformulier worden opgenomen (zie Hoofdstuk <a href='#647D7DE7'>5</a>). Omdat CSS bestanden geen formeel onderdeel zijn van het instrument, zijn URL's naar CSS bestanden op andere virtuele directories dan de formele onderdelen toegestaan;</li>
<li>de HTML en XHTML bestanden worden raadpleegbaar op overheidswebsites. Daarom zijn de opmaak en technische randvoorwaarden van deze bestanden veelal gebaseerd op internationaal erkende richtlijnen van het World Wide Web Consortium (W3C) en de <a href='https://www.digitaleoverheid.nl/overzicht-van-alle-onderwerpen/digitale-inclusie/digitaal-toegankelijk/' target='_blank'>richtlijnen van digitale toegankelijkheid</a>.</li>
<li>HTML en XHTML pagina's dienen bruikbaar te blijven wanneer CSS door een webbrowser niet ondersteund wordt. Dit betekent dat er in de pagina geen inhoud verloren mag gaan als de CSS niet wordt toegepast op de pagina.</li>
</ol>

