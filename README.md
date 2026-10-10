# Tarot — curs interactiv

Curs în română despre istoria, structura și practica tarotului, într-un singur fișier HTML, fără cont și fără server.

**Live:** https://chiuta.github.io/Tarot/

![Captura de ecran](screenshot.png)

## Ce este

Un mic curs interactiv despre tarot ca tradiție culturală și simbolică: istoric, structura pachetului de 78 de cărți, patru niveluri de curs cu exerciții, o comparație a tradițiilor (Marsilia, Rider-Waite-Smith, Thoth), glosar, jurnal și autoevaluare. Tarotul este tratat ca instrument de reflecție și divertisment, nu ca metodă științifică.

## Funcții

Secțiuni (meniul din stânga, ☰ pe mobil): Introducere, Istoric, Structura pachetului, cele patru niveluri (Fundamente, Arcanele Majore cu diagrama Călătoriei Nebunului, Arcanele Minore, Citire profesională), Aplicații practice, Tradiții și pachete, Glosar, Jurnal, Autoevaluare.

Verificate în cod și în browser:
- Extragere aleatorie de 1 sau 3 cărți dintr-un pachet virtual de 78 (amestecare Fisher–Yates cu `crypto.getRandomValues`, fără repetiții); se afișează doar numele cărților; rezultatul se poate adăuga în jurnal.
- Căutare în curs, fără sensibilitate la diacritice.
- Link direct la o secțiune (`#istoric`, `#quiz` etc.), butoanele Înapoi/Înainte ale browserului funcționează.
- Jurnal descărcabil ca `.txt`; test de 10 întrebări cu ordinea răspunsurilor amestecată.
- Printare (doar secțiunea curentă), distribuire/copiere link, ecran complet, păstrare ecran activ (unde browserul le acceptă).

## Manual de utilizare

1. Alege o secțiune din meniu (pe mobil apasă ☰).
2. Citește nivelurile în ordine și încearcă exercițiile practice.
3. În „Aplicații practice” apasă „Extrage o carte” sau „Extrage 3 cărți”; interpretarea o faci tu, cu pachetul tău.
4. Notează în „Jurnal”; apasă „Descarcă (.txt)” înainte să închizi pagina — jurnalul nu se salvează.
5. În „Autoevaluare” răspunde la cele 10 întrebări; „Reia testul” amestecă din nou răspunsurile.

## Confidențialitate și rețea

- Stocare: nu folosește `localStorage`, `sessionStorage`, IndexedDB sau cookie-uri. Jurnalul există doar în pagină; la închidere/reîncărcare browserul te avertizează dacă ai text nesalvat.
- Rețea: nu face nicio cerere externă (fără fonturi, scripturi, imagini sau analitice). Pagina are o politică CSP (`default-src 'none'`) care blochează conexiunile. Nu există linkuri externe.
- Permisiuni: nu cere nimic la încărcare. La apăsarea butoanelor pot fi folosite: ecran complet, wake lock (ecran activ), clipboard (copiere link) și vibrații pe mobil la răspunsurile din test.

## Limite și avertismente

- Tarotul este o tradiție culturală și un instrument de reflecție/divertisment. Nu există dovezi științifice că poate prezice viitorul, diagnostica sau vindeca.
- Conținutul este educațional și nu înlocuiește sfatul unui medic, psiholog, jurist sau consilier financiar. Nu renunța la un tratament și nu lua decizii importante pe baza unei extrageri.
- Afirmațiile istorice sunt prezentate pe scurt; rândurile despre certificări și cursuri din România sunt marcate ca neverificate.
- Nu include imaginile cărților; extragerea afișează doar nume.

## Rulare locală / offline

Descarcă `index.html` și deschide-l în browser; funcționează fără internet.

## Licență

Licența nu este încă declarată.

## Autor

Alexio — Alexandru-Ionuț Chiuță, contact: alexio@trom.tf

## English summary

A single-file, offline Romanian-language course on tarot as a cultural and symbolic tradition: history, the 78-card structure, four course levels, deck comparison, glossary, journal and a 10-question quiz, plus a random draw tool (Fisher–Yates with `crypto.getRandomValues`). No storage, no external requests, no telemetry. Tarot is presented as tradition and entertainment, with no scientific evidence of predictive power; it is not a substitute for medical, legal or financial advice. License not yet declared.
