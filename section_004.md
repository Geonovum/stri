# Identificatienummer en bestandsnaam {#647D7DA1}

Ieder ruimtelijk instrument kent een eigen identificatienummer (idn). In dit hoofdstuk is aangegeven hoe de opbouw van dit idn is. Tevens zijn in dit hoofdstuk de eisen voor de bestandsnamen van de bronbestanden vastgelegd, waarvan het idn een belangrijke basis is.

## Identificatienummer {#647D7DA3}

Ieder ruimtelijk instrument kent een eigen identificatienummer (idn). Het idn is beschreven door middel van een reguliere expressie, als volgt:

NL\.(IMRO\.[0-9]{4}\.[A-Za-z0-9]{1,18}-[A-Za-z0-9]{4}

In <a href='#T004'>Tabel 4</a> worden de onderdelen van deze reguliere expressie nader verklaard.<br/>
<table style='width: 100%;' id='T004'><caption>Tabel 4 Onderdelen van het identificatienummer</caption>
<colgroup><col id='col1' style='width: 22.58504949368529%;'>
<col id='col2' style='width: 77.41495050631471%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Onderdeel reg. exp.<br/>
</th>
<th align='left'>Betekenis <br/>
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'>NL\.(IMRO)\.<br/>
</td>
<td align='left'>de namespace NL.IMRO. als vaste tekst.<br/>
</td>
</tr>
<tr><td align='left'>[0-9]{4}<br/>
</td>
<td align='left'>CBS code van de verantwoordelijke overheid. Altijd 4 cijfers, indien nodig aangevuld met voorloopnullen. Ingeval Rijk “0000”. De CBS-code van de provincie wordt voorafgegaan door 2 voorloopnegens. Ingeval deelgemeente/stadsdeel: CBS-code gemeente.<br/>
</td>
</tr>
<tr><td align='left'>\.<br/>
</td>
<td align='left'>Een punt .<br/>
</td>
</tr>
<tr><td align='left'>[A-Za-z0-9]{1,18}<br/>
</td>
<td align='left'>Minimaal 1 en maximaal 18 alfanumerieke tekens, te bepalen door de bronhouder.<br/>
</td>
</tr>
<tr><td align='left'>- <br/>
</td>
<td align='left'>Een liggend streepje -<br/>
</td>
</tr>
<tr><td align='left'>[A-Za-z0-9]{4}<br/>
</td>
<td align='left'>Vier alfanumerieke karakters voor de door de bronhouder te bepalen versiecode van het instrument binnen het desbetreffende dossier. De versiecode bestaat uit exact 4 alfanumerieke karakters. De versiecode is uniek voor alle instrumenten die met hetzelfde dossiernummer op een openbare weblocatie beschikbaar gesteld en in het Manifest aangeduid zijn. <br/>
</td>
</tr>
</tbody>
</table>

Het gedeelte van het identificatienummer tot aan het liggend streepje wordt het dossiernummer genoemd. De reguliere expressie voor het dossiernummer is derhalve als volgt:

NL\.(IMRO)\.[0-9]{4}\.[A-Za-z0-9]{1,18}<br/>
## Bestandsnaam vereisten {#4036FA61}

Voor ieder bronbestand worden in <a href='#T001'>Tabel 1</a> en <a href='#T002'>Tabel 2</a> eisen gesteld aan de bestandsnaam. De reguliere expressie waarmee de naam van een bestand wordt beschreven, is als volgt:

([a-z]{1,2}\_)?NL\.(IMRO)\.[0-9]{4}\.[A-Za-z0-9]{1,18}-[A-Za-z0-9]{4}<br/>
(\_[A-Za-z0-9\.]{1,20})?\.(html|htm|xhtml|xml|gml|pdf|png|jpg|jpeg)

In <a href='#T005'>Tabel 5</a> worden de onderdelen van deze reguliere expressie nader verklaard.

<table style='width: 100%;' id='T005'><caption>Tabel 5 Onderdelen van de bestandsnaam vereisten</caption>
<colgroup><col id='col1' style='width: 43.73648879280919%;'>
<col id='col2' style='width: 56.26351120719081%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Onderdeel<br/>
</th>
<th align='left'>Betekenis <br/>
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'>([a-z]{1,2}\_)?<br/>
</td>
<td align='left'>Het type onderdeel als één of twee letters en een underscore _ ; dit onderdeel wordt bij het GML bestand niet toegepast en is daarom optioneel; de beschrijving van de lettercodes wordt nader uitgewerkt bij de bestandsnaamconventies.<br/>
</td>
</tr>
<tr><td align='left'>NL\.(IMRO)\.[0-9]{4}\.[A-Za-z0-9]{1,18}-[A-Za-z0-9]{4}<br/>
</td>
<td align='left'>idn van het ruimtelijk instrument.<br/>
</td>
</tr>
<tr><td align='left'>(_[A-Za-z0-9\.]{1,20})?<br/>
</td>
<td align='left'>bij bijlagen en illustraties wordt het identificatienummer gevolgd door een underscore _ en daarna een nadere aanduiding van minimaal 1 en maximaal 20 alfanumerieke tekens en punten, te bepalen door de bronhouder. <br/>
</td>
</tr>
<tr><td align='left'>\.<br/>
</td>
<td align='left'>Een punt .<br/>
</td>
</tr>
<tr><td align='left'>(html|htm|xhtml|xml|gml|pdf|png|jpg|jpeg)<br/>
</td>
<td align='left'>De mogelijke bestandsextensies; de exacte relaties tussen onderdelen en bestandsformaten is nader uitgewerkt in paragraaf <a href='#647D7CE0'>2.2</a> (met IMROPT) en <a href='#647D7D0F'>2.3</a>(zonder IMROPT).<br/>
</td>
</tr>
</tbody>
</table>

