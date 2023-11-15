# Onderdelen van de ruimtelijke instrumenten {#647D7CD7}

Ieder ruimtelijk instrument is opgebouwd uit een samenhangende set onderdelen. Ieder onderdeel bestaat uit één of meerdere bronbestanden. In dit hoofdstuk worden eisen gesteld aan de mogelijke samenstelling van onderdelen en bronbestanden.

## Beschikbaar stellen van bronbestanden {#647D7CD9}

Ieder ruimtelijk instrument is opgebouwd uit een samenhangende set bronbestanden. Voor verschillende typen instrumenten is dit een andere set. Als er gebruik wordt gemaakt van objectgerichte planteksten ontstaat een andere set bronbestanden dan wanneer de teksten zonder gebruikmaking van objectgerichte planteksten beschikbaar worden gesteld. De vereiste bronbestanden per instrument zijn gegeven in <a href='#T001'>Tabel 1</a> en <a href='#T002'>Tabel 2</a>. Deze tabellen zijn limitatief. Een ruimtelijk instrument bestaat alleen uit de genoemde verplichte en optionele bronbestanden.

Burgemeester en wethouders, gedeputeerde staten en de verantwoordelijke minister of ministers (hierna aangeduid als bronhouder) stellen de geautoriseerde bronbestanden beschikbaar aan een ieder. Bij iedere beschikbaarstelling wordt gekozen uit één van de volgende twee opties:<br/>
Optie 1 : beschikbaar stellen <i>met</i> gebruikmaking van IMROPT2012, zie paragraaf <a href='#647D7CE0'>2.2</a>;<br/>
Optie 2 : beschikbaar stellen zonder gebruikmaking van IMROPT2012, zie paragraaf <a href='#647D7D0F'>2.3</a>.<br/>
## Beschikbaar stellen met gebruikmaking van objectgerichte planteksten {#647D7CE0}

In deze optie worden er objectgerichte planteksten beschikbaar gesteld conform het <a href='https://docs.geostandaarden.nl/ro/imropt' target='_blank'> Informatiemodel Ruimtelijke Ordening Planteksten (IMROPT2012)</a>. Dit betekent dat in ieder geval de regels, de toelichting en/of het beleids-/besluitdocument beschikbaar worden gesteld in XML formaat. Bijlagen kunnen ofwel in dit zelfde XML formaat beschikbaar worden gesteld, ofwel in separate bronbestanden. Bij gebruikmaking van objectgerichte planteksten is <a href='#T001'>Tabel 1</a> van toepassing.

<table style='width: 100%;' id='T001'><caption>Tabel 1 Bronbestanden indien er WEL gebruik wordt gemaakt van objectgerichte planteksten</caption>
<colgroup><col id='col1' style='width: 29.51312593963224%;'>
<col id='col2' style='width: 21.31375043367642%;'>
<col id='col3' style='width: 21.302185729154623%;'>
<col id='col4' style='width: 27.87093789753672%;'>
</colgroup>
<tbody valign='top'><tr><td align='left'>Onderdeel van het ruimtelijk instrument<br/>
</td>
<td align='left'>Naamconventie 
(excl. extensie)<br/>
</td>
<td align='left'>Bestandstype<br/>
</td>
<td align='center'>Multipliciteit<br/>
</td>
</tr>
<tr><td align='left'>IMRO<br/>
</td>
<td align='left'> [idn]<br/>
</td>
<td align='left'>GML<br/>
</td>
<td align='center'>1<br/>
</td>
</tr>
<tr><td align='left'>Planteksten<br/>
</td>
<td align='left'>pt_[idn]<br/>
</td>
<td align='left'>XML<br/>
</td>
<td align='center'>1<br/>
</td>
</tr>
<tr><td align='left'>Vaststellingsbesluit<br/>
</td>
<td align='left'>vb_[idn]<br/>
</td>
<td align='left'>HTML, XHTML of PDF<br/>
</td>
<td align='center'>0..1<br/>
</td>
</tr>
<tr><td align='left'>Bijlage<br/>
</td>
<td align='left'> b_[idn]_[xxx]<br/>
</td>
<td align='left'>HTML, XHTML of PDF<br/>
</td>
<td align='center'>0..*<br/>
</td>
</tr>
<tr><td align='left'>Illustratie<br/>
</td>
<td align='left'> i_[idn]_[xxx]<br/>
</td>
<td align='left'>JPEG, PNG of PDF<br/>
</td>
<td align='center'>0..*<br/>
</td>
</tr>
<tr><td align='left'>Geleideformulier<br/>
</td>
<td align='left'> g_[idn]<br/>
</td>
<td align='left'>XML<br/>
</td>
<td align='center'>1<br/>
</td>
</tr>
</tbody>
</table>

## Beschikbaar stellen zonder gebruikmaking van objectgerichte planteksten {#647D7D0F}

In deze optie worden de planteksten niet objectgericht beschikbaar gesteld. Er wordt derhalve geen gebruik gemaakt van IMROPT2012. Dit betekent dat de plan- of besluitregels beschikbaar worden gesteld in HTML of XHTML formaat en de toelichting en/of het beleids-/besluitdocument in HTML, XHTML of PDF formaat. In dit geval is <a href='#T002'>Tabel 2</a> van toepassing.

<table style='width: 100%;' id='T002'><caption>Tabel 2 Bronbestanden indien er GEEN gebruik wordt gemaakt van objectgerichte planteksten</caption>
<colgroup><col id='col1' style='width: 25.04623208506704%;'>
<col id='col2' style='width: 25%;'>
<col id='col3' style='width: 19.995376791493296%;'>
<col id='col4' style='width: 9.997688395746648%;'>
<col id='col5' style='width: 9.997688395746648%;'>
<col id='col6' style='width: 9.96301433194637%;'>
</colgroup>
<thead valign='top'><tr><th align='left' colspan='6'>Plan : bestemmingsplan, inpassingsplan, rijksbestemmingsplan, wijzigingsplan, uitwerkingsplan

Besluit : aanwijzingsbesluit, beheersverordening, amvb, ministeriële regeling, provinciale verordening, reactieve aanwijzing, voorbereidingsbesluit, omgevingsvergunning, exploitatieplan, gerechtelijke uitspraak

Visie : structuurvisie

</th>
</tr>
<tr><th align='left' rowspan='2'>Onderdeel van het ruimtelijk instrument<br/>
</th>
<th align='left' rowspan='2'>Naamconventie (excl. extensie)<br/>
</th>
<th align='left' rowspan='2'>Bestandstype<br/>
</th>
<th align='left' colspan='3'>Multipliciteit<br/>
</th>
</tr>
<tr><th align='left'>Plan<br/>
</th>
<th align='left'>Besluit<br/>
</th>
<th align='left'>Visie<br/>
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'>IMRO<br/>
</td>
<td align='left'> [idn]<br/>
</td>
<td align='left'>GML<br/>
</td>
<td align='center' colspan='3'>1<br/>
</td>
</tr>
<tr><td align='left'>Regels<br/>
</td>
<td align='left'> r_[idn]<br/>
</td>
<td align='left'>HTML of XHTML<br/>
</td>
<td align='center'>1<br/>
</td>
<td align='center'>0..1<br/>
</td>
<td align='center'>0<br/>
</td>
</tr>
<tr><td align='left'>Beleids-/Besluitdocument<br/>
</td>
<td align='left'> d_[idn]<br/>
</td>
<td align='left'>HTML, XHTML of PDF<br/>
</td>
<td align='center'>0<br/>
</td>
<td align='center'>0..1<br/>
</td>
<td align='center'>1<br/>
</td>
</tr>
<tr><td align='left'>Toelichting<br/>
</td>
<td align='left'> t_[idn]<br/>
</td>
<td align='left'>HTML, XHTML of PDF<br/>
</td>
<td align='center'>1<br/>
</td>
<td align='center'>0..1<br/>
</td>
<td align='center'>0..1<br/>
</td>
</tr>
<tr><td align='left'>Vaststellingsbesluit<br/>
</td>
<td align='left'>vb_[idn]<br/>
</td>
<td align='left'>HTML, XHTML of PDF<br/>
</td>
<td align='center' colspan='3'>0..1<br/>
</td>
</tr>
<tr><td align='left'>Bijlage<br/>
</td>
<td align='left'>b_[idn]_[xxx]<br/>
</td>
<td align='left'>HTML, XHTML of PDF<br/>
</td>
<td align='center' colspan='3'>0..*<br/>
</td>
</tr>
<tr><td align='left'>Illustratie<br/>
</td>
<td align='left'>i_[idn]_[xxx]<br/>
</td>
<td align='left'>JPEG, PNG of PDF<br/>
</td>
<td align='center' colspan='3'>0..*<br/>
</td>
</tr>
<tr><td align='left'>Geleideformulier<br/>
</td>
<td align='left'>g_[idn]<br/>
</td>
<td align='left'>XML<br/>
</td>
<td align='center' colspan='3'>1<br/>
</td>
</tr>
</tbody>
</table>

Verklaring bij <a href='#T001'>Tabel 1</a> en <a href='#T002'>Tabel 2</a>:

<div style='display: flex; flex-direction: column;'>
<div style='display: flex; flex-direction: row'>
<div style='flex: 0 1 20%'><i>Bestandstype</i></div>
<div style='flex: 0 1 80%'>bestandstype van het onderdeel; voor exacte bestandsformaten zie paragraaf <a href='#4036FA61'>4.2</a>;</div>
</div>
<div style='display: flex; flex-direction: row'>
<div style='flex: 0 1 20%'><i>[idn]</i></div>
<div style='flex: 0 1 80%'>identificatienummer van het ruimtelijk instrument, zie paragraaf <a href='#647D7DA3'>4.1</a>;</div>
</div>
<div style='display: flex; flex-direction: row'>
<div style='flex: 0 1 20%'><i>[xxx]</i></div>
<div style='flex: 0 1 80%'>tekstuele extensie als onderdeel van de bestandsnaam, zie paragraaf <a href='#4036FA61'>4.2</a>;</div>
</div>
<div style='display: flex; flex-direction: row'>
<div style='flex: 0 1 20%'><i>Multipliciteit</i></div>
<div style='flex: 0 1 10%'>1</div>
<div style='flex: 0 1 70%'>het onderdeel komt altijd precies 1 keer voor en is daarmee dus verplicht;</div>
</div>
<div style='display: flex; flex-direction: row'>
<div style='flex: 0 1 20%'></div>
<div style='flex: 0 1 10%'>0..1</div>
<div style='flex: 0 1 70%'>het onderdeel komt 0 of 1 keer voor en is dus optioneel;</div>
</div>
<div style='display: flex; flex-direction: row'>
<div style='flex: 0 1 20%'></div>
<div style='flex: 0 1 10%'>0..*</div>
<div style='flex: 0 1 70%'>het onderdeel komt 0 of meer keer voor en is dus optioneel.</div>
</div>
</div>

De in <a href='#T001'>Tabel 1</a> en <a href='#T002'>Tabel 2</a> gespecificeerde optionele onderdelen kunnen onder voorwaarde verplicht zijn. In het <a href='https://docs.geostandaarden.nl/ro/imro' target='_blank'> Informatiemodel Ruimtelijke Ordening Planteksten (IMRO2012)</a> wordt nader aangegeven wanneer dit het geval is.<br/>
