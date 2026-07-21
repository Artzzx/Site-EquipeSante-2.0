# Yoast SEO — Page Rendez-vous (téléphone uniquement)
**URL de la page :** https://equipesanteplus.ca/rendez-vous/
**Langue :** fr-CA
**Date :** 2026-07-21

> ⚠️ **Changement de politique** : la réservation en ligne (iframe Medexa) a été retirée. Tous les rendez-vous se prennent désormais uniquement par téléphone au **(579) 957-9690**. Yoast doit être mis à jour en conséquence — les anciens champs contenaient des mentions « réservation en ligne » qui ne sont plus vraies.

---

## 1. Onglet SEO — Champs à remplir dans Yoast

> Accès : WordPress Admin → Pages → Rendez-vous → Yoast SEO (en bas de l'éditeur) → Onglet "SEO"

| Champ Yoast | Valeur à saisir |
|---|---|
| **Keyphrase cible** | rendez-vous infirmière à domicile longueuil |
| **Titre SEO** | Rendez-vous Infirmière à Domicile – Rive-Sud \| Équipe Santé+ |
| **Slug (permalien)** | rendez-vous |
| **Méta description** | Prenez rendez-vous avec une infirmière à domicile sur la Rive-Sud en un appel. Composez le 579-957-9690 : évaluation personnalisée, service bilingue à Longueuil, Brossard et Saint-Hubert. |

**Aperçu Google attendu :**
```
Rendez-vous Infirmière à Domicile – Rive-Sud | Équipe Santé+
https://equipesanteplus.ca/rendez-vous/
Prenez rendez-vous avec une infirmière à domicile sur la Rive-Sud en un appel. Composez le 579-957-9690 : évaluation personnalisée, service bilingue à Longueuil, Brossard et Saint-Hubert.
```

---

## 2. Onglet SEO — Analyse de lisibilité et SEO (Yoast)

| Indicateur Yoast | Statut attendu | Action si rouge |
|---|---|---|
| Keyphrase dans le titre SEO | 🟢 Vert | "Rendez-vous Infirmière à Domicile" présent |
| Keyphrase dans la méta description | 🟢 Vert | "infirmière à domicile" et "Longueuil" présents |
| Keyphrase dans le H1 | 🟡 Orange | H1 = "Prenez rendez-vous par téléphone" — le mot "infirmière" est dans le sous-titre |
| Keyphrase dans l'introduction | 🟢 Vert | Sous-titre contient "soin infirmier à domicile" |
| Densité de keyphrase (0.5–3%) | 🟢 Vert | Keyphrase présente dans les étapes, avantages et FAQ |
| Longueur du texte (>900 mots) | 🟢 Vert | Étapes + section téléphonique + avantages + FAQ |
| Liens internes | 🟢 Vert | 4 liens internes (Prix, FAQ, Contact + lien courriel) |
| Liens sortants | 🟢 Vert | Lien `tel:` et `mailto:` présents (l'iframe externe Medexa a été retirée) |
| Alt text images | 🟢 Vert | Aucune image — SVG décoratifs marqués `aria-hidden` |

> **Note** : Le schéma `ReserveAction` a été **retiré** (il annonçait une réservation en ligne qui n'existe plus et pouvait générer des réclamations). Il est remplacé par `ContactPoint` avec heures d'ouverture — Google peut afficher un bouton « Appeler » dans le Knowledge Panel.

---

## 3. Onglet "Réseaux sociaux" — Open Graph & Twitter Card

### Facebook / Open Graph
| Champ | Valeur à saisir |
|---|---|
| **Titre OG** | Prendre rendez-vous — Infirmière à Domicile Rive-Sud |
| **Description OG** | Appelez le 579-957-9690 pour planifier votre soin infirmier à domicile. Évaluation personnalisée par notre équipe. Service bilingue à Longueuil, Brossard, Saint-Hubert et toute la Rive-Sud. |
| **Image OG** | Photo de l'équipe ou du logo — dimensions : **1200 × 630 px** |

### Twitter / X Card
| Champ | Valeur à saisir |
|---|---|
| **Type de carte** | `summary_large_image` |
| **Titre Twitter** | Rendez-vous Infirmière — Rive-Sud |
| **Description Twitter** | Appelez le 579-957-9690 pour prendre rendez-vous. Soins infirmiers à domicile à Longueuil, Brossard et sur la Rive-Sud. |
| **Image Twitter** | Même image que OG (1200 × 630 px) |

---

## 4. Schema.org ajouté dans le HTML

| Propriété | Valeur |
|---|---|
| **Type principal** | `["MedicalBusiness", "LocalBusiness"]` |
| **Action** | ~~`ReserveAction`~~ **retirée** — remplacée par `ContactPoint` avec `hoursAvailable` |
| **FAQ** | `FAQPage` avec 5 questions (dont « Puis-je réserver en ligne ? » qui clarifie que non) |
| **Champs remplis** | name, description, url, telephone, email, areaServed, contactPoint (téléphone, langues, heures) |
| **Où dans le HTML** | Script JSON-LD en bas de page + microdata FAQPage sur la section FAQ |

---

## 5. Mots-clés secondaires (à intégrer dans Yoast — champ "Keyphrases secondaires")

| # | Mot-clé secondaire | Intention |
|---|---|---|
| 1 | prendre rendez-vous infirmière rive-sud | transactionnelle |
| 2 | téléphone infirmière à domicile longueuil | transactionnelle / locale |
| 3 | rendez-vous soins infirmiers brossard | transactionnelle |
| 4 | comment prendre rendez-vous infirmière domicile | informationnelle |

---

## 6. Liens internes — Récapitulatif

| Lien dans la page | Texte d'ancre | Page de destination |
|---|---|---|
| Section téléphone (numéro affiché) | (579) 957-9690 | `tel:+15799579690` |
| Section téléphone (alternative) | infos@equipesanteplus.ca | `mailto:infos@equipesanteplus.ca` |
| Section téléphone (alternative) | page contact | https://equipesanteplus.ca/contact/ |
| Pied de page | Consulter nos tarifs | https://equipesanteplus.ca/prix/ |
| Pied de page | Lire la FAQ | https://equipesanteplus.ca/faq/ |
| Pied de page | Nous contacter | https://equipesanteplus.ca/contact/ |

---

## 7. Checklist de déploiement final

- [ ] HTML collé dans le widget Elementor et sauvegardé
- [ ] **Iframe Medexa retirée** — vérifier qu'aucun autre widget Elementor sur cette page ne charge encore l'iframe de réservation
- [ ] **Compte Medexa / lien de réservation** : décider s'il faut désactiver l'accès public (formulaire orphelin) — hors du champ de cette page
- [ ] Yoast : mettre à jour le titre SEO et la méta description (les anciennes valeurs mentionnaient « réservation en ligne » qui n'existe plus)
- [ ] Yoast : supprimer toute mention `ReserveAction` dans l'onglet Schema si Yoast Premium a été configuré manuellement
- [ ] Slug vérifié : `/rendez-vous/`
- [ ] Image OG uploadée dans l'onglet Réseaux sociaux de Yoast
- [ ] Keyphrases secondaires saisies
- [ ] Page publiée et testée sur mobile — le numéro doit être cliquable (`tel:`)
- [ ] Vérifier les autres pages qui liaient vers `/rendez-vous/` comme point de « réservation en ligne » (home, service pages, FAQ) et adapter les ancres si elles promettent « réserver en ligne »
- [ ] URL soumise dans Google Search Console → "Demander l'indexation"
- [ ] Test Rich Results Google : vérifier que le `FAQPage` et le `ContactPoint` sont valides et qu'aucune erreur `ReserveAction` ne subsiste
- [ ] Résultat Yoast : minimum 4 feux verts sur 5 indicateurs principaux
