# Initial roadmap

Roadmapen är ett diskussionsunderlag. Communityns första RFC och poll kan
ändra ordning, scope och innehåll.

## 0. Förankring och styrning

- [ ] utse initiala maintainers, domain stewards och data stewards
- [ ] acceptera eller revidera governanceprocessen
- [ ] samla kandidatspår och publicera jämförbar beslutsmatris
- [ ] rösta om första avgränsade spår och framgångskriterier

**Exit:** accepterad RFC med scope, ägare, risker, resurser och mätbara mål.

## 1. Eval och baslinjer

- [ ] definiera taxonomi, mått, abstention och felkostnader
- [ ] skapa liten manuellt dubbelgranskad eval-svit
- [ ] frysa en blind testdel och dokumentera läckageskydd
- [ ] köra regel-, sök/RAG- och modellbaslinjer

**Exit:** reproducerbara baslinjer och beslutad förbättringströskel.

## 2. Data readiness

- [ ] inventera källor och licenser
- [ ] dokumentera proveniens, borttagning och personuppgiftsbedömning
- [ ] mäta täckning, obalans och annotatörsöverensstämmelse
- [ ] godkänna datasetkort före träning

**Exit:** versionerad, tillåten data eller dokumenterat beslut att inte träna.

## 3. Experiment

- [ ] testa enklaste lösningen först
- [ ] jämföra liten finjustering endast om baslinjer motiverar det
- [ ] redovisa kvalitet, kalibrering, latens, kostnad och risk
- [ ] genomföra red-team och domängranskning

**Exit:** transparent go/no-go mot RFC:ns acceptans- och stoppkriterier.

## 4. Kandidatrelease

- [ ] modell-/systemkort, evalrapport och reproduktionsinstruktioner
- [ ] licens- och säkerhetsgranskning
- [ ] tydliga begränsningar, mänsklig kontroll och återställningsplan
- [ ] tidsbegränsad kandidat med incident- och feedbackkanal

**Exit:** communitygodkänd release eller arkiverat experiment med lärdomar.
