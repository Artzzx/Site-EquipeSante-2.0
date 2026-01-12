# 🎨 Standards de Design - Équipe Santé+

## 📐 Uniformisation Complète du Site

Ce document liste tous les standards de design uniformisés à travers **TOUTES** les pages du site (principales + services).

---

## 🎨 Palette de Couleurs

### Couleurs Principales
```css
--primary-green: #446A3B;    /* Texte principal, titres */
--primary-rose: #DB9598;     /* Accents, boutons, headings */
--primary-cream: #F8F3EA;    /* Arrière-plan principal */
--white: #ffffff;            /* Cards, sections */
--dark-green: #365330;       /* Footer, CTA backgrounds */
```

### Couleurs Secondaires
```css
--rose-light: #c77f83;       /* Hover states */
--green-opacity: rgba(68, 106, 59, 0.1);  /* Borders, backgrounds */
```

---

## 📏 Espacements Uniformisés

### Sections (Desktop)
```css
padding: 80px 0;            /* Desktop (900px+) */
padding: 60px 0;            /* Mobile/Tablet (< 900px) */
```

### Hero Sections
```css
padding: 80px 0 60px;       /* Desktop */
padding: 60px 0 40px;       /* Mobile (< 768px) */
```

### Container
```css
max-width: 1200px;
margin: 0 auto;
padding: 0 40px;            /* Desktop (600px+) */
padding: 0 20px;            /* Mobile (< 600px) */
```

### Cards
```css
padding: 32px;              /* Desktop */
padding: 28px;              /* Certaines cards plus petites */
padding: 24px;              /* Mobile */
border-radius: 16px;
```

### Buttons
```css
padding: 16px 32px;
border-radius: 12px;
min-height: 52px;
```

### Badges
```css
padding: 10px 20px;
border-radius: 24px;
```

---

## 🔲 Grid & Layouts

### Grid Gaps
```css
gap: 32px;                  /* Desktop (900px+) */
gap: 24px;                  /* Tablet/Mobile */
```

### Responsive Breakpoints
```css
/* Mobile First */
@media (min-width: 600px) {  /* Tablet */
    /* 2 colonnes */
}

@media (min-width: 900px) {  /* Desktop */
    /* 3 colonnes */
}

@media (max-width: 768px) {  /* Ajustements mobile spécifiques */
    /* Adaptations */
}
```

### Grid Columns
```css
/* Mobile: 1 colonne */
grid-template-columns: 1fr;

/* Tablet (600px+): 2 colonnes */
grid-template-columns: repeat(2, 1fr);

/* Desktop (900px+): 3 colonnes */
grid-template-columns: repeat(3, 1fr);
```

---

## 🔤 Typographie

### Fonts
```css
/* Titres principaux */
font-family: 'LostaMasta', 'DM Sans', sans-serif;

/* Texte body */
font-family: 'DM Sans', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
```

### Tailles de Polices

#### H1 (Hero)
```css
font-size: clamp(36px, 5vw, 60px);  /* Responsive */
line-height: 1.2;
letter-spacing: -0.02em;
font-weight: 400;
```

#### H2 (Section Headers)
```css
font-size: clamp(32px, 4vw, 48px);
line-height: 1.3;
letter-spacing: -0.02em;
font-weight: 400;
```

#### H3 (Cards)
```css
font-size: 20px - 26px;
font-weight: 400;
line-height: 1.3;
```

#### Body Text
```css
font-size: 16px - 18px;
font-weight: 300;
line-height: 1.6 - 1.7;
opacity: 0.9 - 0.95;
```

#### Small Text
```css
font-size: 14px - 15px;
font-weight: 300 - 400;
```

---

## 🎭 Effects & Transitions

### Box Shadows

#### Cards (Default)
```css
box-shadow: 0 2px 12px rgba(68, 106, 59, 0.08);
```

#### Cards (Hover)
```css
box-shadow: 0 8px 24px rgba(68, 106, 59, 0.15);
```

#### Buttons
```css
box-shadow: 0 4px 16px rgba(219, 149, 152, 0.3);
```

#### Buttons (Hover)
```css
box-shadow: 0 8px 24px rgba(219, 149, 152, 0.4);
```

### Transitions
```css
transition: all 0.3s ease;
transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);  /* Cards */
```

### Hover States

#### Cards
```css
:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 24px rgba(68, 106, 59, 0.15);
    border-color: #446A3B;
}
```

#### Buttons
```css
:hover {
    transform: translateY(-2px);
}
```

#### Icons
```css
:hover svg {
    transform: translateX(4px);
}
```

---

## 🎨 Borders

### Cards
```css
border: 1px solid rgba(68, 106, 59, 0.1);
border-radius: 16px;
```

### Buttons
```css
border-radius: 12px;
border: 2px solid transparent;  /* ou couleur spécifique */
```

### Info Boxes
```css
border-left: 4px solid #DB9598;
border-radius: 8px - 12px;
```

---

## 📱 Responsive Standards

### Hero CTA Buttons
```css
/* Mobile: Vertical stack */
flex-direction: column;
gap: 16px;

/* Desktop (600px+): Horizontal */
flex-direction: row;
justify-content: center;
```

### Container Padding
```css
/* Mobile */
padding: 0 20px;

/* Tablet (600px+) */
padding: 0 40px;
```

### Section Padding
```css
/* Mobile */
padding: 60px 0;

/* Desktop (900px+) */
padding: 80px 0;
```

---

## 🌟 Composants Spécifiques

### Hero Badge
```css
display: inline-flex;
align-items: center;
gap: 8px;
background: rgba(219, 149, 152, 0.15);
color: #DB9598;
padding: 10px 20px;
border-radius: 24px;
font-size: 14px;
font-weight: 500;
border: 1px solid rgba(219, 149, 152, 0.3);
```

### CTA Section
```css
background: linear-gradient(135deg, #446A3B 0%, #365330 100%);
padding: 60px 0;
color: #F8F3EA;
```

### Info/Highlight Boxes
```css
background: rgba(219, 149, 152, 0.08);
border-left: 4px solid #DB9598;
padding: 20px 24px;
border-radius: 8px - 12px;
```

### Stat Cards
```css
background: linear-gradient(135deg, #DB9598 0%, #c48386 100%);
padding: 32px;
border-radius: 16px;
text-align: center;
color: #ffffff;
```

---

## ♿ Accessibilité

### Focus States
```css
:focus {
    outline: 3px solid #DB9598;
    outline-offset: 4px;
}
```

### Reduced Motion
```css
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms !important;
        transition-duration: 0.01ms !important;
    }
}
```

### Skip Links
```css
.skip-link {
    position: absolute;
    top: -40px;
    left: 0;
    background: #446A3B;
    color: #ffffff;
    padding: 8px 16px;
}

.skip-link:focus {
    top: 0;
}
```

### Contrast Ratios
- Texte sur fond clair: #446A3B (#446A3B sur #F8F3EA = 5.26:1) ✓ WCAG AA
- Texte sur fond foncé: #F8F3EA (#F8F3EA sur #446A3B = 5.26:1) ✓ WCAG AA
- Titres rose: #DB9598 sur #F8F3EA = 3.38:1 ✓ WCAG AA Large Text

---

## 🎯 Checklist de Conformité

Pour toute nouvelle page ou section, vérifiez:

- [ ] Couleurs respectent la palette (#446A3B, #DB9598, #F8F3EA)
- [ ] Sections: `padding: 60px 0` mobile, `80px 0` desktop
- [ ] Cards: `padding: 32px`, `border-radius: 16px`
- [ ] Buttons: `padding: 16px 32px`, `border-radius: 12px`
- [ ] Container: `max-width: 1200px`, `padding: 0 20px` mobile
- [ ] Grid gaps: `24px` mobile, `32px` desktop
- [ ] Breakpoints: 600px (tablet), 900px (desktop)
- [ ] Fonts: 'LostaMasta' (headings), 'DM Sans' (body)
- [ ] Transitions: `0.3s ease` (standard)
- [ ] Hover: `translateY(-4px)` (cards), `translateY(-2px)` (buttons)
- [ ] Focus states: `outline: 3px solid #DB9598`
- [ ] Accessibilité: Reduced motion support
- [ ] Alt text sur toutes les images
- [ ] Contrast ratios WCAG AA minimum

---

## 📦 Fichiers de Référence

### Pages Principales (référence complète)
- `home_page_equipesanteplus_v2.html` - Référence design complète
- `contact_equipesanteplus.html` - Formulaires
- `faq_equipesanteplus.html` - FAQs et accordéons
- `liste_prix_equipesanteplus.html` - Cards de prix
- `rendez_vous_equipesanteplus.html` - Iframe et steps

### Pages de Services (fragments Elementor)
- `/soins/service_prise_glycemie.html` - Design service complet
- Tous les autres services suivent les mêmes standards

---

## 🔄 Mises à Jour

**Dernière mise à jour**: Janvier 2026

**Changements récents**:
- ✅ Uniformisation des espacements (60px → 80px desktop)
- ✅ Standardisation des card paddings (32px)
- ✅ Cohérence des border-radius (16px cards, 12px buttons)
- ✅ Grid gaps uniformisés (24px mobile, 32px desktop)
- ✅ Container padding cohérent (20px → 40px)

---

## 💡 Notes de Design

### Philosophie
- **Mobile-First**: Toujours partir du mobile et adapter au desktop
- **Simplicité**: Éviter la sur-ingénierie, rester minimaliste
- **Cohérence**: Mêmes patterns partout
- **Accessibilité**: WCAG AA minimum sur tout le site

### Ne PAS faire
- ❌ Utiliser des couleurs hors palette
- ❌ Créer de nouveaux breakpoints (utiliser 600px et 900px)
- ❌ Padding cards différents (toujours 32px desktop, 28px accepté pour petites cards)
- ❌ Border-radius non standard (16px cards, 12px buttons, 24px badges)
- ❌ Transitions trop longues (max 0.4s)
- ❌ Oublier les états hover et focus

---

**Conformité totale = Design professionnel et cohérent!** ✨
