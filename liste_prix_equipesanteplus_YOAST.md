# Yoast SEO — Page Liste des Prix
**URL de la page :** https://equipesanteplus.ca/prix/
**Langue :** fr-CA
**Date :** 2026-03-06

---

## 1. Onglet SEO — Champs à remplir dans Yoast

> Accès : WordPress Admin → Pages → Prix → Yoast SEO (en bas de l'éditeur) → Onglet "SEO"

| Champ Yoast | Valeur à saisir |
|---|---|
| **Keyphrase cible** | prix infirmière à domicile rive-sud |
| **Titre SEO** | Prix Infirmière à Domicile Rive-Sud \| Tarifs Équipe Santé+ |
| **Slug (permalien)** | prix |
| **Méta description** | Tarifs transparents pour soins infirmiers à domicile Rive-Sud : prélèvements 90$, lavage d'oreille 85$, médicaments 60$, glycémie 50$. Aucun frais caché. Longueuil, Brossard, Saint-Hubert. |

**Aperçu Google attendu :**
```
Prix Infirmière à Domicile Rive-Sud | Tarifs Équipe Santé+
https://equipesanteplus.ca/prix/
Tarifs transparents pour soins infirmiers à domicile Rive-Sud : prélèvements 90$, lavage d'oreille 85$, médicaments 60$, glycémie 50$. Aucun frais caché. Longueuil, Brossard, Saint-Hubert.
```

---

## 2. Onglet SEO — Analyse de lisibilité et SEO (Yoast)

| Indicateur Yoast | Statut attendu | Action si rouge |
|---|---|---|
| Keyphrase dans le titre SEO | 🟢 Vert | "Prix Infirmière à Domicile Rive-Sud" présent |
| Keyphrase dans la méta description | 🟢 Vert | "soins infirmiers à domicile Rive-Sud" présent |
| Keyphrase dans le H1 | 🟡 Orange | H1 = "Liste de prix détaillée" — acceptable |
| Keyphrase dans l'introduction | 🟢 Vert | Sous-titre contient "soins infirmiers à domicile sur la Rive-Sud" |
| Densité de keyphrase (0.5–3%) | 🟢 Vert | Keyphrase présente dans les catégories de prix |
| Longueur du texte (>900 mots) | 🟢 Vert | Page très longue avec tableau de prix complet |
| Liens internes | 🟢 Vert | 4 liens internes (Contact, Rendez-vous, FAQ, Prélèvements) |
| Liens sortants | 🟢 Vert | Lien /contact/ présent dans le CTA |
| Alt text images | 🟢 Vert | Aucune image — emojis utilisés comme icônes |

> **Note** : Le schéma **Offer + PriceSpecification** est en place pour 5 services. Google peut afficher les prix directement dans les résultats de recherche.

---

## 3. Onglet "Réseaux sociaux" — Open Graph & Twitter Card

### Facebook / Open Graph
| Champ | Valeur à saisir |
|---|---|
| **Titre OG** | Tarifs Infirmière à Domicile — Transparent et Sans Surprise |
| **Description OG** | Prélèvements 90$, lavage d'oreille 85$, administration médicaments 60$, glycémie 50$. Déplacement inclus sur toute la Rive-Sud. Équipe Santé+ — soins à domicile professionnels. |
| **Image OG** | Utiliser une photo de service ou le logo — dimensions : **1200 × 630 px** |

### Twitter / X Card
| Champ | Valeur à saisir |
|---|---|
| **Type de carte** | `summary_large_image` |
| **Titre Twitter** | Prix Infirmière à Domicile Rive-Sud |
| **Description Twitter** | Tarifs transparents : prélèvements 90$, lavage oreille 85$, médicaments 60$, glycémie 50$. Déplacement inclus. |
| **Image Twitter** | Même image que OG (1200 × 630 px) |

---

## 4. Schema.org ajouté dans le HTML

| Propriété | Valeur |
|---|---|
| **Type principal** | `MedicalBusiness` + `Offer` (×4) |
| **Champs remplis** | name, priceCurrency, price, priceSpecification, seller |
| **Services avec prix** | Prélèvements (90$), Lavage d'oreille (85$), Médicaments (60$), Glycémie (50$) |
| **Où dans le HTML** | Script JSON-LD en bas de page |

---

## 5. Mots-clés secondaires (à intégrer dans Yoast — champ "Keyphrases secondaires")

| # | Mot-clé secondaire | Intention |
|---|---|---|
| 1 | tarif prélèvement sanguin longueuil | transactionnelle |
| 2 | coût lavage oreille à domicile | transactionnelle |
| 3 | infirmière privée prix brossard | transactionnelle |
| 4 | soins infirmiers tarif rive-sud | transactionnelle / locale |

---

## 6. Liens internes — Récapitulatif

| Lien dans la page | Texte d'ancre | Page de destination |
|---|---|---|
| Lien dans le Hero | Obtenir un devis | https://equipesanteplus.ca/contact/ |
| Lien dans le CTA | Nous contacter | https://equipesanteplus.ca/contact/ |
| Lien ajouté en bas de page | Prendre rendez-vous | https://equipesanteplus.ca/rendez-vous/ |
| Lien ajouté en bas de page | Questions fréquentes | https://equipesanteplus.ca/faq/ |
| Lien ajouté en bas de page | En savoir plus sur les prélèvements | https://equipesanteplus.ca/soins/prelevements/ |

---

## 7. Checklist de déploiement final

- [ ] HTML collé dans le widget Elementor et sauvegardé
- [ ] Keyphrase cible saisie dans Yoast : `prix infirmière à domicile rive-sud`
- [ ] Titre SEO saisi (vérifier compteur — max 60 car.)
- [ ] Méta description saisie (vérifier compteur — 140 à 160 car.)
- [ ] Slug vérifié : `/prix/`
- [ ] Image OG uploadée dans l'onglet Réseaux sociaux de Yoast
- [ ] Keyphrases secondaires saisies
- [ ] Page publiée et testée sur mobile
- [ ] Vérifier l'affichage des prix enrichis dans Google Search Console après indexation
- [ ] URL soumise dans Google Search Console → "Demander l'indexation"
- [ ] Résultat Yoast : minimum 4 feux verts sur 5 indicateurs principaux
