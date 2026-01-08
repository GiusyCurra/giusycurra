# Sito Giusy Currà - Social Media Manager

Sito personale per presentare i servizi di social media management.

## Struttura dei File

```
giusycurra/
├── index.html        (Pagina principale)
├── style.css         (Stili CSS)
├── README.md         (Questo file)
└── images/           (Cartella per le foto)
```

## Come Modificare il Sito

### 1. Titolo e Descrizione Pagina
Apri `index.html` e modifica le righe 6-7:
```html
<title>Giusy Currà - Social Media Manager</title>
<meta name="description" content="Sono Giusy Currà, social media manager...">
```

### 2. Testo del Hero (sezione grande)
Cerca questa sezione e modifica il testo:
```html
<!-- Hero -->
<section id="home" class="hero">
  <h1>Fai Crescere il Tuo Brand sui Social Media</h1>
  <p>Sono Giusy Currà, social media manager specializzata...</p>
  <a href="#contact" class="btn">Contattami</a>
</section>
```

### 3. Servizi
Modifica le tre card qui:
```html
<!-- Servizi -->
<section id="services" class="services">
  <h2>I Miei Servizi</h2>
  <div class="grid">
    <div class="card">
      <h3>📱 Gestione Social Media</h3>
      <p>Scrivi qui la descrizione del servizio...</p>
    </div>
    <!-- Altre card... -->
  </div>
</section>
```

### 4. Sezione "Chi Sono"
Modifica qui il tuo testo:
```html
<!-- Chi Sono -->
<section id="about">
  <h2>Chi Sono</h2>
  <p>Scrivi qui la tua biografia...</p>
</section>
```

### 5. Contatti nel Footer
Modifica email, WhatsApp e Instagram:
```html
<!-- Footer -->
<footer id="contact">
  <h2>Contattami</h2>
  <p>📧 Email: <a href="mailto:TUA_EMAIL">TUA_EMAIL</a></p>
  <p>📱 WhatsApp: <a href="https://wa.me/TUO_NUMERO">Inviami un messaggio</a></p>
  <p>🌐 Instagram: <a href="https://instagram.com/TUO_USERNAME">@TUO_USERNAME</a></p>
</footer>
```

---

## Come Aggiungere Foto

### Passo 1: Salva le foto
1. Scarica/prepara le tue foto
2. Mettile nella cartella **`images`**
3. Usa questi nomi di file:
   - `profile.jpg` - Foto profilo per "Chi Sono"
   - `hero.jpg` - Foto copertina nel Hero
   - `service-1.jpg`, `service-2.jpg`, `service-3.jpg` - Foto servizi

### Passo 2: Aggiungi la foto nel Hero
Apri `index.html` e modifica la sezione Hero così:
```html
<!-- Hero -->
<section id="home" class="hero">
  <img src="images/hero.jpg" alt="Copertina social media" class="hero-img">
  <h1>Fai Crescere il Tuo Brand sui Social Media</h1>
  <p>Sono Giusy Currà...</p>
  <a href="#contact" class="btn">Contattami</a>
</section>
```

### Passo 3: Aggiungi la foto in "Chi Sono"
```html
<!-- Chi Sono -->
<section id="about">
  <h2>Chi Sono</h2>
  <img src="images/profile.jpg" alt="Foto di Giusy Currà" class="profile-img">
  <p>Sono Giusy Currà, social media manager...</p>
</section>
```

### Passo 4: Aggiungi foto nei servizi
```html
<div class="card">
  <img src="images/service-1.jpg" alt="Gestione social media" class="card-img">
  <h3>📱 Gestione Social Media</h3>
  <p>Amministrazione completa...</p>
</div>
```

### Passo 5: Aggiungi stili nel CSS
Apri `style.css` e aggiungi alla fine:
```css
/* Immagini */
.profile-img {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  margin-bottom: 1rem;
  object-fit: cover;
}

.hero-img {
  width: 100%;
  height: 300px;
  object-fit: cover;
  margin-bottom: 2rem;
  border-radius: 0.5rem;
}

.card-img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  margin-bottom: 1rem;
  border-radius: 0.5rem;
}
```

---

## Colori Personalizzati

Se vuoi cambiare i colori, apri `style.css` e modifica queste variabili:
```css
:root {
  --primary: #6366f1;      /* Blu (menu, bottoni) */
  --secondary: #ec4899;    /* Rosa (hover) */
  --dark: #0f172a;         /* Nero (footer) */
  --light: #f8fafc;        /* Grigio chiaro (sfondo) */
  --text: #1e293b;         /* Grigio scuro (testo) */
  --gray: #64748b;         /* Grigio testo */
}
```

---

## Test Responsive

Per verificare che il sito funzioni bene anche da cellulare:
1. Apri il sito nel browser
2. Premi `F12` per aprire Developer Tools
3. Clicca su "Toggle device toolbar" (icona smartphone)
4. Prova diversi dispositivi

---

## FAQ

**D: Come cambio il font?**
In `style.css` modifica questa riga:
```css
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
```

**D: Come aggiungo un'altra sezione?**
Copia una sezione esistente e adatta il testo e l'ID nel menu.

**D: Le foto sono sfocate/distorte**
Usa foto con le giuste dimensioni (almeno 1200x800px per hero, 500x500px per profile).

---

Buona modifica! 🚀
