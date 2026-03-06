# Yoast SEO — Page FAQ
**URL de la page :** https://equipesanteplus.ca/faq/
**Langue :** fr-CA
**Date :** 2026-03-06

---

## 1. Onglet SEO — Champs à remplir dans Yoast

> Accès : WordPress Admin → Pages → FAQ → Yoast SEO (en bas de l'éditeur) → Onglet "SEO"

| Champ Yoast | Valeur à saisir |
|---|---|
| **Keyphrase cible** | faq infirmière à domicile rive-sud |
| **Titre SEO** | FAQ Infirmière à Domicile Rive-Sud \| Équipe Santé+ |
| **Slug (permalien)** | faq |
| **Méta description** | Questions fréquentes sur les soins infirmiers à domicile à Longueuil, Brossard, Saint-Hubert. Zones desservies, tarifs, heures d'ouverture, préparation aux soins — toutes les réponses ici. |

**Aperçu Google attendu :**
```
FAQ Infirmière à Domicile Rive-Sud | Équipe Santé+
https://equipesanteplus.ca/faq/
Questions fréquentes sur les soins infirmiers à domicile à Longueuil, Brossard, Saint-Hubert. Zones desservies, tarifs, heures d'ouverture, préparation aux soins — toutes les réponses ici.
```

---

## 2. Onglet SEO — Analyse de lisibilité et SEO (Yoast)

| Indicateur Yoast | Statut attendu | Action si rouge |
|---|---|---|
| Keyphrase dans le titre SEO | 🟢 Vert | "FAQ Infirmière à Domicile" présent |
| Keyphrase dans la méta description | 🟢 Vert | "soins infirmiers à domicile" présent |
| Keyphrase dans le H1 | 🟡 Orange | H1 = "Foire aux questions" — ajouter "Infirmière à Domicile" si possible |
| Keyphrase dans l'introduction | 🟢 Vert | Sous-titre contient "soins infirmiers à domicile" |
| Densité de keyphrase (0.5–3%) | 🟢 Vert | Keyphrase bien distribuée dans les réponses |
| Longueur du texte (>900 mots) | 🟢 Vert | Page FAQ longue avec plusieurs questions/réponses détaillées |
| Liens internes | 🟢 Vert | 3 liens internes ajoutés (Rendez-vous, Prix, Contact) |
| Liens sortants | 🟢 Vert | Lien tel et mailto présents |
| Alt text images | 🟢 Vert | Aucune image — SVG décoratifs marqués aria-hidden |

> **Note importante** : Le schéma **FAQPage** est en place. Si Yoast détecte les questions/réponses dans le HTML (elles sont dans la structure), Google peut afficher un **rich snippet FAQ** directement dans les résultats de recherche — visibilité maximale.

---

## 3. Onglet "Réseaux sociaux" — Open Graph & Twitter Card

### Facebook / Open Graph
| Champ | Valeur à saisir |
|---|---|
| **Titre OG** | Toutes Vos Questions sur les Soins Infirmiers à Domicile Rive-Sud |
| **Description OG** | Zones desservies, tarifs, heures, modes de paiement, préparation aux soins — Équipe Santé+ répond à toutes vos questions sur les soins infirmiers à domicile sur la Rive-Sud de Montréal. |
| **Image OG** | Utiliser une photo de l'équipe ou du logo — dimensions : **1200 × 630 px** |

### Twitter / X Card
| Champ | Valeur à saisir |
|---|---|
| **Type de carte** | `summary_large_image` |
| **Titre Twitter** | FAQ — Infirmière à Domicile Rive-Sud |
| **Description Twitter** | Zones desservies, tarifs, heures d'ouverture et plus — toutes les réponses sur les soins infirmiers à domicile. |
| **Image Twitter** | Même image que OG (1200 × 630 px) |

---

## 4. Schema.org ajouté dans le HTML

| Propriété | Valeur |
|---|---|
| **Type principal** | `schema.org/FAQPage` |
| **Champs remplis** | mainEntity → 5 Question + Answer (villes, heures, langues, paiement, préparation) |
| **Où dans le HTML** | Script JSON-LD en bas de page |
| **Impact Google** | Affichage potentiel en **Rich Snippet FAQ** dans les SERP |

---

## 5. Mots-clés secondaires (à intégrer dans Yoast — champ "Keyphrases secondaires")

| # | Mot-clé secondaire | Intention |
|---|---|---|
| 1 | questions soins infirmiers longueuil | informationnelle |
| 2 | zones desservies infirmière rive-sud | informationnelle / locale |
| 3 | OIIQ infirmière à domicile | informationnelle |
| 4 | comment prendre rendez-vous infirmière | transactionnelle |

---

## 6. Liens internes — Récapitulatif

| Lien dans la page | Texte d'ancre | Page de destination |
|---|---|---|
| Lien ajouté en bas de page | Prendre rendez-vous | https://equipesanteplus.ca/rendez-vous/ |
| Lien ajouté en bas de page | Consulter les tarifs | https://equipesanteplus.ca/prix/ |
| Lien ajouté en bas de page | Nous contacter | https://equipesanteplus.ca/contact/ |
| Lien existant (section contact) | (579) 957-9690 | tel:+15799579690 |

---

## 7. Checklist de déploiement final

- [ ] HTML collé dans le widget Elementor et sauvegardé
- [ ] Keyphrase cible saisie dans Yoast : `faq infirmière à domicile rive-sud`
- [ ] Titre SEO saisi (vérifier compteur — max 60 car.)
- [ ] Méta description saisie (vérifier compteur — 140 à 160 car.)
- [ ] Slug vérifié : `/faq/`
- [ ] Image OG uploadée dans l'onglet Réseaux sociaux de Yoast
- [ ] Keyphrases secondaires saisies
- [ ] Page publiée et testée sur mobile
- [ ] Vérifier l'affichage Rich Snippet dans Google Search Console après indexation
- [ ] URL soumise dans Google Search Console → "Demander l'indexation"
- [ ] Résultat Yoast : minimum 4 feux verts sur 5 indicateurs principaux
