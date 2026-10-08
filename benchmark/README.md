# Benchmarkkonvention

Benchmarken ska mäta en avgränsad förmåga, inte skapa ett allmänt
"intelligenspoäng". Varje benchmarkversion bör innehålla:

- uppgiftsdefinition och avsedd användning
- källor, licenser, språk/region och tidsperiod
- annoteringsguide och kvalitetskontroll
- frysta train/dev/test-splitar och läckageanalys
- mått, konfidensintervall och felkostnader
- regel-/sök-/modellbaslinjer
- slices för språk, dokumenttyp, svårighet och risk
- kända begränsningar och ändringslogg

Rapportera alltid antal exempel och osäkerhet, inte bara ett medelvärde.
Resultat från olika benchmarkversioner får inte jämföras som om de vore samma.

## Kandidatspecifika mått

**Krav ↔ anbud:** precision/recall per krav, evidenstäckning, stöd för
motiveringen, abstention, kritiska falskt positiva/negativa och
domänexpertbedömning.

**Decision/router:** accuracy eller kostnadsviktad regret, kalibrering,
abstention/eskalering, latens, kostnad samt robusthet mot okända och skadliga
instruktioner.

Se [benchmark-item.schema.json](../schemas/benchmark-item.schema.json) och det
syntetiska [exemplet](../examples/benchmark-item.json). Lägg aldrig verklig
sekretessbelagd anbudsdata i repot.
