# Mail a freddo Lexroom × Poste Italiane

Set **unico universale** di 3 email a freddo, valido sia per **avvocati / studi legali** sia per **aziende / team legali in-house**. Solo brand Lexroom (Poste è il vettore di invio, non viene nominata).

## Flusso
1. **`Email/01-visita-sito.html`** — CTA: visita il sito (intro generale)
2. **`Email/02-visita-sito-2.html`** — CTA: visita il sito (approfondimento, più specifico sul tema fonti verificabili)
3. **`Email/03-lead-magnet-demo.html`** — product tour (lead magnet, unico della sequenza) + prenota demo

> Il **lead magnet** compare solo nell'ultima mail ed è il **product tour**. La prima CTA della mail 3 porta alla pagina del product tour; la seconda alla prenotazione demo.

## Come visualizzarle (gratis, niente da installare)
- **Anteprima di tutte e 3 insieme:** doppio click su **`index.html`** → si apre nel browser. Pulsanti per vista singola e per simulare la larghezza mobile.
- **Singola mail:** doppio click su un file in `Email/` per aprirlo nel browser.

### (Opzionale) test su client email reali
Se vuoi verificare la resa in Gmail/Outlook/Apple Mail prima dell'invio, puoi incollare l'HTML in un servizio gratuito di anteprima (es. *Mailtrap*, *PutsMail* di Litmus, o l'editor HTML di un qualsiasi ESP). Non necessario per la revisione dei testi.

## Asset integrati
- **Banner header** (in cima a ogni mail):
  - Email 1 → `Prompt library 1.png` ("Il partner AI consigliato dai giuristi") · banner link → home
  - Email 2 → `prompt library 5.png` ("Il nuovo standard legale") · banner link → home
  - Email 3 → `prompt library 4.png` ("Il (tuo) giudizio amplificato") · banner link → product tour
- **Logo footer** → `Marchio Lexroom Blu profilo (1).png`
- **Social** (link reali): Facebook, LinkedIn, Instagram

## Hosting immagini (pubblico)
Banner e logo sono caricati su un repo GitHub pubblico e referenziati via URL diretti `raw.githubusercontent.com` (funzionano come sorgente immagini nelle email):
- Repo: https://github.com/davidefacchin-lexroom/lexroom-email-assets
- Base URL: `https://raw.githubusercontent.com/davidefacchin-lexroom/lexroom-email-assets/main/assets/`
- File: `banner-1.png` (Email 1), `banner-2.png` (Email 2), `banner-3.png` (Email 3), `logo.png`
- Per sostituire un'immagine: aggiorna il file nel repo (stesso nome) e l'URL resta valido.

> Nota: per una campagna ad alto volume è preferibile spostare le immagini sul dominio/CDN di Lexroom; in tal caso basta sostituire la base URL nei 3 file.

## Link CTA (dentro i bottoni)
- ✅ Email 1 — CTA "Scopri Lexroom": `https://lexroom.ai/soluzioni/professionisti-legali`
- ✅ Email 2 — CTA "Scopri perché Lexroom è la migliore AI legale": `https://lexroom.ai/soluzioni/professionisti-legali`
- ✅ Email 3 — CTA 1 "Scopri Lexroom": `https://www.lexroom.ai/risorse/product-tour`
- ✅ Email 3 — CTA 2 "Prenota una demo gratuita": `https://lexroom.ai/soluzioni/professionisti-legali`
- ⏳ Link **unsubscribe** nel footer (`#`): da collegare al sistema di invio
- Banner header: Email 1/2 → `https://lexroom.ai/`, Email 3 → product tour.

## FAQ in coda
Ogni mail termina con un blocco **"Domande frequenti"** (5 FAQ identiche, registro « Lei »): affidabilità/«e se l'AI inventa?», fonti e sentenze, sicurezza dati/GDPR, copertura materia, integrazione Word. Fonte: Notion "Modjo — Themes" (obiezioni, escluse prezzo/pagamento).

## Icone social (link reali)
- Facebook · LinkedIn · Instagram — rese come pulsanti `f` / `in` / `IG` (sostituibili con icone grafiche se disponibili)

## Note tecniche
- Layout a tabelle + CSS inline → compatibile con i principali client email.
- Card 600px, responsive sotto i 620px (header e immagine si impilano).
- Oggetto e preheader consigliati sono nei commenti in cima a ogni file HTML.
- Palette: navy `#131A33`, sfondo card `#EAF4F5`, bottoni cobalto `#2E45C5`, testo `#1C2B4A`.
