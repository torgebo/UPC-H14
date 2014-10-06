# UiO Programming Challenge H14
Dette er oppgaverepoet for UPC høsten 2014. Informasjon herfra må ikke deles med personer utenfor oppgavegruppa før etter konkurransen.

For de som er med i oppgavegruppa er det to arbeidsoppgaver her inne:

- Lage oppgaver
- Lese/verifisere/lage løsninger oppgaver

## Hvordan lage en oppgave
En oppgave består i hovedsak av en oppgavetekst som bl.a. definerer et input- og outputformat, og et sett med testcaser som besvarelser skal valideres mot.

I tillegg må det lages fasit/løsningsforslag til oppgaven. Disse brukes til automatisk verifisering av alle testcasene.

Alle oppgaver må løses og godkjennes av minst én annen person enn oppgaveforfatter.

Her er en trinn-for-trinn beskrivelse av alt man må gjøre for å lage en oppgave som er klar til å lastes opp til testserveren.

1. Finn på problemtittel, og gi oppgaven en meningsgivende ID. IDen må være alfanumerisk og maksimalt 8 tegn lang.
2. Kopier mappen `template`, og gi kopien IDen du kom opp med som navn
3. Fyll ut problemtittel og -forfatter i `README.md`
4. Fyll ut problem-ID og -tittel i `domjudge-problem.ini`
5. Fyll ut `problem.md`
6. Legg ev. bilder i `images`
7. Lag ett eller flere eksempeltestcaser. Gi testcasene filnavn på formen `X.sample.in` og `X.sample.out` og legg dem i mappen `samples`.
8. Lag testcaser. Gi testcasene filnavn på formen `X.in` og `X.out` og legg dem i mappen `testcases`
9. Lag én eller flere løsningsforslag. Det kan være en god idé å lage løsninger som er for trege eller feil. Skriv `@EXPECTED_RESULTS@: CORRECT` som en kommentar øverst i løsningskoden. Bytt  `CORRECT` med `TIMEOUT` eller `WRONG-ANSWER` etter hva som passer. Dette brukes til automatisk testing.
10. Fyll ut `solution.md`

Legg oppgaven inn i listen under når du er ferdig med punktene over!

## Hvordan lage testcaser
Testcasene skal (ideelt) faile alle løsninger som ikke oppfyller alle kravene i oppgaveteksten. Dette betyr at alle edgecaser bør sjekkes av testcasene.

Hvis oppgaven er ment å skulle løses med en bestemt algoritme (med en gitt kompleksitet) bør du lage testcaser som sørger for at andre løsninger (f.eks. brute force) bruker for lang tid. I utgangspunktet bør riktig løsninger finne svaret på mindre enn ett sekund. Dette kan endres i `domjudge-problem.ini`.

## Oppgaver

### [A bit mean](bitmean)
__Algoritme/problemsjanger__: Triksing med binære tall  
__Forfatter__: martinvl  
__Løst av__: martinvl