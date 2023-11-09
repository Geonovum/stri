# Authenticiteitskenmerken {#1CDA4685}

De op internet beschikbaar gestelde bronbestanden inclusief Manifest en geleideformulier moeten voorzien zijn van een waarmerk waarmee de integriteit, authenticiteit en volledigheid van de bestanden worden gewaarborgd. In dit hoofdstuk worden de normen hiervoor gegeven.

## Waarmerken {#717AB549}

In het kader van de beveiliging van de digitale ruimtelijke instrumenten, wordt een aantal concrete maatregelen getroffen:

<ol><li>Waarmerken van een individueel ruimtelijk instrument door middel van een elektronische handtekening, zie paragraaf <a href='#789E64F8'>6.2</a>;</li>
<li>Waarmerken van het Manifest van een bronhouder door middel van een elektronische handtekening, zie paragraaf <a href='#647D7F2D'>6.3</a>;</li>
<li>Het waarmerken gebeurt met een elektronische handtekening waarbij gebruik gemaakt wordt van <a href='https://cert.pkioverheid.nl/' target='_blank'>certificaten van PKI-Overheid</a>;</li>
<li>De integriteit, authenticiteit en volledigheid van een individueel ruimtelijk instrument moet door de afnemers in de digitale verbeelding van dit instrument vastgesteld kunnen worden.</li>
</ol>

Bij het waarmerken wordt als technische standaard de W3C <a href='https://www.w3.org/TR/xmldsig-core1/' target='_blank'>XML-Signature Syntax and Processing (xmldsig) standaard</a> toegepast, met gebruikmaking van PKI-Overheid certificaten. Vanwege operationele veiligheidsaspecten is een aantal normatieve aanvullende restricties van toepassing, die door de landelijke voorziening <a href=' https://www.ruimtelijkeplannen.nl/' target='_blank'>Ruimtelijkeplannen.nl</a> worden gehanteerd.

Voor aanvullende specificaties en organisatorische aspecten rondom elektronische handtekeningen wordt verder verwezen naar PKI-Overheid.<br/>
## Authenticiteitskenmerken van een individueel instrument {#789E64F8}

De informatiebeveiliging van een individueel ruimtelijk instrument is als volgt:

<ol><li>van ieder individueel onderdeel zoals beschreven in Tabel 1 en Tabel 2 wordt een <a href='https://www.w3.org/TR/xmldsig-core/#sec-MessageDigests' target='_blank'>digest</a> berekend. Dit vormt een waarborg voor de integriteit en authenticiteit van de onderdelen en daarmee van het ruimtelijk instrument zelf;</li>
<li>ook over de inhoud van het geleideformulier (exclusief de elektronische handtekening) wordt een digest berekend. Dit vormt de waarborg voor de volledigheid van de onderdelen die samen het ruimtelijk instrument vormen;</li>
<li>de digests worden middels een elektronische handtekening gewaarmerkt;</li>
<li>de elektronische handtekening wordt samen met de digests vastgelegd in een XML Signature element (xmldsig) in het geleideformulier. Het geleideformulier bevat daarmee dus alle authenticiteitinformatie over het individuele ruimtelijk instrument.</li>
</ol>

Ieder ruimtelijk instrument heeft precies één gewaarmerkt geleideformulier, waarbij de inhoud van het Signature element overeen komt met bovenstaande onderdelen.<br/>
## Authenticiteitskenmerken van het Manifest {#647D7F2D}

Het Manifest heeft tot doel om de totale beschikbare instrumentele voorraad van een bronhouder te beschrijven. De informatiebeveiliging van het Manifest van de bronhouder wordt als volgt geregeld:

<ol><li>Over de inhoud van het Manifest (exclusief de elektronische handtekening) wordt een digest berekend. Dit vormt de waarborg voor de integriteit, authenticiteit en volledigheid van het Manifest;</li>
<li>De digest wordt middels een elektronische handtekening gewaarmerkt;</li>
<li>De elektronische handtekening wordt samen met de digest vastgelegd in een XML Signature element (xmldsig) in het Manifest.</li>
</ol>

Iedere bronhouder heeft precies één gewaarmerkt Manifest, waarbij de inhoud van het Signature element overeen komt met bovenstaande onderdelen.<br/>
