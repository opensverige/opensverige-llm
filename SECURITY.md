# Säkerhetspolicy

## Rapportera privat

Publicera inte sårbarheter, läckta uppgifter eller reproduktionssteg i en
publik issue. Använd GitHubs **Report a vulnerability** under repots flik
Security. Om funktionen inte är tillgänglig, kontakta en maintainer privat via
OpenSveriges etablerade kontaktkanal och be om en säker rapporteringsväg.

Ange gärna:

- berörd version, commit eller artefakt
- påverkan och förutsättningar
- minsta möjliga reproduktion utan verkliga person- eller kunddata
- förslag på åtgärd, om du har ett

Vi bekräftar mottagande när en maintainer har triagerat rapporten och
samordnar publicering efter att en åtgärd finns. Ingen garanti om svarstid
lämnas innan en formell security-grupp är utsedd.

## Omfattning

Policyn gäller kod, pipelines och projektpublicerade eval-/modellartefakter.
Dataskyddsincidenter, prompt injection, modellutvinning, dataläckage och
felaktig åtkomstkontroll räknas som säkerhetsfrågor. Vanliga modellfel utan
säkerhetspåverkan rapporteras som issues utan skyddsvärda data.

## Ansvarsfull testning

Testa endast system och data du har tillstånd att använda. Försök inte komma åt
andra användares data, påverka tillgänglighet eller publicera hemligheter.
