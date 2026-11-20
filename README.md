# Observatoire du Web des Artisans & TPE en France (2026–2027)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24284538.svg)](https://doi.org/10.5281/zenodo.24284538)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

Données ouvertes et rapports empiriques mesurant la présence en ligne, la capacité à recevoir des demandes de devis, la visibilité sur Google / moteurs IA (GEO) et la conformité légale (RGPD / LCEN) des artisans et TPE françaises.

- **Portail Web GitHub Pages :** [https://snipe91.github.io/observatoire-web-artisans-france/](https://snipe91.github.io/observatoire-web-artisans-france/)
- **Portail général des études :** [https://sitedigitalpro.com/etudes/](https://sitedigitalpro.com/etudes/)

---

## 3 Études Empiriques Publiées (CC-BY-4.0)

### 1. Baromètre des sites d'artisans du bâtiment (1 030 sites chargés en navigateur réel)
- **Méthode :** 1 030 sites français chargés dans un navigateur réel (inspection du DOM rendu, marge d'erreur ± 2,6 pts à IC 95 %, mesure du 29 septembre 2026).
- **Chiffres clés :** `77,3 %` sans données structurées `Schema.org` métier, `40,4 %` sans numéro de téléphone cliquable sur mobile (`tel:`), `63,8 %` sans politique de confidentialité, `83,2 %` sans `/llms.txt`.
- **Étude complète :** [https://sitedigitalpro.com/barometre-artisans-batiment/](https://sitedigitalpro.com/barometre-artisans-batiment/)
- **Rapport Markdown :** [barometre_artisans_1030_rapport_scientifique.md](./barometre_artisans_1030_rapport_scientifique.md)
- **Données brutes :** [barometre-indicateurs.csv](./data/barometre-indicateurs.csv) · [barometre-par-metier.csv](./data/barometre-par-metier.csv) · [LISEZ-MOI.txt](./data/LISEZ-MOI.txt)

### 2. Baromètre TPE France (600 entreprises issues d'OpenStreetMap)
- **Chiffres clés :** `52,9 %` sans politique de confidentialité, `34,6 %` sans mentions légales LCEN, `21,5 %` de sites indisponibles techniquement.
- **Étude complète :** [https://sitedigitalpro.com/barometre-tpe-2026/](https://sitedigitalpro.com/barometre-tpe-2026/)
- **Archive Zenodo (CERN) :** [https://zenodo.org/records/24284538](https://zenodo.org/records/24284538) (DOI [`10.5281/zenodo.24284538`](https://doi.org/10.5281/zenodo.24284538))
- **Rapport Markdown :** [barometre_tpe_2026_rapport_scientifique.md](./barometre_tpe_2026_rapport_scientifique.md)
- **Données brutes :** [barometre_tpe_2026_indicateurs_cles.csv](./data/barometre_tpe_2026_indicateurs_cles.csv) · [barometre_tpe_2026_repartition_sectorielle.csv](./data/barometre_tpe_2026_repartition_sectorielle.csv)

### 3. Baromètre des sanctions CNIL en France (2011–2026, 395 décisions)
- **Chiffres clés :** `1 118 238 301 €` cumulés, `81,1 %` des montants liés aux cookies/traceurs (`907 074 000 €`), `35,4 %` des dossiers liés à la sécurité/violation de données (`140` dossiers), amende médiane `15 000 €`.
- **Étude complète :** [https://sitedigitalpro.com/barometre-sanctions-cnil/](https://sitedigitalpro.com/barometre-sanctions-cnil/)
- **Rapport Markdown :** [barometre_sanctions_cnil_395_rapport_scientifique.md](./barometre_sanctions_cnil_395_rapport_scientifique.md)
- **Données brutes :** [barometre_sanctions_cnil_2011_2026_395.csv](./data/barometre_sanctions_cnil_2011_2026_395.csv)

---

## Ressources & Outils Gratuits Associés

- [Création de site internet pour artisans du bâtiment](https://sitedigitalpro.com/creation-site-web-artisan/)
- [Forfaits transparents et propriété WordPress](https://sitedigitalpro.com/nos-forfaits/)
- [Mise en conformité RGPD d'un site web](https://sitedigitalpro.com/mise-en-conformite-rgpd/)
- [Scanner gratuit de conformité RGPD (rgpd-audit.com)](https://rgpd-audit.com)
- [Test gratuit de visibilité Google & IA](https://sitedigitalpro.com/test-visibilite-site/)

---

## Contenu du dépôt

- [barometre_tpe_2026_rapport_scientifique.md](./barometre_tpe_2026_rapport_scientifique.md)
- [barometre_artisans_1030_rapport_scientifique.md](./barometre_artisans_1030_rapport_scientifique.md)
- [barometre_sanctions_cnil_395_rapport_scientifique.md](./barometre_sanctions_cnil_395_rapport_scientifique.md)
- [data/](./data/) (`barometre-par-metier.csv`, `barometre-indicateurs.csv`, `LISEZ-MOI.txt`, `barometre_tpe_2026_indicateurs_cles.csv`, `barometre_tpe_2026_repartition_sectorielle.csv`, `barometre_sanctions_cnil_2011_2026_395.csv`)
