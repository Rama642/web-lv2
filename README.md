# LV 1 zadatak - Web stranica Filmovita

### LINK: [Postavite link na vašu objavljenu stranicu ovdje]

<hr />

## 📋 Opis projekta

Filmovita je responzivna web stranica izrađena u HTML-u i CSS-u (bez JavaScripta) koja prikazuje bazu filmova s različitim funkcionalnostima i vizualnim prikazima.

## ✅ Implementirane značajke

### 1. **HTML i CSS struktura**
- ✅ Tri HTML dokumenta: `index.html`, `grafikon.html`, `slike.html`
- ✅ Odgovarajući CSS dokumenti za svaku stranicu
- ✅ Semantički HTML elementi (header, nav, main, section, article, aside, footer)

### 2. **SEO i pristupačnost**
- ✅ Meta tagovi za SEO (description, keywords, Open Graph)
- ✅ ARIA atributi za pristupačnost
  - `role` atributi (banner, navigation, main, contentinfo, complementary)
  - `aria-label` i `aria-labelledby` za kontekst
  - `aria-current="page"` za trenutnu stranicu
  - `aria-required` za obavezna polja
- ✅ Skip link za keyboard navigaciju
- ✅ Screen reader only elementi
- ✅ Pristupačni focus stilovi

### 3. **Responzivnost**
- ✅ Desktop verzija (1024px+)
- ✅ Tablet verzija (768px - 1024px)
- ✅ Mobile verzija (<768px)
- ✅ Media queries za različite rezolucije
- ✅ Responzivna tablica koja se prilagođava mobilnim uređajima

### 4. **Navigacija**
- ✅ Dropdown/hamburger menu bez JavaScripta
- ✅ Koristi checkbox i CSS :checked pseudo-klasu
- ✅ Sticky navigacija
- ✅ Animirani hamburger icon

### 5. **Slike**
- ✅ Picture element za različite slike na različitim rezolucijama
- ✅ Lazy loading (loading="lazy")
- ✅ Optimizirane dimenzije slika
- ✅ Srcset za različite ekrane

### 6. **Tablica filmova**
- ✅ Stilizirana tablica s podacima o filmovima
- ✅ Hover efekti na redovima
- ✅ Responzivni prikaz (card layout na mobilnim uređajima)
- ✅ Caption za pristupačnost
- ✅ Scope atributi u zaglavlju

### 7. **Grafikoni (CSS-only)**
- ✅ **Pie Chart** - kružni grafikon s conic-gradient
- ✅ **Histogram** - stupčasti grafikon
- ✅ CSS varijable za boje i dimenzije
- ✅ Animacije:
  - Rotacija pie charta pri učitavanju
  - Rast stupaca histograma
  - Hover efekti s dodatnim informacijama
- ✅ Različiti prikazi na različitim rezolucijama:
  - Desktop: oba grafikona vidljiva
  - Tablet/Mobile: kontrole za odabir prikaza (radio buttons)

### 8. **Galerija slika**
- ✅ Grid layout za galeriju
- ✅ **Lightbox efekt bez JavaScripta** (koristi :target pseudo-klasu)
- ✅ Lazy loading za sve slike
- ✅ Zoom efekt pri hoveru
- ✅ Close dugme za zatvaranje lightboxa
- ✅ Responzivni prikaz galerije

### 9. **Dodatne značajke**
- ✅ Kontakt forma
- ✅ CSS Grid i Flexbox za layout
- ✅ CSS animacije i transformacije:
  - Slide down animacija za header
  - Fade in za sekcije
  - Hover transformacije
  - Keyframe animacije
- ✅ Gradijenti za vizualni efekt
- ✅ Box shadow i border radius za moderne izglede
- ✅ Sticky aside elementi

### 10. **Pristupačnost**
- ✅ WCAG 2.1 standardi
- ✅ Keyboard navigacija
- ✅ Screen reader podrška
- ✅ Prefers-reduced-motion za korisnika s osjetljivošću na animacije
- ✅ High contrast mode podrška
- ✅ Focus indicators

### 11. **Optimizacije**
- ✅ CSS varijable za lako održavanje
- ✅ Lazy loading za slike
- ✅ Optimizirane dimenzije slika
- ✅ Print styles
- ✅ Minimalan broj HTTP zahtjeva

## 📁 Struktura projekta

```
filmovita/
├── index.html              # Glavna stranica s tablicom filmova
├── grafikon.html           # Stranica s grafikonima
├── slike.html              # Galerija slika
├── style.css               # Zajednički stilovi za sve stranice
├── style-index.css         # Specifični stilovi za index.html
├── style-grafikon.css      # Specifični stilovi za grafikon.html
├── style-slike.css         # Specifični stilovi za slike.html
└── README.md               # Dokumentacija projekta
```

## 🎨 Dizajn

- **Boje**: Netflix-inspirirana paleta (crvena #e50914, crna #221f1f)
- **Tipografija**: Segoe UI, Abel
- **Layout**: CSS Grid i Flexbox
- **Stilovi**: Moderni, minimalisti, profesionalni

## 🚀 Pokretanje projekta

1. Preuzmi sve fajlove
2. Otvori `index.html` u web pregledniku
3. Alternativno, objavi na:
   - GitHub Pages
   - Netlify
   - Vercel
   - Drugi hosting servis

## 📊 Korišteni podaci

Projekt koristi bazu od 19 filmova s sljedećim informacijama:
- ID
- Naslov
- Godina proizvodnje
- Žanr
- Trajanje
- Država
- Ocjena

## 🛠️ Tehnologije

- HTML5
- CSS3
- Semantički markup
- ARIA atributi
- Media queries
- CSS Grid & Flexbox
- CSS varijable
- CSS animacije i transformacije

## ✨ Posebne tehnike

### Lightbox bez JavaScripta
Koristi se `:target` pseudo-klasa:
```css
.lightbox:target {
    display: flex;
}
```

### Dropdown navigacija bez JavaScripta
Koristi se checkbox i `:checked` pseudo-klasa:
```css
.nav-toggle:checked ~ .nav-menu {
    display: flex;
}
```

### Pie Chart u CSS-u
Koristi se `conic-gradient`:
```css
background: conic-gradient(
    var(--color-komedija) 0deg 94deg,
    var(--color-drama) 94deg 188deg,
    ...
);
```

### Responzivne slike
Koristi se `<picture>` element:
```html
<picture>
    <source media="(min-width: 1024px)" srcset="large.jpg">
    <source media="(min-width: 768px)" srcset="medium.jpg">
    <img src="small.jpg" alt="..." loading="lazy">
</picture>
```

## 📱 Testiranje pristupačnosti

Projekt je testiran s:
- ChromeVox (screen reader)
- Keyboard navigacija
- WAVE accessibility tool
- Lighthouse audit

## 👨‍💻 Autor

Web programiranje - LV1 zadatak
2024./2025.

## 📄 Licenca

Sva prava pridržana © 2025 Filmovita

---

**Napomena**: Prije objave, postavite link na objavljenu stranicu u sekciji LINK na vrhu ovog dokumenta.
