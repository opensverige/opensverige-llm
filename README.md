# OpenSverige LLM

Ett öppet, communitydrivet och **eval-first** initiativ för små svenska och
nordiska specialistmodeller.

Projektet är i en tidig orienteringsfas. Vi har ännu inte valt slutligt scope,
tränat någon modell eller verifierat någon modell för produktionsbruk. Scope,
prioriteringar och acceptanskriterier ska beslutas öppet genom RFC:er och
community-omröstningar.

## Vision

Göra det praktiskt möjligt att utveckla, jämföra och dokumentera små modeller
som löser avgränsade svenska eller nordiska uppgifter med mätbar kvalitet,
rimlig kostnad och tydlig spårbarhet.

## Principer

- **Eval före träning:** definiera uppgift, baslinje och acceptanskriterier
  innan dataframtagning eller finjustering.
- **Smalt före generellt:** optimera för en tydlig uppgift, inte för att bygga
  ännu en generell språkmodell.
- **Reproducerbart:** publicera versionsatta datasetkort, evaler, konfiguration
  och resultat när licenser och sekretess tillåter.
- **Starka baslinjer:** jämför mot regler, sök/RAG och tillgängliga modeller.
  Träning är inte automatiskt rätt lösning.
- **Svenska först, nordiskt kompatibelt:** prioritera svenska behov och designa
  så att danska, norska, finska och isländska bidrag kan läggas till.
- **Öppen styrning:** större beslut tas via RFC och dokumenterad poll.
- **Ansvarsfullt:** dataskydd, säkerhet, licenser och mänsklig kontroll är
  produktkrav, inte efterarbete.

## Kandidatspår

Följande är **kandidater**, inte beslutade åtaganden:

1. **LagKlar / krav ↔ anbud** – strukturera, matcha och motivera kopplingar
   mellan krav och anbudstext. Evaler bör mäta bland annat täckning,
   evidensanknytning, abstention och falskt positiva matchningar.
2. **Micro decision/router** – en mycket liten modell som väljer verktyg,
   modell, arbetsflöde eller eskalering för ett begränsat antal beslut.
   Evaler bör mäta routingkvalitet, kalibrering, latens och kostnad.

Alternativ, avgränsningar och ordningsföljd beslutas genom en inledande
[community-RFC](governance/RFC_TEMPLATE.md) och poll. Nya kandidatspår är
välkomna om de har en tydlig användare, eval och dataväg.

## Föreslaget arbetssätt

1. Beskriv uppgiften och riskerna i en RFC.
2. Skapa en fryst, versionsatt eval-svit med baslinjer.
3. Dokumentera tillåtna datakällor, proveniens, licens och borttagning.
4. Testa enklaste fungerande lösning (regler/RAG/promptning) före träning.
5. Träna endast om mätningarna motiverar det.
6. Publicera resultat inklusive misslyckanden, begränsningar och kostnad.

Se [roadmap](roadmap/ROADMAP.md), [benchmarkguide](benchmark/README.md) och
[exempelscheman](schemas/).

## Resurser och roller vi söker

- domänexperter inom upphandling, kravarbete och svensk offentlig sektor
- ML-/NLP-utvecklare och MLOps-kompetens
- dataförvaltare med licens-, GDPR- och provenienskompetens
- eval-/red-team-bidrag och svensk/nordisk språkkompetens
- juridisk rådgivning för data- och användningsvillkor
- beräkningsresurser, lagring och CI-sponsring
- maintainers för dokumentation, community och releaseprocess

Roller ger inte ensam beslutanderätt; se [governance](governance/README.md).

## Säkerhet och juridiska gränser

Projektets artefakter är forskning och utveckling, **inte juridisk rådgivning**
och inte garanti för att ett krav, anbud eller beslut är korrekt. En eventuell
LagKlar-modell får inte presenteras som juridiskt tillförlitlig. Högriskbeslut
ska ha kvalificerad mänsklig granskning, spårbar evidens och möjlighet att
avstå/eskalera.

Bidra inte med personuppgifter, sekretessbelagda uppgifter, skyddsvärda
anbudshandlingar eller material utan rätt att använda och återpublicera.
Kodlicensen omfattar inte automatiskt dataset, modellvikter eller tredjeparts-
material; varje artefakt måste få ett eget licens- och dataset-/modellkort.

Rapportera sårbarheter enligt [SECURITY.md](SECURITY.md), inte i en publik issue.

## Konkreta nästa steg

- öppna och diskutera RFC:n för första scope/poll
- rekrytera två domänexperter per prioriterat spår
- enas om evalmått, baslinjer och stoppkriterier
- inventera data med proveniens och rättslig grund
- skapa en liten, manuellt granskad eval-svit
- kör baslinjer innan beslut om träning

## Bidra

Läs [CONTRIBUTING.md](CONTRIBUTING.md) och vår
[uppförandekod](CODE_OF_CONDUCT.md). Små dokumentationsfixar kan skickas
direkt; scope, data, benchmarkändringar och modellreleaser ska börja med en
issue eller RFC.

Koden är licensierad under [MIT License](LICENSE).
