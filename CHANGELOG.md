# Jurnal de modificări — Tarot

## 2.0.1 — 2026-11-02 (reîmprospătare kit)

- Nou (kit): **Sincronizare între dispozitive** (`FFF.sync`) — în dialogul «Transparență» (clic pe versiune → Copie de siguranță): conectezi două dispozitive direct (WebRTC, cod/QR, fără server și fără cont) și își schimbă datele aplicației; cea mai recentă valoare câștigă, secretele (chei API, parole) nu se trimit, ștergerile nu se propagă. Aplicarea trece prin importul kitului (confirmare, chei permise, rollback).
- Nou (kit): **Istoric local — «mașina timpului»** (`FFF.history`) — instantanee automate ale datelor (IndexedDB, fără secrete), diferență față de starea curentă și restaurare reversibilă; «Șterge datele aplicației» șterge și istoricul.
- Module adăugate: `qr`, `p2p`, `sync`, `history` (+~140 KB). Versiunea aplicației nu se schimbă.

## 2.0.1 — 2026-10-27 (anterior: 2.0.0)

Doar text (nota despre imagini).

- Notă nouă la finalul secțiunii „Istoric” (`#img-note`, cheia `t_img`, 8 limbi): aplicația nu conține imagini de cărți; istoricul Marsilia / Rider-Waite 1909 în text; statutul de domeniu public al ediției din 1909 (SUA: publicată înainte de 1930; UE/UK: autori decedați de peste 70 de ani) cu precizarea că scanările și restaurările moderne pot avea drepturi proprii; imaginile sunt marcate „planificat”.
- README: „Stare” și „Offline”.

Nu implementat:

- Imagini Rider-Waite 1909 / Marsilia înglobate: NU s-au adăugat. Din mediul meu nu am putut descărca și verifica licența fiecărei imagini (Wikimedia/arhive inaccesibile), iar aplicația nu are voie să descarce nimic la rulare.

Istoricul anterior (1.x–2.0.0) este în secțiunea „History” din README.md.
