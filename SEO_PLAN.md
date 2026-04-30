# SEO_PLAN — Équipe Santé+ (Yoast SEO 2.0)

**Site :** https://equipesanteplus.ca/
**Activité :** Soins infirmiers à domicile, Rive-Sud de Montréal (Montérégie) — B2C
**Audience :** Familles francophones de la Rive-Sud cherchant des soins à domicile pour aînés ou patients post-opératoires
**Langue principale :** fr-CA
**Date :** 2026-04-30

> Format Yoast 2.0 : un bloc par page HTML scannée dans le repo.
> SEO Title ≤ 60 car. (suffixe « | Équipe Santé+ » inclus). Méta description 140–155 car. en français.
> Slugs lowercase, hyphens, sans accents (compatibles WordPress).

---

## Page_all_soins.html
**Focus Keyphrase :** soins infirmiers à domicile rive-sud
**SEO Title :** Soins Infirmiers à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Soins infirmiers à domicile sur la Rive-Sud : prélèvements, glycémie, plaies, pieds, médicaments. Infirmière OIIQ à Longueuil, Brossard, Saint-Hubert.
**Slug :** soins-infirmier
**Cornerstone :** Yes
**Action Steps :**
- [ ] Page hub des services — déclarer comme « Cornerstone content » dans Yoast
- [ ] H1 actuel `Nos Services de Soins Infirmiers à Domicile` → ajouter « Rive-Sud » pour ancrer la keyphrase localement
- [ ] Vérifier que chaque carte de service contient un lien interne `<a href>` vers la page enfant correspondante (audit des 17 sous-pages)
- [ ] Ajouter `BreadcrumbList` JSON-LD (Accueil › Services)
- [ ] Mettre à jour le bloc JSON-LD existant en `MedicalBusiness` + `OfferCatalog` listant les `MedicalProcedure` enfants
- [ ] Ajouter texte d'introduction (100-150 mots) au-dessus de la grille pour atteindre le seuil de mots Yoast et inclure la keyphrase dans les 100 premiers mots
- [ ] Vérifier les attributs `alt` sur les icônes/images de cartes de service (descriptifs, pas vides)
- [ ] Ajouter au moins un lien sortant d'autorité (ex : OIIQ, gouvernement du Québec)

---

## contact_equipesanteplus.html
**Focus Keyphrase :** contact infirmière à domicile rive-sud
**SEO Title :** Contact Infirmière à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Contactez Équipe Santé+ pour des soins infirmiers à domicile sur la Rive-Sud. Téléphone 579-957-9690, formulaire en ligne, réponse rapide 7j/7.
**Slug :** contact
**Cornerstone :** No
**Action Steps :**
- [ ] Fichier livré comme widget Elementor (sans `<title>`/`<meta>`) — saisir titre/méta dans Yoast WordPress
- [ ] H1 actuel `Contactez-nous` → conserver tel quel (intent transactionnel clair) ; la keyphrase reste indirecte mais acceptée
- [ ] Vérifier que le numéro de téléphone est dans `<a href="tel:+15799579690">` (et non en texte brut)
- [ ] Vérifier que l'email est dans `<a href="mailto:...">`
- [ ] Confirmer le bloc JSON-LD `ContactPage` + `MedicalBusiness` (présent — vérifier `telephone`, `address.addressRegion=QC`, `areaServed`)
- [ ] Ajouter un sous-titre ou paragraphe intro contenant « infirmière à domicile Rive-Sud » dans les 100 premiers mots
- [ ] Vérifier les 3 liens internes existants (FAQ, Prix, Rendez-vous)
- [ ] Marquer les SVG décoratifs avec `aria-hidden="true"`

---

## faq_equipesanteplus.html
**Focus Keyphrase :** faq soins infirmiers à domicile
**SEO Title :** FAQ Soins Infirmiers à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Questions fréquentes sur nos soins infirmiers à domicile : tarifs, ordonnances, zones desservies, déroulement. Réponses claires pour la Rive-Sud.
**Slug :** faq
**Cornerstone :** No
**Action Steps :**
- [ ] Fichier livré comme widget Elementor — saisir titre/méta dans Yoast
- [ ] H1 actuel `Foire aux questions` → remplacer par `Foire aux questions sur les soins infirmiers à domicile` pour intégrer la keyphrase
- [ ] Confirmer le JSON-LD `FAQPage` (présent — vérifier que CHAQUE accordion correspond à un objet `Question`/`acceptedAnswer` complet)
- [ ] Vérifier que le contenu textuel des réponses dans le JSON-LD correspond exactement au DOM visible (sinon Google rejette le rich snippet)
- [ ] Ajouter au moins 3 liens internes contextuels dans les réponses (vers services pertinents : prélèvements, soins de pieds, post-opératoires)
- [ ] Ajouter un sous-titre H2 introductif contenant la keyphrase
- [ ] Vérifier `aria-expanded` et `aria-controls` sur les boutons d'accordion (accessibilité + crawlabilité)

---

## header.html
**Focus Keyphrase :** N/A (composant partagé, non-indexable)
**SEO Title :** N/A
**Meta Description :** N/A
**Slug :** N/A
**Cornerstone :** No
**Action Steps :**
- [ ] Composant de navigation réutilisable — exclure de l'indexation (pas une page WordPress)
- [ ] Vérifier que le `<img>` du logo a un `alt="Équipe Santé+ — Soins infirmiers à domicile Rive-Sud"`
- [ ] Vérifier que les liens de menu utilisent les slugs définitifs listés dans ce plan
- [ ] Le `<title>` interne `Header - Équipe Santé+` est sans effet (jamais rendu en page complète) — laisser tel quel
- [ ] S'assurer que le numéro de téléphone du menu est dans `<a href="tel:...">`
- [ ] Ajouter `aria-label="Navigation principale"` sur le `<nav>`

---

## home_page_equipesanteplus_v2.html
**Focus Keyphrase :** infirmière à domicile rive-sud
**SEO Title :** Infirmière à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Infirmière à domicile sur la Rive-Sud : prélèvements, soins de pieds, médicaments, suivi post-op. Service professionnel 7j/7 à Longueuil et Brossard.
**Slug :** (racine — aucun slug)
**Cornerstone :** Yes
**Action Steps :**
- [ ] Déclarer comme « Cornerstone content » dans Yoast (page d'accueil)
- [ ] H1 actuel `Équipe Santé+ | Soins Infirmiers à Domicile` → simplifier en `Infirmière à Domicile sur la Rive-Sud` pour matcher la keyphrase exacte
- [ ] Conserver le balisage `MedicalBusiness` + `LocalBusiness` JSON-LD ; vérifier `geo`, `areaServed` (liste explicite des villes), `openingHoursSpecification`
- [ ] Vérifier que les 3 `<img>` ont des `alt` descriptifs en français (ex : pas « image1.webp » mais « Infirmière effectuant un prélèvement à domicile »)
- [ ] Corriger la balise OG ouverte non fermée ligne 26 : `<meta property="og:site_name" content="Équipe Santé+"` manque le `>` final
- [ ] Corriger l'ordre logique des H2 (vérifier qu'aucun H3 n'apparaît avant son H2 parent)
- [ ] Confirmer présence d'au moins 5 liens internes vers les pages de service principales
- [ ] Ajouter un lien sortant d'autorité (OIIQ ou Santé Québec)
- [ ] Vérifier que l'image OG `IMG_5030.webp` est en 1200×630 px

---

## liste_prix_equipesanteplus.html
**Focus Keyphrase :** prix soins infirmiers à domicile
**SEO Title :** Prix Soins Infirmiers à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Tarifs transparents pour soins infirmiers à domicile sur la Rive-Sud : prélèvement 90$, glycémie 50$, lavage oreille 85$. Sans frais cachés.
**Slug :** prix
**Cornerstone :** No
**Action Steps :**
- [ ] Fichier livré comme widget Elementor — saisir titre/méta dans Yoast
- [ ] H1 actuel `Liste de prix détaillée` → remplacer par `Liste de prix des soins infirmiers à domicile` (intègre la keyphrase)
- [ ] Confirmer le JSON-LD `OfferCatalog` ou `PriceSpecification` ; chaque prix doit avoir `priceCurrency: CAD` et un `Offer.itemOffered.@type: MedicalProcedure`
- [ ] Vérifier que chaque ligne tarifaire pointe en lien interne vers la page de service correspondante
- [ ] Ajouter un paragraphe introductif (~100 mots) avec la keyphrase dans les 100 premiers mots
- [ ] Marquer SVG décoratifs `aria-hidden="true"`
- [ ] Vérifier liens internes (FAQ, Rendez-vous, Contact) en bas de page

---

## rendez_vous_equipesanteplus.html
**Focus Keyphrase :** prendre rendez-vous infirmière à domicile
**SEO Title :** Rendez-vous Infirmière à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Prenez rendez-vous en ligne avec une infirmière à domicile sur la Rive-Sud. Réservation simple en 4 étapes, confirmation rapide, soins 7j/7.
**Slug :** rendez-vous
**Cornerstone :** No
**Action Steps :**
- [ ] Fichier livré comme widget Elementor — saisir titre/méta dans Yoast
- [ ] H1 actuel `Prenez rendez-vous en ligne` → ajouter `avec une infirmière à domicile` pour la keyphrase
- [ ] Confirmer le JSON-LD `ReserveAction` (présent) — vérifier `target.urlTemplate` et `result.@type: Reservation`
- [ ] Si l'iframe de réservation est tiers, vérifier `title` sur l'iframe pour l'accessibilité
- [ ] Ajouter un H2 contenant la keyphrase dans la section « Comment ça fonctionne »
- [ ] Vérifier qu'au moins 3 liens internes pointent vers Services, Prix, FAQ
- [ ] Marquer SVG décoratifs `aria-hidden="true"`

---

## soins/prelèvements.html
**Focus Keyphrase :** prélèvement sanguin à domicile
**SEO Title :** Prélèvement Sanguin à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Prélèvement sanguin à domicile sur la Rive-Sud par infirmière OIIQ. Sans douleur, résultats en 24-48h, à Longueuil, Brossard, Saint-Hubert. Dès 90$.
**Slug :** soins/prelevements
**Cornerstone :** Yes
**Action Steps :**
- [ ] Renommer le fichier `prelèvements.html` → `prelevements.html` (les caractères accentués dans une URL ou nom de fichier cassent les déploiements WordPress)
- [ ] Déclarer comme Cornerstone (service à fort volume)
- [ ] Ajouter un bloc JSON-LD `MedicalProcedure` complet (actuellement absent — la page utilise du microdata `itemscope` seulement) : `name`, `description`, `procedureType`, `bodyLocation`, `provider` (`MedicalBusiness`)
- [ ] H1 `Prélèvements à Domicile` → reformuler en `Prélèvement Sanguin à Domicile` pour la correspondance exacte de la keyphrase
- [ ] Le titre actuel `Prélèvements Sanguins à Domicile Longueuil | Prise de Sang Rive-Sud 90$` (66 car.) dépasse 60 — remplacer par la valeur ci-dessus
- [ ] Vérifier que la keyphrase apparaît dans le premier paragraphe de la page
- [ ] Ajouter au moins 3 liens internes contextuels (glycémie, soins post-op, contact)
- [ ] Vérifier `aria-hidden="true"` sur tous les SVG décoratifs

---

## soins/service_accompagnement_aines.html
**Focus Keyphrase :** accompagnement aînés à domicile
**SEO Title :** Accompagnement Aînés à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Accompagnement des aînés à domicile sur la Rive-Sud : présence bienveillante, sorties, soutien quotidien. Briser l'isolement à Longueuil et Brossard.
**Slug :** soins/accompagnement-aines
**Cornerstone :** No
**Action Steps :**
- [ ] Fichier livré comme widget Elementor — saisir titre/méta dans Yoast
- [ ] H1 `Accompagnement des Aînés à Domicile` → conserver (correspondance forte avec la keyphrase)
- [ ] Ajouter un bloc JSON-LD : combiner `Service` (déjà en microdata) + `MedicalBusiness` provider en JSON-LD pour cohérence
- [ ] Vérifier que la keyphrase apparaît au moins 1× dans le premier paragraphe
- [ ] Ajouter 3 liens internes (administration médicaments, soins de pieds, contact)
- [ ] Cas particulier : ce service n'est pas un acte médical mais un service d'accompagnement — utiliser `Service` + `serviceType="Elderly companionship"`, PAS `MedicalProcedure`
- [ ] Vérifier alt-text sur les visuels de section témoignages
- [ ] Marquer SVG décoratifs `aria-hidden="true"`

---

## soins/service_administration_medicaments.html
**Focus Keyphrase :** administration de médicaments à domicile
**SEO Title :** Administration Médicaments à Domicile | Équipe Santé+
**Meta Description :** Administration de médicaments à domicile par infirmière OIIQ : injections, pilulier, suivi. Sécuritaire et professionnel sur la Rive-Sud. Dès 60$.
**Slug :** soins/administration-medicaments
**Cornerstone :** No
**Action Steps :**
- [ ] Le titre actuel `Administration de Médicaments à Domicile | Infirmière Longueuil 60$` (66 car.) dépasse 60 — remplacer par la valeur ci-dessus
- [ ] Ajouter un bloc JSON-LD `MedicalProcedure` complet (actuellement absent — microdata seul) avec `procedureType`, `provider`
- [ ] H1 conserver tel quel (correspond à la keyphrase)
- [ ] Vérifier que la keyphrase exacte « administration de médicaments à domicile » apparaît dans les 100 premiers mots
- [ ] Ajouter 3 liens internes (prélèvements, soins post-op, prix)
- [ ] Marquer SVG décoratifs `aria-hidden="true"`
- [ ] Vérifier la hiérarchie H2 → H3 (aucun saut)

---

## soins/service_lavage_oreille.html
**Focus Keyphrase :** lavage d'oreille à domicile
**SEO Title :** Lavage d'Oreille à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Lavage d'oreille à domicile sur la Rive-Sud : retrait de bouchon de cérumen par infirmière qualifiée. Soulagement rapide à Longueuil. Dès 85$.
**Slug :** soins/lavage-oreille
**Cornerstone :** No
**Action Steps :**
- [ ] Le titre actuel `Lavage d'Oreille à Domicile Longueuil | Irrigation Auriculaire Rive-Sud 85$` (78 car.) dépasse 60 — remplacer par la valeur ci-dessus
- [ ] Ajouter un bloc JSON-LD `MedicalProcedure` complet (microdata seul actuellement) avec `bodyLocation: Ear`, `procedureType: TherapeuticProcedure`
- [ ] H1 conserver
- [ ] Vérifier que la keyphrase apparaît dans le premier paragraphe
- [ ] Ajouter 3 liens internes (soins courants, soins de pieds, contact)
- [ ] Vérifier section « Contre-indications » — bon signal E-E-A-T (montre l'expertise)
- [ ] Marquer SVG décoratifs `aria-hidden="true"`

---

## soins/service_prise_glycemie.html
**Focus Keyphrase :** prise de glycémie à domicile
**SEO Title :** Prise de Glycémie à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Prise de glycémie à domicile pour suivi du diabète sur la Rive-Sud. Mesure précise, enseignement, soins par infirmière OIIQ. Dès 50$.
**Slug :** soins/prise-glycemie
**Cornerstone :** No
**Action Steps :**
- [ ] Le titre actuel `Prise de Glycémie à Domicile Longueuil | Infirmière Diabète Rive-Sud 50$` (74 car.) dépasse 60 — remplacer par la valeur ci-dessus
- [ ] Ajouter un bloc JSON-LD `MedicalProcedure` complet (actuellement microdata seul) ; lier à `MedicalCondition: Diabetes`
- [ ] H1 conserver
- [ ] Vérifier la keyphrase dans le premier paragraphe
- [ ] Ajouter 3 liens internes (administration médicaments, prise de tension, soins de pieds — pertinent pour patients diabétiques)
- [ ] Confirmer que la section « Valeurs de glycémie » utilise un `<table>` sémantique (pas une grille CSS) pour rich snippet potentiel
- [ ] Marquer SVG décoratifs `aria-hidden="true"`

---

## soins/service_prise_tension_arterielle.html
**Focus Keyphrase :** prise de tension à domicile
**SEO Title :** Prise de Tension Artérielle à Domicile | Équipe Santé+
**Meta Description :** Prise de tension artérielle à domicile sur la Rive-Sud : signes vitaux, suivi cardiovasculaire, enseignement par infirmière OIIQ. Dès 50$.
**Slug :** soins/prise-tension-arterielle
**Cornerstone :** No
**Action Steps :**
- [ ] Fichier livré comme widget Elementor — saisir titre/méta dans Yoast
- [ ] H1 conserver `Prise de Tension Artérielle à Domicile`
- [ ] JSON-LD `MedicalProcedure` présent — vérifier `procedureType`, `bodyLocation`, `provider.@type: MedicalBusiness`
- [ ] Vérifier que la keyphrase apparaît dans le premier paragraphe
- [ ] Ajouter 3 liens internes (glycémie, soins courants, soins post-op)
- [ ] Tableau « Catégories de tension » → confirmer `<table>` HTML sémantique
- [ ] Vérifier hiérarchie H2 → H3 (30+ H3 mentionnés — auditer la structure)
- [ ] Marquer SVG décoratifs `aria-hidden="true"`

---

## soins/service_soins_courants.html
**Focus Keyphrase :** soins courants à domicile
**SEO Title :** Soins Courants à Domicile Rive-Sud | Équipe Santé+
**Meta Description :** Soins courants à domicile sur la Rive-Sud : infections urinaires, strep A, herpès labial via ordonnance collective par infirmière OIIQ. Dès 75$.
**Slug :** soins-infirmier/soins-courants
**Cornerstone :** No
**Action Steps :**
- [ ] Le titre actuel `Soins Courants à Domicile Longueuil | Infection Urinaire, Strep, Herpès | Équipe Santé+` (89 car.) dépasse 60 — remplacer par la valeur ci-dessus
- [ ] Slug canonique actuel `/soins-infirmier/soins-courant/` → corriger en `/soins-infirmier/soins-courants/` (pluriel cohérent avec le H1)
- [ ] H1 conserver
- [ ] JSON-LD `MedicalBusiness` + `OfferCatalog` présent — vérifier les 3 `MedicalProcedure` (UTI, Strep A, Herpès labial) avec `procedureType` et `code` (ICD si possible)
- [ ] Bonne page E-E-A-T (cite OIIQ, LII, INSPQ) — conserver ces liens sortants d'autorité
- [ ] Ajouter 3 liens internes (administration médicaments, prise de tension, contact)
- [ ] Marquer SVG décoratifs `aria-hidden="true"`

---

## soins/service_soins_drain.html
**Focus Keyphrase :** soins de drain à domicile
**SEO Title :** Soins de Drain Chirurgical à Domicile | Équipe Santé+
**Meta Description :** Soins et retrait de drain chirurgical (Jackson-Pratt, Hémovac) à domicile sur la Rive-Sud. Suivi post-op par infirmière OIIQ. Dès 85$.
**Slug :** soins/soins-drain-chirurgical
**Cornerstone :** No
**Action Steps :**
- [ ] Fichier livré comme widget Elementor — saisir titre/méta dans Yoast
- [ ] H1 conserver `Soins de Drain Chirurgical à Domicile`
- [ ] JSON-LD `MedicalProcedure` présent — vérifier `procedureType: SurgicalProcedure`, `bodyLocation`, `followup`
- [ ] Vérifier que la keyphrase apparaît dans le premier paragraphe
- [ ] Ajouter 3 liens internes contextuels (soins post-opératoires, soins courants, prélèvements)
- [ ] Section « Types de drainage : normal vs inquiétant » — utiliser un balisage `<table>` sémantique
- [ ] Marquer SVG décoratifs `aria-hidden="true"`

---

## soins/service_soins_post_operatoires.html
**Focus Keyphrase :** soins post-opératoires à domicile
**SEO Title :** Soins Post-Opératoires à Domicile | Équipe Santé+
**Meta Description :** Soins post-opératoires à domicile sur la Rive-Sud après chirurgie : plaie, drain, signes vitaux, retrait de sutures par infirmière OIIQ. Dès 110$.
**Slug :** soins/soins-post-operatoires
**Cornerstone :** Yes
**Action Steps :**
- [ ] Fichier livré comme widget Elementor — saisir titre/méta dans Yoast
- [ ] Déclarer comme Cornerstone (service à forte intention transactionnelle, audience post-chirurgie ciblée)
- [ ] H1 conserver `Soins Post-Opératoires à Domicile`
- [ ] Ajouter un bloc JSON-LD `MedicalProcedure` complet (actuellement absent) avec `procedureType: SurgicalProcedure` (suivi), `provider.@type: MedicalBusiness`
- [ ] Vérifier que la keyphrase apparaît dans le premier paragraphe
- [ ] Ajouter 3-5 liens internes contextuels (soins de drain, soins courants, prélèvements, administration médicaments)
- [ ] Section « Signes de complications à surveiller » → balisage liste `<ul>` clair pour rich snippet
- [ ] Marquer SVG décoratifs `aria-hidden="true"`

---

## soins/soins_de_pieds.html
**Focus Keyphrase :** soins de pieds à domicile
**SEO Title :** Soins de Pieds Infirmiers à Domicile Rive-Sud | É. Santé+
**Meta Description :** Soins de pieds infirmiers à domicile sur la Rive-Sud : pieds diabétiques, ongles incarnés, cors, callosités. Infirmière AIISPQ à Longueuil.
**Slug :** soins/soins-de-pieds
**Cornerstone :** Yes
**Action Steps :**
- [ ] Le titre actuel `Soins de Pieds Infirmiers à Domicile Longueuil | Pieds Diabétiques Rive-Sud` (78 car.) dépasse 60 — remplacer par la valeur ci-dessus (« É. Santé+ » abrégé pour rester ≤ 60 car.) OU utiliser `Soins de Pieds à Domicile Rive-Sud | Équipe Santé+` (51 car.) si on accepte de raccourcir le mot-clé en titre
- [ ] Déclarer comme Cornerstone (forte demande aînés + diabétiques sur la Rive-Sud)
- [ ] JSON-LD `MedicalProcedure` présent avec `BodyStructure: Pied` — vérifier la propriété `performer` mentionne AIISPQ
- [ ] H1 conserver `Soins de pieds infirmiers à domicile`
- [ ] Renforcer la « Distinction importante » (soins infirmiers vs esthétiques) — c'est un signal E-E-A-T fort
- [ ] Ajouter 3 liens internes (glycémie pour diabétiques, accompagnement aînés, contact)
- [ ] Vérifier le caractère `?` collé à `consulter ?` dans le H2 — conserver l'espace insécable français
- [ ] Marquer SVG décoratifs `aria-hidden="true"`

---

## Récapitulatif global

| Action transversale | Pages concernées |
|---|---|
| Pages déclarées **Cornerstone** | Accueil, Page_all_soins, Prélèvements, Soins post-opératoires, Soins de pieds |
| **Titles à raccourcir** (> 60 car.) | Prélèvements, Administration médicaments, Lavage oreille, Prise glycémie, Soins courants, Soins de pieds |
| **JSON-LD à ajouter** (microdata seul actuellement) | Prélèvements, Accompagnement aînés, Administration médicaments, Lavage oreille, Prise glycémie, Soins post-opératoires |
| **Pages widget Elementor** (titre/méta à saisir dans Yoast WP) | Contact, FAQ, Liste prix, Rendez-vous, toutes les pages `/soins/*` |
| **Renommage de fichier requis** | `prelèvements.html` → `prelevements.html` |
| **Liens internes à auditer** (objectif ≥ 3 par page) | Toutes |
| **Balisage `<table>` sémantique** | Glycémie, Tension artérielle, Soins de drain |
| **`aria-hidden="true"` sur SVG décoratifs** | Toutes |
