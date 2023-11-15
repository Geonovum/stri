# Beschikbaar stellen {#647D7DE7}

De bronbestanden van ieder ruimtelijk instrument moeten beschikbaar worden gesteld door de bronhouder. In dit hoofdstuk zijn de eisen voor deze beschikbaarstelling gegeven, inclusief inhoud en opbouw van het Manifest en geleideformulier, dat hier een onderdeel van is.

## Eisen aan de beschikbaarstelling {#42F69F15}

Ieder ruimtelijk instrument dat is vastgelegd in het Manifest van een bronhouder dient door de bronhouder in zijn geheel beschikbaar te zijn gesteld. Dit betekent dat alle bronbestanden zoals genoemd in <a href='#T001'>Tabel 1</a> en <a href='#T002'>Tabel 2</a> beschikbaar zijn via het internet. Deze beschikbaarstelling moet voldoen aan een aantal eisen:

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

<table style='width: 100%;' id='T006'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'>
<col id='col2' style='width: 6.465222348916762%;'>
<col id='col3' style='width: 67.67388825541619%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Klasse
</th>
<th align='left' colspan='2'>Manifest
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'><i>attribuutnaam</i><br/>
</td>
<td align='left'><i>m</i><br/>
</td>
<td align='left'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left'>overheidsCode<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>CBS-code van de beleidsmatig verantwoordelijke overheid. Altijd 4 cijfers, indien nodig aangevuld met voorloopnullen. Ingeval Rijk “0000”. Ingeval provincie: CBS-code provincie met voorafgaand 2 voorloopnegens. In geval deelgemeente/stadsdeel: CBS-code gemeente.<br/>
</td>
</tr>
<tr><td align='left'>naamOverheid<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Naam van de voor het Manifest verantwoordelijke overheid.<br/>
</td>
</tr>
<tr><td align='left'>datum<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Datum waarop het huidige Manifest is gegenereerd.<br/>
</td>
</tr>
<tr><td align='left'>dossier<br/>
</td>
<td align='left'>1..*<br/>
</td>
<td align='left'>Het ordenend element waarbinnen alle ruimtelijke instrumenten met een identiek dossiernummer worden geplaatst.<br/>
</td>
</tr>
<tr><td align='left'>signature<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>het PKI-Overheid waarmerk.<br/>
</td>
</tr>
</tbody>
</table>

Binnen ieder &lt;Dossier&gt; element worden de volgende gegevens opgenomen:

<table style='width: 100%;' id='T007'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'>
<col id='col2' style='width: 6.465222348916762%;'>
<col id='col3' style='width: 67.67388825541619%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Klasse
</th>
<th align='left' colspan='2'>Dossier
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'><i>attribuutnaam</i><br/>
</td>
<td align='left'><i>m</i><br/>
</td>
<td align='left'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left'>id<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>het dossiernummer van het desbetreffende Dossier conform het format zoals gegeven in Hoofdstuk <a href='#647D7DA1'>4</a> van de STRI2012.<br/>
</td>
</tr>
<tr><td align='left'>status<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>De actuele procedurestatus van het desbetreffende Dossier. De volgende waarden zijn mogelijk:<br/>
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
<tr><td align='left'>plan<br/>
</td>
<td align='left'>1..*<br/>
</td>
<td align='left'>informatie over ieder beschikbaar gesteld ruimtelijk instrument binnen het Dossier.<br/>
</td>
</tr>
</tbody>
</table>

Bij ieder &lt;Plan&gt; element in het Dossier worden de volgende gegevens over het ruimtelijk instrument opgenomen:

<table style='width: 100%;' id='T008'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'>
<col id='col2' style='width: 6.465222348916762%;'>
<col id='col3' style='width: 67.67388825541619%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Klasse
</th>
<th align='left' colspan='2'>Plan (in Manifest)
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'><i>attribuutnaam</i><br/>
</td>
<td align='left'><i>m</i><br/>
</td>
<td align='left'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left'>id<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>het idn van het desbetreffende ruimtelijk instrument conform het format zoals gegeven in Hoofdstuk <a href='#647D7DA1'>4</a> van de STRI2012.<br/>
</td>
</tr>
<tr><td align='left'>naam<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>De naam van het ruimtelijk instrument. De waarde is gelijk aan de Naam in het IMRO GML bestand.<br/>
</td>
</tr>
<tr><td align='left'>datum<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>De datum van het ruimtelijk instrument. De Waarde is gelijk aan de Datum in het IMRO GML bestand.<br/>
</td>
</tr>
<tr><td align='left'>geleideFormulier<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>De URL van het geleideformulier van het ruimtelijk instrument.<br/>
</td>
</tr>
</tbody>
</table>

De exacte opbouw van het XML Manifest is vastgelegd in een XML Schema dat naast deze standaard beschikbaar is.<br/>
## Opbouw Geleideformulier {#293B3DB0}

Het geleideformulier is opgebouwd zoals weergegeven met de tabellen in deze paragraaf.

<table style='width: 100%;' id='T009'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'>
<col id='col2' style='width: 6.465222348916762%;'>
<col id='col3' style='width: 67.67388825541619%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Klasse
</th>
<th align='left' colspan='2'>Geleideformulier
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'><i>attribuutnaam</i><br/>
</td>
<td align='left'><i>m</i><br/>
</td>
<td align='left'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left'>overheidsCode<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>CBS-code van de beleidsmatig verantwoordelijke overheid. Altijd 4 cijfers, indien nodig aangevuld met voorloopnullen. Ingeval Rijk “0000”. Ingeval provincie: CBS-code provincie met voorafgaand 2 voorloopnegens. Ingeval deelgemeente/stadsdeel: CBS-code gemeente. De waarde is gelijk aan IMRO:overheidsCode in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left'>naamOverheid<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Naam van de verantwoordelijke overheid. De waarde is gelijk aan IMRO:naamOverheid in het IMRO GML bestand van het instrument. In het geval dat de IMRO:naamOverheid in het IMRO GML bestand meer dan eens voorkomt, worden de waardes in dit attribuut achter elkaar gezet, gescheiden door komma’s.<br/>
</td>
</tr>
<tr><td align='left'>datum<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Datum waarop het geleideformulier is gegenereerd.<br/>
</td>
</tr>
<tr><td align='left'>plan<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Het ordenend element waar binnen de informatie met betrekking tot een individueel ruimtelijk instrument wordt geplaatst.<br/>
</td>
</tr>
<tr><td align='left'>signature<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>het PKI-Overheid waarmerk.<br/>
</td>
</tr>
</tbody>
</table>

In het &lt;Plan&gt; element in het Geleideformulier worden de volgende gegevens over het ruimtelijk instrument opgenomen:

<table style='width: 100%;' id='T010'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'>
<col id='col2' style='width: 6.465222348916762%;'>
<col id='col3' style='width: 67.67388825541619%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Klasse
</th>
<th align='left' colspan='2'>Plan (in GeleideFormulier)
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'><i>attribuutnaam</i><br/>
</td>
<td align='left'><i>m</i><br/>
</td>
<td align='left'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left'>id<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Identificatienummer van het instrument. De waarde is gelijk aan IMRO:identificatie in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left'>eigenschappen<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>root element voor alle eigenschappen van het instrument.<br/>
</td>
</tr>
<tr><td align='left'>onderdelen<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>root element van alle onderdelen behorende bij het instrument.<br/>
</td>
</tr>
<tr><td align='left'>supplementen<br/>
</td>
<td align='left'>0..1<br/>
</td>
<td align='left'>root element van de bij het instrument behorende supplementen.<br/>
</td>
</tr>
</tbody>
</table>

In het &lt;Eigenschappen&gt; element in het Geleideformulier worden de volgende gegevens over het ruimtelijk instrument opgenomen:

<table style='width: 100%;' id='T011'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'>
<col id='col2' style='width: 6.465222348916762%;'>
<col id='col3' style='width: 67.67388825541619%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Klasse
</th>
<th align='left' colspan='2'>Eigenschappen
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'><i>attribuutnaam</i><br/>
</td>
<td align='left'><i>m</i><br/>
</td>
<td align='left'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left'>naam<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>De naam van het ruimtelijk instrument. De waarde is gelijk aan de Naam in het IMRO GML bestand.<br/>
</td>
</tr>
<tr><td align='left'>type<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Het type instrument. De waarde is gelijk aan IMRO:typePlan in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left'>status<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>De status van het instrument. De volgende waarden zijn mogelijk:<br/>
<ul><li><b>concept</b></li>
<li><b>voorontwerp</b></li>
<li><b>ontwerp</b></li>
<li><b>vastgesteld</b></li>
<li><b>geconsolideerd</b></li>
</ul>

De waarde is gelijk aan de status in het IMRO GML bestand.<br/>
</td>
</tr>
<tr><td align='left'>datum<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Dit is de datum waarop de Status in werking is getreden of in werking treedt. De waarde is gelijk aan IMRO:datum in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left'>versieIMRO<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Dit geeft de gebruikte versie van IMRO weer die is gebruikt bij het coderen van het instrument. De waarde is gelijk aan IMRO: verwijzingNorm(norm) in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
<tr><td align='left'>versiePraktijkRichtlijn<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>Dit geeft de gebruikte Praktijkrichtlijn weer die is gebruikt bij het coderen van het instrument. De waarde is gelijk aan IMRO: verwijzingNorm(norm) in het IMRO GML bestand van het instrument.<br/>
</td>
</tr>
</tbody>
</table>

In het &lt;Onderdelen&gt; element in het Geleideformulier wordt de volgende informatie over de beschikbaar gestelde bronbestanden opgenomen:

<table style='width: 100%;' id='T012'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'>
<col id='col2' style='width: 6.465222348916762%;'>
<col id='col3' style='width: 67.67388825541619%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Klasse
</th>
<th align='left' colspan='2'>Onderdelen
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'><i>attribuutnaam</i><br/>
</td>
<td align='left'><i>m</i><br/>
</td>
<td align='left'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left'>basisUrl<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>In dit attribuut wordt de virtuele directory gespecificeerd van alle onderliggende elementen.<br/>
</td>
</tr>
<tr><td align='left'>IMRO <br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>bestandsnaam van het IMRO GML<br/>
</td>
</tr>
<tr><td align='left'>planteksten<br/>
</td>
<td align='left'>0..1<br/>
</td>
<td align='left'>bestandsnaam van de XML planteksten<br/>
</td>
</tr>
<tr><td align='left'>regels<br/>
</td>
<td align='left'>0..1<br/>
</td>
<td align='left'>bestandsnaam van de regels<br/>
</td>
</tr>
<tr><td align='left'>beleidsBesluitdocument<br/>
</td>
<td align='left'>0..1<br/>
</td>
<td align='left'>bestandsnaam van een beleids/besluitdocument<br/>
</td>
</tr>
<tr><td align='left'>toelichting<br/>
</td>
<td align='left'>0..1<br/>
</td>
<td align='left'>bestandsnaam van de toelichting<br/>
</td>
</tr>
<tr><td align='left'>vaststellingsbesluit<br/>
</td>
<td align='left'>0..1<br/>
</td>
<td align='left'>bestandsnaam van het vaststellingsbesluit<br/>
</td>
</tr>
<tr><td align='left'>bijlage<br/>
</td>
<td align='left'>0..*<br/>
</td>
<td align='left'>bestandsnaam van een bijlage<br/>
</td>
</tr>
<tr><td align='left'>illustratie<br/>
</td>
<td align='left'>0..*<br/>
</td>
<td align='left'>bestandsnaam van een illustratie<br/>
</td>
</tr>
<tr><td align='left'>geleideformulier<br/>
</td>
<td align='left'>1<br/>
</td>
<td align='left'>bestandsnaam van het XML geleideformulier<br/>
</td>
</tr>
</tbody>
</table>

In het &lt;Supplementen&gt; element in het Geleideformulier worden de volgende gegevens over mogelijke supplementen opgenomen:

<table style='width: 100%;' id='T013'><caption></caption>
<colgroup><col id='col1' style='width: 25.860889395667048%;'>
<col id='col2' style='width: 6.465222348916762%;'>
<col id='col3' style='width: 67.67388825541619%;'>
</colgroup>
<thead valign='top'><tr><th align='left'>Klasse
</th>
<th align='left' colspan='2'>Supplementen
</th>
</tr>
</thead>
<tbody valign='top'><tr><td align='left'><i>attribuutnaam</i><br/>
</td>
<td align='left'><i>m</i><br/>
</td>
<td align='left'><i>Toelichting</i><br/>
</td>
</tr>
<tr><td align='left'>basisURL<br/>
</td>
<td align='left'>0..1<br/>
</td>
<td align='left'>In dit attribuut wordt de virtuele directory gespecificeerd van alle onderliggende elementen. <br/>
</td>
</tr>
<tr><td align='left'>startPagina<br/>
</td>
<td align='left'>0..1<br/>
</td>
<td align='left'>Referentie naar een internetpagina over het instrument dat door de bronhouder beschikbaar is gesteld als startpunt van de verbeelding er van.<br/>
</td>
</tr>
<tr><td align='left'>CSS<br/>
</td>
<td align='left'>0..1<br/>
</td>
<td align='left'>Referentie naar een Cascading Style Sheet (CSS) voor de lay-out en presentatie van planteksten. Dit is van toepassing op zowel objectgerichte planteksten die vanuit XML naar HTML zijn getransformeerd, als niet-objectgerichte planregels in HTML of XHTML.<br/>
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
