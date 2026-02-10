# Love Nails - Sito Web Professionale

Sito web multi-pagina professionale e moderno per Love Nails, nail salon a Torino.

## 📋 Struttura del Sito

Il sito è composto da 5 pagine principali:

### 1. **Home Page** (`index.html`)
- Hero section con headline accattivante e CTA
- Presentazione del salone
- Sezione "Perché scegliere Love Nails" con 3 punti di forza
- Testimonianze clienti
- Call-to-action finale

### 2. **Servizi** (`servizi.html`)
- Manicure (Base, Semipermanente, Ricostruzione Gel, Refill)
- Pedicure (Classica, Semipermanente, SPA)
- Nail Art & Extra (Nail Art, Rimozione, Riparazione)

### 3. **Prezzi** (`prezzi.html`)
- Listino completo e trasparente
- Prezzi organizzati per categoria
- Note e informazioni aggiuntive

### 4. **Galleria** (`galleria.html`)
- Grid di immagini placeholder (da sostituire con foto reali)
- Linee guida fotografiche dettagliate
- Suggerimenti per la qualità delle immagini

### 5. **Contatti** (`contatti.html`)
- Informazioni complete (indirizzo, telefono, orari)
- Mappa Google Maps integrata
- Form di contatto funzionale
- Indicazioni su come raggiungere il salone

## 🎨 Design & Stile

### Palette Colori
- **Primary:** #E8B4B8 (Rosa cipria elegante)
- **Secondary:** #2D2D2D (Grigio antracite)
- **Accent:** #D4AF37 (Oro/champagne)
- **Background:** #FAFAFA (Bianco sporco)
- **Text:** #333333 (Grigio scuro)

### Tipografia
- **Headings:** Cormorant Garamond (serif elegante)
- **Body:** Montserrat (sans-serif moderna)

## 📱 Caratteristiche

### Responsive Design
- ✅ Mobile-first approach
- ✅ Ottimizzato per smartphone, tablet e desktop
- ✅ Menu hamburger su mobile
- ✅ Layout adattivo

### UX/UI
- ✅ Navigation sticky (sempre visibile)
- ✅ Pulsante WhatsApp floating
- ✅ Click-to-call su tutti i numeri di telefono
- ✅ Animazioni smooth al scroll
- ✅ Form di contatto con validazione

### SEO Ready
- ✅ Meta tag title e description
- ✅ Struttura HTML semantica
- ✅ Alt text per le immagini (da aggiungere quando si inseriscono foto reali)

## 🚀 Come Utilizzare

### 1. Personalizzazione Immediata

**Sostituire le immagini nella galleria:**
- Preparare foto professionali seguendo le linee guida in `galleria.html`
- Salvare le immagini nella cartella principale o in una sottocartella `/images`
- Sostituire i placeholder nella galleria con `<img src="path/to/image.jpg" alt="Descrizione">`

**Esempio:**
```html
<!-- Da placeholder -->
<div class="gallery-item">
    <div class="gallery-item__placeholder">...</div>
</div>

<!-- A immagine reale -->
<div class="gallery-item">
    <img src="images/manicure-1.jpg" alt="Manicure con nail art floreale">
</div>
```

### 2. Aggiornare gli Orari

Nel file `contatti.html`, cerca la sezione "Orari di Apertura" e modifica:

```html
<div class="contact__hours">
    <p><strong>Lunedì - Venerdì:</strong> TUOI_ORARI</p>
    <p><strong>Sabato:</strong> TUOI_ORARI</p>
    <p><strong>Domenica:</strong> STATO</p>
</div>
```

### 3. Configurare Google Maps

Nel file `contatti.html`, sostituisci l'URL dell'iframe con la tua mappa personalizzata:

1. Vai su [Google Maps](https://www.google.com/maps)
2. Cerca "Corso Francia, 261/A, Torino"
3. Clicca su "Condividi" > "Incorpora una mappa"
4. Copia il codice iframe
5. Sostituisci l'iframe esistente nel file `contatti.html`

### 4. Aggiungere Social Media

Se hai profili social (Instagram, Facebook, ecc.), puoi aggiungerli nel footer:

```html
<div class="footer__section">
    <h4 class="footer__subtitle">Seguici</h4>
    <div style="display: flex; gap: 15px; margin-top: 15px;">
        <a href="TUO_LINK_INSTAGRAM" target="_blank" style="color: var(--primary-color);">
            <!-- Icona Instagram -->
        </a>
        <a href="TUO_LINK_FACEBOOK" target="_blank" style="color: var(--primary-color);">
            <!-- Icona Facebook -->
        </a>
    </div>
</div>
```

### 5. Personalizzare i Prezzi

Nel file `prezzi.html`, modifica i prezzi nella tabella:

```html
<div class="pricing-row">
    <span class="pricing-row__service">Nome Servizio</span>
    <span class="pricing-row__price">€ TUO_PREZZO</span>
</div>
```

## 📧 Form di Contatto

Il form attualmente mostra un alert di conferma. Per renderlo funzionale:

**Opzione 1 - Servizio Email (Formspree, EmailJS)**
1. Registrati su [Formspree](https://formspree.io/) o [EmailJS](https://www.emailjs.com/)
2. Ottieni l'endpoint/chiave API
3. Modifica il JavaScript in `script.js` per inviare i dati

**Opzione 2 - Backend PHP**
Crea un file `send-email.php` e configura il form per inviare a questo endpoint.

## 🌐 Hosting & Deployment

### Opzioni Gratuite:
- **GitHub Pages** (per siti statici)
- **Netlify** (consigliato, con form integrati)
- **Vercel**
- **Cloudflare Pages**

### Istruzioni Base (Netlify):
1. Crea account su [Netlify](https://www.netlify.com/)
2. Trascina la cartella del sito su Netlify
3. Il sito sarà online in pochi secondi
4. Ottieni un dominio gratuito `.netlify.app` o collega il tuo dominio

## 🔧 Manutenzione

### Aggiornare i Contenuti
- **Testimonianze:** Modifica in `index.html` sezione testimonials
- **Servizi:** Aggiungi/modifica card in `servizi.html`
- **Prezzi:** Aggiorna tabelle in `prezzi.html`
- **Galleria:** Sostituisci placeholder con foto reali in `galleria.html`

### Ottimizzare le Immagini
Prima di caricare le foto:
1. Ridimensiona a max 1920px di larghezza
2. Comprimi usando [TinyPNG](https://tinypng.com/) o [Squoosh](https://squoosh.app/)
3. Salva in formato JPG o WebP
4. Usa nomi descrittivi: `manicure-gel-rosa.jpg`

## 📊 Analytics (Opzionale)

Per monitorare le visite, aggiungi Google Analytics:

1. Crea account su [Google Analytics](https://analytics.google.com/)
2. Ottieni il tracking ID
3. Aggiungi prima del `</head>` in ogni pagina:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=TUO-GA-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'TUO-GA-ID');
</script>
```

## 💡 Suggerimenti

1. **Aggiorna regolarmente la galleria** con nuovi lavori
2. **Testa il sito su diversi dispositivi** (smartphone, tablet, desktop)
3. **Monitora le conversioni** (chiamate, form inviati)
4. **Raccogli testimonianze** dai clienti soddisfatti
5. **Mantieni i prezzi aggiornati** per evitare confusioni

## 📞 Contatti

**Love Nails**
- Indirizzo: C.so Francia, 261/A - 10146 Torino (TO)
- Telefono: 338 190 8170
- WhatsApp: [Clicca qui](https://wa.me/393381908170)

## 📄 File Inclusi

```
love-nails/
│
├── index.html          # Home page
├── servizi.html        # Pagina servizi
├── prezzi.html         # Pagina prezzi
├── galleria.html       # Pagina galleria
├── contatti.html       # Pagina contatti
├── style.css           # Foglio di stile principale
├── script.js           # JavaScript per interazioni
└── README.md           # Questo file
```

## ✨ Prossimi Passi

1. ✅ Sostituire le immagini placeholder con foto professionali
2. ✅ Aggiornare gli orari di apertura
3. ✅ Configurare la mappa Google Maps
4. ✅ Testare il sito su mobile
5. ✅ Pubblicare online
6. ✅ Condividere il link con i clienti!

---

**Buona fortuna con Love Nails! 💅✨**
