# Beschikbaar stellen {#647D7DE7}

De bronbestanden van ieder ruimtelijk instrument moeten beschikbaar worden gesteld door de bronhouder. In dit hoofdstuk zijn de eisen voor deze beschikbaarstelling gegeven, inclusief inhoud en opbouw van het Manifest en geleideformulier, dat hier een onderdeel van is.

## Eisen aan de beschikbaarstelling {#42F69F15}

Ieder ruimtelijk instrument dat is vastgelegd in het Manifest van een bronhouder dient door de bronhouder in zijn geheel beschikbaar te zijn gesteld. Dit betekent dat alle bronbestanden zoals genoemd in Tabel 1 en Tabel 2 beschikbaar zijn via het internet. Deze beschikbaarstelling moet voldoen aan een aantal eisen:

<ul><li>Publicatie van de manifesten en plannen door bronhouders van ruimtelijke plannen via standaard poort 443 voor HTTPS verkeer;</li>
<li>Het gebruik van een beveiligde <a href='https://datatracker.ietf.org/doc/html/rfc8446' target='_blank'>HTTPS verbinding via TLS</a> is wettelijk verplicht door de <a href='https://wetten.overheid.nl/BWBR0048156' target='_blank'>Wet digitale overheid</a>. Gebruik hiervoor de richtlijnen van het <a href='https://www.ncsc.nl/onderwerpen/verbindingsbeveiliging/documenten/publicaties/2021/januari/19/ict-beveiligingsrichtlijnen-voor-transport-layer-security-2.1' target='_blank'>NCSC</a>;</li>
<li>Voor de bestanden is de GET operatie van het transportprotocol van HTTP toegestaan conform de <a href=' https://forumstandaardisatie.nl/open-standaarden/http' target='_blank'>lijst van open standaarden</a> van het Forum standaardisatie;</li>
<li>Het gebruik van HTTP compressie via content encodings is onderdeel van de HTTP/1.1 standaard en is derhalve toegestaan; het gebruik hiervan kan een voordeel bieden bij het beschikbaar stellen van de potentieel erg grote planbestanden;</li>
<li>Alle bronbestanden dienen zonder autorisatie- of authenticatiemechanismen zoals inloggen beschikbaar te zijn en worden niet afgeschermd door bijvoorbeeld firewalls;</li>
<li>De beschikbaarstelling van een ruimtelijk instrument mag op iedere URL plaatsvinden en hoeft dus niet op de officiële website van de bronhouder te geschieden;</li>
<li>Alle bij het ruimtelijk instrument behorende bronbestanden worden binnen 1 virtuele directory beschikbaar gesteld.</li>
</ul>

De bronbestanden van ieder beschikbaar gesteld ruimtelijk instrument blijven toegankelijk totdat een instrument onherroepelijk in werking is getreden. Op dat moment blijven in elk geval de actuele versie van het instrument en alle eventuele daarbij behorende reactieve aanwijzingen en gerechtelijke uitspraken beschikbaar. Als een instrument geheel vervallen is, mag het in zijn geheel worden verwijderd van internet.<br/>
## Opbouw Manifest {#1A10E1C7}

Iedere bronhouder in Nederland stelt een Manifest beschikbaar. Het Manifest is een XML bestand dat een inhoudsopgave vormt van alle elektronisch beschikbare ruimtelijk instrumenten van de desbetreffende bronhouder. In het Manifest zijn de ruimtelijke instrumenten gerangschikt per dossiernummer. Aan ieder dossiernummer in het Manifest wordt een procedurestatus toegekend. De bronhouder houdt deze status per dossiernummer bij iedere wijziging actueel. Het Manifest is gewaarmerkt met een elektronische handtekening.

In aanvulling op het Manifest kent ieder ruimtelijk instrument een verplicht XML Geleideformulier met gedetailleerde informatie over het individueel instrument. Ook het geleideformulier is gewaarmerkt met een elektronische handtekening.

Het Manifest mag op ieder webadres (URL) beschikbaar worden gesteld. Het geleideformulier wordt beschikbaar gesteld binnen dezelfde virtuele directory als het instrument zelf.

Hoewel Manifest en geleideformulier beide een Signature element kennen, heeft dit element bij beide types documenten een andere inhoud en betekenis. In Hoofdstuk <a href='#1CDA4685'>6</a> wordt hier nader op ingegaan.

Het Manifest is als volgt opgebouwd:

<table style='width: 100%;'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'
<col id='col2' style='width: 6.465222348916762%;'
<col id='col3' style='width: 67.67388825541619%;'
</colgroup>
<tbody valign='top'><tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;'>Klasse

</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;' colspan='2'>Manifest

</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>attribuutnaam</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>m</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>overheidsCode<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>CBS-code van de beleidsmatig verantwoordelijke overheid. Altijd 4 cijfers, indien nodig aangevuld met voorloopnullen. Ingeval Rijk “0000”. Ingeval provincie: CBS-code provincie met voorafgaand 2 voorloopnegens. In geval deelgemeente/stadsdeel: CBS-code gemeente.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>naamOverheid<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Naam van de voor het Manifest verantwoordelijke overheid.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>datum<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Datum waarop het huidige Manifest is gegenereerd.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>dossier<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1..*<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Het ordenend element waarbinnen alle ruimtelijke instrumenten met een identiek dossiernummer worden geplaatst.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>signature<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>het PKI-Overheid waarmerk.<br/>
</td>
</tr>
</tbody>
</table>

Binnen ieder &lt;Dossier&gt; element worden de volgende gegevens opgenomen:

<table style='width: 100%;'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'
<col id='col2' style='width: 6.465222348916762%;'
<col id='col3' style='width: 67.67388825541619%;'
</colgroup>
<tbody valign='top'><tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;'>Klasse

</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;' colspan='2'>Dossier

</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>attribuutnaam</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>m</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>id<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>het dossiernummer van het desbetreffende Dossier conform het format zoals gegeven in Hoofdstuk 5 van de STRI2012.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>status<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>De actuele procedurestatus van het desbetreffende Dossier. De volgende waarden zijn mogelijk:<br/>
<ul><li><b>in voorbereiding</b></li>
<li><b>vastgesteld</b></li>
<li><b>geheel in werking</b></li>
<li><b>deels in werking</b></li>
<li><b>niet in werking</b></li>
<li><b>geheel onherroepelijk in werking</b></li>
<li><b>deels onherroepelijk in werking</b></li>
<li><b>vervallen</b></li>
<li><b>geconsolideerd</b></li>
</ul>

</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>plan<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1..*<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>informatie over ieder beschikbaar gesteld ruimtelijk instrument binnen het Dossier.<br/>
</td>
</tr>
</tbody>
</table>

Bij ieder &lt;Plan&gt; element in het Dossier worden de volgende gegevens over het ruimtelijk instrument opgenomen:

<table style='width: 100%;'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'
<col id='col2' style='width: 6.465222348916762%;'
<col id='col3' style='width: 67.67388825541619%;'
</colgroup>
<tbody valign='top'><tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;'>Klasse

</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;' colspan='2'>Plan (in Manifest)

</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>attribuutnaam</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>m</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>id<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>het idn van het desbetreffende ruimtelijk instrument conform het format zoals gegeven in Hoofdstuk 5 van de STRI2012.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>naam<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>De naam van het ruimtelijk instrument. De waarde is gelijk aan de Naam in het IMRO GML bestand.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>datum<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>De datum van het ruimtelijk instrument. De Waarde is gelijk aan de Datum in het IMRO GML bestand.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>geleideFormulier<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>De URL van het geleideformulier van het ruimtelijk instrument.<br/>
</td>
</tr>
</tbody>
</table>

De exacte opbouw van het XML Manifest is vastgelegd in een XML Schema dat naast deze standaard beschikbaar is.<br/>
## Opbouw Geleideformulier {#293B3DB0}

Het geleideformulier is opgebouwd zoals weergegeven met de tabellen in deze paragraaf.

<table style='width: 100%;'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'
<col id='col2' style='width: 6.465222348916762%;'
<col id='col3' style='width: 67.67388825541619%;'
</colgroup>
<tbody valign='top'><tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;'>Klasse

</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;' colspan='2'>Geleideformulier

</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>attribuutnaam</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>m</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>overheidsCode<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>CBS-code van de beleidsmatig verantwoordelijke overheid. Altijd 4 cijfers, indien nodig aangevuld met voorloopnullen. Ingeval Rijk “0000”. Ingeval provincie: CBS-code provincie met voorafgaand 2 voorloopnegens. Ingeval deelgemeente/stadsdeel: CBS-code gemeente. De waarde is gelijk aan IMRO:overheidsCode in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>naamOverheid<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Naam van de verantwoordelijke overheid. De waarde is gelijk aan IMRO:naamOverheid in het IMRO GML bestand van het instrument. In het geval dat de IMRO:naamOverheid in het IMRO GML bestand meer dan eens voorkomt, worden de waardes in dit attribuut achter elkaar gezet, gescheiden door komma’s.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>datum<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Datum waarop het geleideformulier is gegenereerd.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>plan<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Het ordenend element waar binnen de informatie met betrekking tot een individueel ruimtelijk instrument wordt geplaatst.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>signature<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>het PKI-Overheid waarmerk.<br/>
</td>
</tr>
</tbody>
</table>

In het &lt;Plan&gt; element in het Geleideformulier worden de volgende gegevens over het ruimtelijk instrument opgenomen:

<table style='width: 100%;'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'
<col id='col2' style='width: 6.465222348916762%;'
<col id='col3' style='width: 67.67388825541619%;'
</colgroup>
<tbody valign='top'><tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;'>Klasse

</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;' colspan='2'>Plan (in GeleideFormulier)

</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>attribuutnaam</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>m</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>id<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Identificatienummer van het instrument. De waarde is gelijk aan IMRO:identificatie in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>eigenschappen<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>root element voor alle eigenschappen van het instrument.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>onderdelen<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>root element van alle onderdelen behorende bij het instrument.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>supplementen<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>root element van de bij het instrument behorende supplementen.<br/>
</td>
</tr>
</tbody>
</table>

In het &lt;Eigenschappen&gt; element in het Geleideformulier worden de volgende gegevens over het ruimtelijk instrument opgenomen:

<table style='width: 100%;'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'
<col id='col2' style='width: 6.465222348916762%;'
<col id='col3' style='width: 67.67388825541619%;'
</colgroup>
<tbody valign='top'><tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;'>Klasse

</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;' colspan='2'>Eigenschappen

</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>attribuutnaam</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>m</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>naam<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>De naam van het ruimtelijk instrument. De waarde is gelijk aan de Naam in het IMRO GML bestand.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>type<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Het type instrument. De waarde is gelijk aan IMRO:typePlan in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>status<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>De status van het instrument. De volgende waarden zijn mogelijk:<br/>
<ul><li><b>concept</b></li>
<li><b>voorontwerp</b></li>
<li><b>ontwerp</b></li>
<li><b>vastgesteld</b></li>
<li><b>geconsolideerd</b></li>
</ul>

De waarde is gelijk aan de status in het IMRO GML bestand.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>datum<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Dit is de datum waarop de Status in werking is getreden of in werking treedt. De waarde is gelijk aan IMRO:datum in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>versieIMRO<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Dit geeft de gebruikte versie van IMRO weer die is gebruikt bij het coderen van het instrument. De waarde is gelijk aan IMRO: verwijzingNorm(norm) in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>versiePraktijkRichtlijn<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Dit geeft de gebruikte Praktijkrichtlijn weer die is gebruikt bij het coderen van het instrument. De waarde is gelijk aan IMRO: verwijzingNorm(norm) in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
</tbody>
</table>

In het &lt;Onderdelen&gt; element in het Geleideformulier wordt de volgende informatie over de beschikbaar gestelde bronbestanden opgenomen:

<table style='width: 100%;'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'
<col id='col2' style='width: 6.465222348916762%;'
<col id='col3' style='width: 67.67388825541619%;'
</colgroup>
<tbody valign='top'><tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;'>Klasse

</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;' colspan='2'>Onderdelen

</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>attribuutnaam</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>m</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>basisUrl<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>In dit attribuut wordt de virtuele directory gespecificeerd van alle onderliggende elementen.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>IMRO <br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bestandsnaam van het IMRO GML<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>planteksten<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bestandsnaam van de XML planteksten<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>regels<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bestandsnaam van de regels<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>beleidsBesluitdocument<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bestandsnaam van een beleids/besluitdocument<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>toelichting<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bestandsnaam van de toelichting<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>vaststellingsbesluit<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bestandsnaam van het vaststellingsbesluit<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bijlage<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..*<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bestandsnaam van een bijlage<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>illustratie<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..*<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bestandsnaam van een illustratie<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>geleideformulier<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>bestandsnaam van het XML geleideformulier<br/>
</td>
</tr>
</tbody>
</table>

In het &lt;Supplementen&gt; element in het Geleideformulier worden de volgende gegevens over mogelijke supplementen opgenomen:

<table style='width: 100%;'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'
<col id='col2' style='width: 6.465222348916762%;'
<col id='col3' style='width: 67.67388825541619%;'
</colgroup>
<tbody valign='top'><tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;'>Klasse

</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: #4F81BD;' colspan='2'>Supplementen

</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>attribuutnaam</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>m</i><br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>basisURL<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>In dit attribuut wordt de virtuele directory gespecificeerd van alle onderliggende elementen. <br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>startPagina<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Referentie naar een internetpagina over het instrument dat door de bronhouder beschikbaar is gesteld als startpunt van de verbeelding er van.<br/>
</td>
</tr>
<tr><td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>CSS<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>0..1<br/>
</td>
<td align='left' style='border-top: 0.5pt solid #95B3D7; border-left: 0.5pt solid #95B3D7; border-bottom: 0.5pt solid #95B3D7; border-right: 0.5pt solid #95B3D7; background-color: none;'>Referentie naar een Cascading Style Sheet (CSS) voor de lay-out en presentatie van planteksten. Dit is van toepassing op zowel objectgerichte planteksten die vanuit XML naar HTML zijn getransformeerd, als niet-objectgerichte planregels in HTML of XHTML.<br/>
</td>
</tr>
</tbody>
</table>

De exacte opbouw van het XML geleideformulier is vastgelegd in een XML Schema dat naast deze standaard beschikbaar is.<br/>
## Wijzigen reeds eerder gepubliceerde plannen {#5EBB12FD}

Ambtelijk foutherstel in een ruimtelijke plan of besluit door de bronhouder, zonder voorafgaand besluit, is het herstellen van de metadata c.q. de technische kenmerken van het ruimtelijk plan of besluit of het opheffen van inconsistenties in de planvoorraad tussen bronhouder en Ruimtelijkeplannen.nl. Het naderhand door de bronhouder aanpassen van reeds eerder gepubliceerde plannen kan en mag, indien het gaat om:<br/>
<ul><li>een (beperkte) set van metadata die van cruciaal belang is voor (blijvende) begrijpelijkheid, raadpleegbaarheid en bruikbaarheid van plannen, niet alleen in de landelijke voorziening Ruimtelijkeplannen.nl, maar ook in het Digitaal Stelsel Omgevingswet.</li>
<li>het ervoor zorgen dat, op grond van de bestaande verplichting daartoe in het Besluit ruimtelijke ordening (Bro), de lokaal aanwezige planvoorraad consistent is met de landelijke voorziening van de Wro; Ruimtelijkeplannen.nl.</li>
</ul>

Bij gebreken aan de inhoud van het plan of besluit zal het bevoegd gezag een nieuw besluit moeten nemen of een nieuwe procedure moeten volgen.<br/>
## Aanvullende specificaties {#4FC40025}

Naast de voorwaarden voor het Manifest en Geleideformulier in voorgaande paragrafen, gelden deze aanvullende specificaties:<br/>
<ul><li>het is niet mogelijk om &lt;Plan&gt; elementen met een verschillend dossiernummer binnen hetzelfde &lt;Dossier&gt; element te plaatsen;</li>
<li>het is niet mogelijk om &lt;Plan&gt; elementen met hetzelfde dossiernummer in verschillende &lt;Dossier&gt; elementen te plaatsen;</li>
<li>het is niet mogelijk om meerdere &lt;Dossier&gt; elementen met hetzelfde dossiernummer te plaatsen;</li>
<li>&lt;Dossier&gt; elementen met de status geconsolideerd bevatten alleen &lt;Plan&gt; elementen met de status geconsolideerd;</li>
<li>&lt;Dossier&gt; elementen met de status vastgesteld, geheel in werking, deels in werking, niet in werking, geheel onherroepelijk in werking of deels onherroepelijk in werking bevatten altijd minstens één &lt;Plan&gt; element met de status vastgesteld of de status onherroepelijk.</li>
<li>&lt;Plan&gt; elementen met de status geconsolideerd komen alleen voor in &lt;Dossier&gt; elementen met de status geconsolideerd;</li>
<li>voor de opbouw van het Manifest en het Geleideformulier is een XML Schema beschikbaar, dat samen met deze standaard beschikbaar is.</li>
</ul>

<p class="note">
De planstatus onherroepelijk wordt niet gebruikt in ruimtelijke plannen conform IMRO2012. De planstatus onherroepelijk is een planstatus uit het <a href='http://ro-standaarden.geonovum.nl/2008/1.1/20081224-IMRO2008.pdf' target='_blank'>Informatiemodel Ruimtelijke Ordening 2008 (IMRO2008)</a>.</p>
