# Governance

OpenSverige LLM drivs öppet av bidragsgivare och maintainers. Den här första
modellen är avsiktligt enkel och kan ändras genom RFC.

## Beslut

- Små, reversibla ändringar beslutas i PR-review.
- Scope, kandidatspår, evalprotokoll, data, modellreleaser och styrning kräver
  en numrerad RFC.
- En RFC ska vara öppen för kommentarer i minst sju kalenderdagar.
- Därefter genomför maintainers en dokumenterad community-poll med tydliga
  alternativ, röstperiod och beslutskriterium.
- Maintainers sammanfattar argument, utfall, reservationer och nästa steg.
  Popularitet ersätter inte säkerhets-, licens- eller dataskyddskrav.

Innan repot har utsedda maintainers får inga irreversibla beslut om scope,
data eller release tas. Vid akut säkerhetsrisk får en maintainer tillfälligt
stoppa en release eller ta bort exponering; beslutet ska följas upp öppet när
det kan ske säkert.

## Roller

- **Contributor:** deltar i issues, RFC:er, data, evaler eller kod.
- **Reviewer:** har dokumenterad kompetens inom ett område och granskar där.
- **Maintainer:** förvaltar repo, process och releaser; utses genom RFC/poll.
- **Domain steward:** bevakar uppgiftsdefinition och konsekvenser i domänen.
- **Data steward:** bevakar proveniens, licenser, integritet och borttagning.

Roller ska dokumenteras i repot när personer utses. Intressekonflikter ska
deklareras i relevanta beslut.

## RFC-livscykel

`Draft → Discussion → Poll → Accepted/Rejected → Implemented/Superseded`

Kopiera [RFC-mallen](RFC_TEMPLATE.md) till `governance/rfcs/NNNN-kort-namn.md`
i en PR. RFC-numret tilldelas vid merge. Ändringar mot en accepterad RFC ska
vara spårbara i roadmap, issues och PR:er.
