# Prosjektstyringsplan

**Prosjekt:** Ruteplanlegging av fortransport hos Lerøy
**Emne:** LOG650 – Forskningsprosjekt i Logistikk og Kunstig Intelligens
**Prosjektperiode:** Februar–Juni 2026
**Prosjektgruppe:** 4 studenter (Hanne Haugvaldstad, Mira Wiem, Marte Dolva, Kenneth Sandvik)

---

## Sammendrag
Dette dokumentet etablerer prosjektets styringsbaseline for omfang, fremdrift, ressurser, risiko og kvalitet. Prosjektet utvikler en kvantitativ ruteoptimaliseringsmodell for fortransport av slakteklar fisk. Problemet modelleres som et Vehicle Routing Problem (VRP), et klassisk kombinatorisk optimaliseringsproblem innen transportlogistikk. Formålet er å analysere hvordan beslutningsvariabler knyttet til rutestruktur påvirker totale transportkostnader.

## Behov
Fortransport av slakteklar fisk representerer en sentral kostnadsdriver i havbruksnæringen. Det foreligger et behov for analytiske beslutningsverktøy som kan strukturere rutevalg og minimere transportkostnader under gitte kapasitets- og strukturbegrensninger.

## Roller
- **Sponsor:** Faglærer for LOG650 fungerer som prosjektsponsor og godkjenner milepæler og leveranser.
- **Kunde:** Prosjektets primære kunde er emnet LOG650. Lerøy benyttes som casegrunnlag basert på syntetisk, realistisk datastruktur.

## Forretningscase
Prosjektets verdi ligger i metodisk innsikt og demonstrasjon av hvordan kvantitative optimaliseringsmodeller kan anvendes som beslutningsstøtte innen logistikk.

### Alternativer
1) Status quo uten modell, 2) Enkel heuristisk VRP-modell (valgt), 3) Kompleks eksakt optimalisering (forkastet grunnet omfang og tidsramme).

## Forutsetninger
Syntetiske data benyttes. Transportkostnad per km og kjøretøykapasitet antas konstante gjennom analyseperioden.

## Gevinster
Forventet gevinst er dokumentert kostnadsreduksjon sammenlignet med referanseløsning (baseline).

## Kostnader
Prosjektet har ingen direkte monetær kostnad, men krever tidsressurser tilsvarende 15 studiepoeng per student.

## Analyse
Kost-nytte vurderes gjennom kvantitativ sammenligning av baseline og optimalisert løsning.

---

## Omfang
Transportnettverket består av syv oppdrettslokaliteter og ett slakteri. Scenarioanalyse inkluderer volumøkning på 20 % og kostnadsendring på ±20 %. Multimodal transport og flere slakterier er eksplisitt ekskludert.

## Mål
Utvikle og analysere en VRP-modell som minimerer total transportkostnad innen gitte begrensninger.

## Krav
- Alle lokaliteter skal besøkes én gang
- Ruten skal starte og avsluttes ved slakteriet
- Kapasitetsbegrensning skal overholdes
- Resultater skal være reproduserbare

## Løsning
Modellen implementeres i Python. Målfunksjonen kan uttrykkes som: Minimere Z = Σ (d_ij × c × x_ij), der d_ij er avstand, c er kostnad per km, og x_ij er beslutningsvariabel som indikerer om ruten går fra i til j.

## Metodisk konsistens
- Forskningsspørsmål 1 besvares gjennom modellformulering av VRP.
- Forskningsspørsmål 2 besvares gjennom kostnadssammenligning mellom baseline og optimalisert løsning.
- Forskningsspørsmål 3 besvares gjennom sensitivitet- og scenarioanalyse.

## Omfangsverifikasjon
Leveranser verifiseres gjennom intern peer-review, test av kode og dokumentert reproduserbarhet.

---

## Fremdrift
Prosjektet gjennomføres i henhold til emnets fire faser. Kritisk linje består av:
Datamodellering → Implementering → Scenarioanalyse → Rapport.

### Milepæler
| Milepæl | Dato |
| :--- | :--- |
| Proposal godkjent | 2026-02-15 |
| Prosjektplan godkjent | 2026-03-01 |
| Modell ferdig | 2026-04-01 |
| Hovedutkast | 2026-05-01 |
| Endelig levering | 2026-06-01 |

---

## Risiko
Hovedrisikoer inkluderer tidsbegrensning, begrenset Python-erfaring og modellforenkling. Risiko håndteres gjennom iterativ utvikling og tydelig avgrensning.

## Bruk av kunstig intelligens
Kunstig intelligens benyttes som støtteverktøy i kodeutvikling, datastrukturering og kvalitetssikring. Alle faglige vurderinger, modellvalg og resultattolkninger er utført av prosjektgruppen.

## Kvalitet
Kvalitet sikres gjennom reproduserbar kode, dokumenterte metodevalg, intern fagfellevurdering og konsekvent bruk av APA 7-referansestandard.
