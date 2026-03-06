# Yoast SEO — Page Rendez-vous
**URL de la page :** https://equipesanteplus.ca/rendez-vous/
**Langue :** fr-CA
**Date :** 2026-03-06

---

## 1. Onglet SEO — Champs à remplir dans Yoast

> Accès : WordPress Admin → Pages → Rendez-vous → Yoast SEO (en bas de l'éditeur) → Onglet "SEO"

| Champ Yoast | Valeur à saisir |
|---|---|
| **Keyphrase cible** | rendez-vous infirmière à domicile longueuil |
| **Titre SEO** | Rendez-vous Infirmière à Domicile – Rive-Sud \| Équipe Santé+ |
| **Slug (permalien)** | rendez-vous |
| **Méta description** | Réservez votre soin infirmier à domicile en ligne. Disponibilités en temps réel, confirmation immédiate. Service à Longueuil, Brossard, Saint-Hubert et toute la Rive-Sud. 7j/7. |

**Aperçu Google attendu :**
```
Rendez-vous Infirmière à Domicile – Rive-Sud | Équipe Santé+
https://equipesanteplus.ca/rendez-vous/
Réservez votre soin infirmier à domicile en ligne. Disponibilités en temps réel, confirmation immédiate. Service à Longueuil, Brossard, Saint-Hubert et toute la Rive-Sud. 7j/7.
```

---

## 2. Onglet SEO — Analyse de lisibilité et SEO (Yoast)

| Indicateur Yoast | Statut attendu | Action si rouge |
|---|---|---|
| Keyphrase dans le titre SEO | 🟢 Vert | "Rendez-vous Infirmière à Domicile" présent |
| Keyphrase dans la méta description | 🟢 Vert | "soin infirmier à domicile" présent |
| Keyphrase dans le H1 | 🟡 Orange | H1 = "Prenez rendez-vous en ligne" — ajouter "infirmière" si possible |
| Keyphrase dans l'introduction | 🟢 Vert | Sous-titre contient "soin infirmier à domicile" |
| Densité de keyphrase (0.5–3%) | 🟢 Vert | Keyphrase bien présente dans les étapes et FAQ |
| Longueur du texte (>900 mots) | 🟢 Vert | Page avec étapes, avantages et FAQ détaillés |
| Liens internes | 🟢 Vert | 3 liens internes ajoutés (Prix, FAQ, Contact) |
| Liens sortants | 🟢 Vert | Lien vers la plateforme Medexa (externe) + tel présent |
| Alt text images | 🟢 Vert | Aucune image — SVG décoratifs marqués aria-hidden |

> **Note** : Le schéma **ReserveAction** est en place. Cela permet potentiellement à Google d'afficher un bouton **"Réserver"** dans les fiches d'établissement et les Knowledge Panels.

---

## 3. Onglet "Réseaux sociaux" — Open Graph & Twitter Card

### Facebook / Open Graph
| Champ | Valeur à saisir |
|---|---|
| **Titre OG** | Prenez Rendez-vous avec une Infirmière à Domicile — Rive-Sud |
| **Description OG** | Réservez en ligne en quelques clics. Disponibilités en temps réel, confirmation immédiate. Équipe Santé+ dessert Longueuil, Brossard, Saint-Hubert et toute la Rive-Sud, 7 jours sur 7. |
| **Image OG** | Utiliser une photo de l'équipe ou de l'application — dimensions : **1200 × 630 px** |

### Twitter / X Card
| Champ | Valeur à saisir |
|---|---|
| **Type de carte** | `summary_large_image` |
| **Titre Twitter** | Rendez-vous Infirmière à Domicile — Rive-Sud |
| **Description Twitter** | Réservez en ligne, disponibilités en temps réel. Service 7j/7 à Longueuil, Brossard, Saint-Hubert. |
| **Image Twitter** | Même image que OG (1200 × 630 px) |

---

## 4. Schema.org ajouté dans le HTML

| Propriété | Valeur |
|---|---|
| **Type principal** | `["MedicalBusiness", "LocalBusiness"]` |
| **Action** | `ReserveAction` avec `EntryPoint` (URL de réservation) |
| **Champs remplis** | name, description, url, telephone, potentialAction |
| **Où dans le HTML** | Script JSON-LD en bas de page |

---

## 5. Mots-clés secondaires (à intégrer dans Yoast — champ "Keyphrases secondaires")

| # | Mot-clé secondaire | Intention |
|---|---|---|
| 1 | réservation infirmière brossard | transactionnelle |
| 2 | booking infirmière rive-sud en ligne | transactionnelle |
| 3 | prendre rendez-vous soins infirmiers | transactionnelle |
| 4 | prise rendez-vous prélèvement sanguin domicile | transactionnelle / locale |

---

## 6. Liens internes — Récapitulatif

| Lien dans la page | Texte d'ancre | Page de destination |
|---|---|---|
| Lien dans le formulaire de réservation | (579) 957-9690 | tel:+15799579690 |
| Lien ajouté en bas de page | Consulter nos tarifs | https://equipesanteplus.ca/prix/ |
| Lien ajouté en bas de page | Lire la FAQ | https://equipesanteplus.ca/faq/ |
| Lien ajouté en bas de page | Nous contacter | https://equipesanteplus.ca/contact/ |

---

## 7. Checklist de déploiement final

- [ ] HTML collé dans le widget Elementor et sauvegardé
- [ ] Vérifier que l'iframe Medexa se charge correctement après déploiement
- [ ] Keyphrase cible saisie dans Yoast : `rendez-vous infirmière à domicile longueuil`
- [ ] Titre SEO saisi (vérifier compteur — max 60 car.)
- [ ] Méta description saisie (vérifier compteur — 140 à 160 car.)
- [ ] Slug vérifié : `/rendez-vous/`
- [ ] Image OG uploadée dans l'onglet Réseaux sociaux de Yoast
- [ ] Keyphrases secondaires saisies
- [ ] Page publiée et testée sur mobile (iframe doit être fonctionnel)
- [ ] URL soumise dans Google Search Console → "Demander l'indexation"
- [ ] Résultat Yoast : minimum 4 feux verts sur 5 indicateurs principaux
