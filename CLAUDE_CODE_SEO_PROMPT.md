# Claude Code — Prompt SEO pour Équipe Santé+

> **Comment utiliser ce prompt :**  
> Copie tout le texte entre les lignes `---` et colle-le dans Claude Code.  
> Remplace `[URL_DE_LA_PAGE]` par le vrai lien avant d'envoyer.

---

## Prompt à donner à Claude Code

Tu travailles sur le site **Équipe Santé+** (`equipesanteplus.ca`), une clinique de soins infirmiers à domicile sur la Rive-Sud de Montréal. Le site tourne sur **WordPress + Elementor Pro (version SaaS/Cloud uniquement)**. Le plugin SEO utilisé est **Yoast SEO**.

**Page à traiter :** `[URL_DE_LA_PAGE]`

---

### Étape 1 — Lire et analyser la page

Fetch le contenu de la page à l'URL fournie. Analyse en profondeur :

1. **Le sujet principal** de la page (quel service, quelle intention de recherche ?)
2. **La structure HTML existante** : H1, H2, H3, balises sémantiques présentes ou absentes
3. **Le contenu textuel** : mots-clés naturellement présents, localisation mentionnée, longueur
4. **Les éléments Schema.org déjà en place** (s'il y en a)
5. **Les problèmes SEO visibles** : H1 manquant, hiérarchie brisée, attributs `alt` manquants, etc.

---

### Étape 2 — Déterminer le meilleur schéma Schema.org

En fonction du contenu analysé, choisis le ou les types Schema.org les plus appropriés parmi :

- `MedicalProcedure` — pour les pages de services médicaux spécifiques
- `MedicalBusiness` — pour les pages institutionnelles ou de contact
- `FAQPage` + `Question` + `Answer` — pour les pages ou sections FAQ
- `ContactPage` — pour la page de prise de RDV
- `PriceSpecification` / `Offer` — pour les pages de tarification
- `LocalBusiness` — à combiner si la page cible le SEO local (toujours pertinent)
- `BreadcrumbList` — si la page est une sous-page d'une catégorie

**Justifie ton choix** dans un commentaire HTML en haut du fichier livré :
```html
<!-- SCHEMA CHOISI : [NomDuSchema]
     RAISON : [Explication en 1-2 phrases]
     SOURCE : https://schema.org/[NomDuSchema] -->
```

---

### Étape 3 — Modifier le fichier HTML

Applique les corrections suivantes **sans modifier le contenu textuel visible de la page** (ne change pas les textes, prix, descriptions de services ou informations médicales) :

**SEO technique obligatoire :**
- Ajouter `lang="fr-CA"` sur le conteneur racine (ex: `<div class="esp-service-detail" lang="fr-CA">`)
- Intégrer les attributs Schema.org choisis aux bons éléments HTML existants
- Corriger la hiérarchie des titres si cassée (sans changer le texte des titres)
- Ajouter `aria-hidden="true"` sur tous les SVG purement décoratifs
- Ajouter ou corriger les attributs `alt` manquants sur les images
- S'assurer que les numéros de téléphone sont dans des liens `<a href="tel:+1XXXXXXXXXX">`
- Corriger les caractères mal encodés si présents (`Ã©` → `é`, `Ã ` → `à`, `Ã¨` → `è`, etc.)

**Liens internes :**
- Vérifier qu'il y a au moins 3 liens internes vers d'autres pages du site
- Si moins de 3 existent, en ajouter dans les sections de fin de page (ex: "Services complémentaires") sans créer de nouvelle section visible

**Format du fichier livré :**
- Fichier HTML unique (HTML + `<style>` + `<script>` si applicable)
- Pas de `<html>`, `<head>`, `<body>`, `<!DOCTYPE>` — le fichier doit pouvoir être collé directement dans un widget HTML Elementor
- Ne pas ajouter de librairies JavaScript ou CSS externes
- Ne pas modifier le CSS existant

---

### Étape 4 — Produire le fichier Yoast SEO

Crée un fichier Markdown séparé nommé `[nom-de-la-page]_YOAST.md`.

Ce fichier doit contenir **tout ce que je dois saisir manuellement dans Yoast SEO sur WordPress** après avoir déployé la page. Structure le fichier exactement comme suit :

```markdown
# Yoast SEO — [Nom de la page]
**URL de la page :** https://equipesanteplus.ca/[slug]/
**Langue :** fr-CA
**Date :** [date du jour]

---

## 1. Onglet SEO — Champs à remplir dans Yoast

> Accès : WordPress Admin → Pages → [nom de la page] → Yoast SEO (en bas de l'éditeur) → Onglet "SEO"

| Champ Yoast | Valeur à saisir |
|---|---|
| **Keyphrase cible** | [le mot-clé principal — ex: lavage d'oreille à domicile] |
| **Titre SEO** | [titre optimisé, max 60 caractères, format : Mot-clé principal – Rive-Sud \| Équipe Santé+] |
| **Slug (permalien)** | [slug-recommandé] |
| **Méta description** | [140–160 caractères, inclut la keyphrase, une localisation Rive-Sud, et un appel à l'action clair] |

**Aperçu Google attendu :**
```
[Titre SEO]
https://equipesanteplus.ca/[slug]/
[Méta description]
```

---

## 2. Onglet SEO — Section "Analyse de lisibilité et SEO" (Yoast)

Ces éléments sont automatiquement vérifiés par Yoast. Voici ce qui doit être au vert après déploiement :

| Indicateur Yoast | Statut attendu | Action si rouge |
|---|---|---|
| Keyphrase dans le titre SEO | 🟢 Vert | Ajuster le titre SEO ci-dessus |
| Keyphrase dans la méta description | 🟢 Vert | Ajuster la méta description ci-dessus |
| Keyphrase dans le H1 | 🟢 Vert | [vérifier si le H1 de la page contient la keyphrase] |
| Keyphrase dans l'introduction | 🟢 Vert | [le premier paragraphe contient-il la keyphrase ?] |
| Densité de keyphrase (0.5–3%) | 🟢 Vert | Ne pas sur-optimiser |
| Longueur du texte (>900 mots) | 🟢 / 🟡 | [estimation du nombre de mots de la page] |
| Liens internes | 🟢 Vert | [nombre de liens internes présents] |
| Liens sortants | 🟢 Vert | [présents ou non] |
| Alt text images | 🟢 Vert | Corrigé dans le HTML livré |

---

## 3. Onglet "Réseaux sociaux" — Open Graph & Twitter Card

> Accès : Yoast SEO → Onglet avec l'icône Facebook/Twitter

### Facebook / Open Graph
| Champ | Valeur à saisir |
|---|---|
| **Titre OG** | [titre pour partage Facebook — peut être légèrement différent du titre SEO] |
| **Description OG** | [~200 caractères, axé sur la valeur du service, pas sur les mots-clés] |
| **Image OG** | Utiliser le logo ou une image du service — dimensions recommandées : **1200 × 630 px** |

### Twitter / X Card
| Champ | Valeur à saisir |
|---|---|
| **Type de carte** | `summary_large_image` |
| **Titre Twitter** | [max 70 caractères] |
| **Description Twitter** | [max 200 caractères] |
| **Image Twitter** | Même image que OG (1200 × 630 px) |

---

## 4. Schema.org ajouté dans le HTML

| Propriété | Valeur |
|---|---|
| **Type principal** | `schema.org/[TypeChoisi]` |
| **Champs remplis** | [liste des propriétés Schema ajoutées : name, description, provider, etc.] |
| **Où dans le HTML** | [ex: sur le `<section class="esp-hero">`, sur chaque `.esp-faq-item`, etc.] |

---

## 5. Mots-clés secondaires (à intégrer dans Yoast — champ "Keyphrases secondaires")

| # | Mot-clé secondaire | Intention |
|---|---|---|
| 1 | [mot-clé] | [informationnelle / transactionnelle / locale] |
| 2 | [mot-clé] | |
| 3 | [mot-clé] | |
| 4 | [mot-clé longue traîne] | |

---

## 6. Liens internes — Récapitulatif

| Lien dans la page | Texte d'ancre | Page de destination |
|---|---|---|
| [lien 1] | [ancre] | [URL] |
| [lien 2] | [ancre] | [URL] |
| [lien 3] | [ancre] | [URL] |

---

## 7. Checklist de déploiement final

À compléter après avoir collé le HTML dans Elementor et configuré Yoast :

- [ ] HTML collé dans le widget Elementor et sauvegardé
- [ ] Keyphrase cible saisie dans Yoast
- [ ] Titre SEO saisi (vérifier compteur de caractères — max 60)
- [ ] Méta description saisie (vérifier compteur — 140 à 160 caractères)
- [ ] Slug vérifié dans WordPress (Permaliens)
- [ ] Image OG uploadée dans l'onglet Réseaux sociaux de Yoast
- [ ] Keyphrases secondaires saisies
- [ ] Page publiée et testée sur mobile
- [ ] URL soumise dans Google Search Console → "Demander l'indexation"
- [ ] Résultat Yoast : minimum 4 feux verts sur 5 indicateurs principaux
```

---

### Étape 5 — Résumé de livraison

Une fois les deux fichiers produits, présente un résumé court :

```
## Fichiers livrés

1. `[nom-page].html` — Page modifiée avec Schema.org intégré
2. `[nom-page]_YOAST.md` — Guide complet pour la configuration Yoast

## Changements apportés au HTML
- [liste des modifications SEO appliquées]
- Encodage : [OK / X caractères corrigés]
- Schema ajouté : [type]
- Liens internes : [nombre présents]

## Attention / Actions manuelles requises
- [ex: vérifier le vrai numéro de téléphone]
- [ex: fournir une image OG avant déploiement]
```

---

*Prompt réutilisable pour chaque page du site Équipe Santé+*  
*WordPress SaaS/Cloud + Elementor Pro + Yoast SEO — jamais Database ou Server version*
