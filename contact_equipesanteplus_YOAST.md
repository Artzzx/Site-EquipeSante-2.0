# Yoast SEO — Page Contact
**URL de la page :** https://equipesanteplus.ca/contact/
**Langue :** fr-CA
**Date :** 2026-03-06

---

## 1. Onglet SEO — Champs à remplir dans Yoast

> Accès : WordPress Admin → Pages → Contact → Yoast SEO (en bas de l'éditeur) → Onglet "SEO"

| Champ Yoast | Valeur à saisir |
|---|---|
| **Keyphrase cible** | contact infirmière longueuil |
| **Titre SEO** | Contact Infirmière à Domicile – Rive-Sud \| Équipe Santé+ |
| **Slug (permalien)** | contact |
| **Méta description** | Contactez Équipe Santé+ pour vos soins infirmiers à domicile sur la Rive-Sud. Appelez le 579-957-9690 ou écrivez-nous — réponse rapide, service 7j/7 à Longueuil, Brossard et environs. |

**Aperçu Google attendu :**
```
Contact Infirmière à Domicile – Rive-Sud | Équipe Santé+
https://equipesanteplus.ca/contact/
Contactez Équipe Santé+ pour vos soins infirmiers à domicile sur la Rive-Sud. Appelez le 579-957-9690 ou écrivez-nous — réponse rapide, service 7j/7 à Longueuil, Brossard et environs.
```

---

## 2. Onglet SEO — Analyse de lisibilité et SEO (Yoast)

| Indicateur Yoast | Statut attendu | Action si rouge |
|---|---|---|
| Keyphrase dans le titre SEO | 🟢 Vert | Le titre contient "Infirmière" et "Rive-Sud" |
| Keyphrase dans la méta description | 🟢 Vert | "Infirmière à domicile" présent dans la méta |
| Keyphrase dans le H1 | 🟡 Orange | H1 actuel = "Contactez-nous" — keyphrase indirecte acceptable |
| Keyphrase dans l'introduction | 🟢 Vert | Sous-titre contient "soins infirmiers à domicile" |
| Densité de keyphrase (0.5–3%) | 🟢 Vert | Keyphrase présente naturellement, pas sur-optimisée |
| Longueur du texte (>900 mots) | 🟡 Orange | Page formulaire courte — acceptable pour une page de contact |
| Liens internes | 🟢 Vert | 3 liens internes ajoutés (FAQ, Prix, Rendez-vous) |
| Liens sortants | 🟢 Vert | Lien mailto et tel présents |
| Alt text images | 🟢 Vert | Aucune image — SVG décoratifs marqués aria-hidden |

---

## 3. Onglet "Réseaux sociaux" — Open Graph & Twitter Card

### Facebook / Open Graph
| Champ | Valeur à saisir |
|---|---|
| **Titre OG** | Contactez Équipe Santé+ — Infirmière à Domicile Rive-Sud |
| **Description OG** | Une question ? Un rendez-vous à planifier ? Appelez le 579-957-9690 ou envoyez-nous un message. Soins infirmiers à domicile à Longueuil, Brossard, Saint-Hubert et toute la Rive-Sud. |
| **Image OG** | Utiliser une photo de l'équipe ou du logo — dimensions : **1200 × 630 px** |

### Twitter / X Card
| Champ | Valeur à saisir |
|---|---|
| **Type de carte** | `summary_large_image` |
| **Titre Twitter** | Contact — Infirmière à Domicile Rive-Sud |
| **Description Twitter** | Appelez le 579-957-9690 ou écrivez-nous. Soins infirmiers à domicile 7j/7 à Longueuil et Rive-Sud. |
| **Image Twitter** | Même image que OG (1200 × 630 px) |

---

## 4. Schema.org ajouté dans le HTML

| Propriété | Valeur |
|---|---|
| **Type principal** | `schema.org/ContactPage` |
| **Type imbriqué** | `schema.org/MedicalBusiness` |
| **Champs remplis** | name, telephone, description, url, address (addressRegion, addressCountry) |
| **Où dans le HTML** | Script JSON-LD en bas de page |

---

## 5. Mots-clés secondaires (à intégrer dans Yoast — champ "Keyphrases secondaires")

| # | Mot-clé secondaire | Intention |
|---|---|---|
| 1 | infirmière rive-sud téléphone | transactionnelle / locale |
| 2 | rendez-vous infirmière brossard | transactionnelle |
| 3 | joindre infirmière à domicile | transactionnelle |
| 4 | soins infirmiers contact saint-hubert | locale |

---

## 6. Liens internes — Récapitulatif

| Lien dans la page | Texte d'ancre | Page de destination |
|---|---|---|
| Lien ajouté en bas de page | nos questions fréquentes | https://equipesanteplus.ca/faq/ |
| Lien ajouté en bas de page | notre liste de prix | https://equipesanteplus.ca/prix/ |
| Lien ajouté en bas de page | prenez rendez-vous en ligne | https://equipesanteplus.ca/rendez-vous/ |

---

## 7. Checklist de déploiement final

- [ ] HTML collé dans le widget Elementor et sauvegardé
- [ ] Keyphrase cible saisie dans Yoast : `contact infirmière longueuil`
- [ ] Titre SEO saisi (vérifier compteur — max 60 car.)
- [ ] Méta description saisie (vérifier compteur — 140 à 160 car.)
- [ ] Slug vérifié : `/contact/`
- [ ] Image OG uploadée dans l'onglet Réseaux sociaux de Yoast
- [ ] Keyphrases secondaires saisies
- [ ] Page publiée et testée sur mobile
- [ ] URL soumise dans Google Search Console → "Demander l'indexation"
- [ ] Résultat Yoast : minimum 4 feux verts sur 5 indicateurs principaux
