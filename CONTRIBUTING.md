# Bidra till OpenSverige LLM

Tack för att du vill bidra. Projektet är communitydrivet och beslut ska vara
spårbara, inkluderande och förankrade i mätbara behov.

## Innan du börjar

- Läs [uppförandekoden](CODE_OF_CONDUCT.md) och
  [säkerhetspolicyn](SECURITY.md).
- Sök bland befintliga issues och RFC:er.
- Öppna en issue innan större arbete påbörjas.
- Använd en RFC för scope, nya modellspår, dataset, evalprotokoll,
  arkitekturval eller ändringar som påverkar projektets risknivå.

## Bidragsflöde

1. Forka repot och skapa en fokuserad branch.
2. Gör en liten, sammanhållen förändring.
3. Lägg till eller uppdatera tester/evaler och dokumentation.
4. Kontrollera att inga hemligheter, personuppgifter eller otillåtna data ingår.
5. Skicka en PR och fyll i checklistan.

Genom att bidra intygar du att du har rätt att lämna bidraget under projektets
licens. Signera commits med Developer Certificate of Origin:

```text
Signed-off-by: Namn <e-post>
```

Använd `git commit -s` för att lägga till raden automatiskt.

## Data och evaler

Databidrag måste ange:

- källa och stabil identifierare
- licens/användningsvillkor
- insamlingsmetod och datum
- personuppgifts- och sekretessbedömning
- tillåtna användningar och kända begränsningar
- kontakt eller process för rättelse/borttagning

Skicka inte känsliga, sekretessbelagda eller skyddsvärda uppgifter. Exempeldata
ska vara syntetiska eller uttryckligen tillåtna. Benchmarkändringar ska
versionssättas; testdata får inte oavsiktligt läcka in i träning.

## Granskning

Minst en maintainer granskar vanliga bidrag. För RFC:er, datareleaser,
benchmarkprotokoll och modellreleaser krävs dessutom relevant domän- eller
data/säkerhetsgranskning enligt [governance](governance/README.md).

Maintainers kan begära mindre scope, mer evidens eller att ett bidrag stoppas
av juridiska, säkerhetsmässiga eller dataskyddsrelaterade skäl.
