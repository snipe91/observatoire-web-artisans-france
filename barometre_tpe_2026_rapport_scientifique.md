# Baromètre 2026-2027 du Web des TPE et Artisans Français
## Analyse empirique de la conformité légale, de la sécurité RGPD et des performances techniques sur 600 établissements (France métropolitaine)

**Auteur :** Site Digital Pro (Stéphane Lueger — Observatoire Numérique des TPE & Artisans)  
**DOI Zenodo :** [10.5281/zenodo.24284538](https://doi.org/10.5281/zenodo.24284538)  
**Date d'observation :** Septembre - Novembre 2026  
**Échantillon :** 600 sites web d'artisans, commerçants et professions libérales en France métropolitaine  
**Corpus initial :** 8 653 domaines extraits de la base OpenStreetMap (données ouvertes géocodées)  
**Licence :** Creative Commons Attribution 4.0 International (CC-BY 4.0)  
**Source de référence :** [Site Digital Pro - Baromètre TPE 2026](https://sitedigitalpro.com/barometre-tpe-2026/)  
**Dépôt GitHub Open Data :** [snipe91/barometre-tpe-france](https://github.com/snipe91/barometre-tpe-france)

---

### Résumé Exécutif

Cette étude empirique documente l'état réel de conformité juridique (RGPD, LCEN) et de fiabilité technique des sites internet des Très Petites Entreprises (TPE) et artisans en France métropolitaine. Contrairement aux enquêtes déclaratives sur sondage, chaque résultat découle d'un audit automatisé direct par requêtes HTTP réelles, sans estimation théorique.

Les constats majeurs révèlent une vulnérabilité critique du tissu économique local :
- **52,9 % des sites audités** ne disposent d'aucune politique de confidentialité accessible, en violation directe des articles 12 et 13 du RGPD.
- **34,6 % des sites** omettent les mentions légales obligatoires prescrites par la loi pour la confiance dans l'économie numérique (LCEN).
- **21,5 % des établissements** possèdent un site indisponible (erreurs DNS, timeout serveur, erreurs 5xx ou 404).
- **81,1 % du montant cumulé des amendes CNIL** (plus de 907 millions d'euros sur un total de 1,118 milliard entre 2011 et 2026) sanctionnent la gestion illicite des cookies et traceurs sans consentement préalable.

Cette étude analyse l'impact direct de ces carences sur le déclassement dans le Pack Local de Google et sur l'exclusion par les moteurs de recherche à intelligence artificielle générative (**GEO** : Generative Engine Optimization sur ChatGPT Search, Perplexity et Google AI Overviews).

---

### 1. Méthodologie et Protocole de Collecte

#### 1.1 Source des données et sélection
Le corpus d'étude a été extrait de la base géographique collaborative **OpenStreetMap (OSM)**, filtré sur les nœuds et polygones situés en France métropolitaine portant :
1. Une activité commerciale, artisanale ou libérale vérifiée (`shop=*`, `craft=*`, `amenity=*`, `office=*`).
2. Une URL de site internet déclarée (`website=*`).
3. Un ancrage national prouvé (code pays FR, présence d'un numéro SIRET public ou extension de domaine en `.fr`).

Sur un ensemble de **8 653 domaines uniques**, un échantillonnage aléatoire stratifié de **600 sites web** a été constitué pour analyse exhaustive.

#### 1.2 Répartition sectorielle de l'échantillon
- Soins et bien-être (Instituts de beauté : 91, Coiffeurs : 78) : 169 sites (28,2 %)
- Commerces de bouche (Boulangeries : 68, Boucheries : 43) : 111 sites (18,5 %)
- Artisans du bâtiment (Menuisiers : 27, Fabricants de fenêtres : 25, Chauffagistes : 21, Ébénistes : 21, Plombiers : 18, Maçons : 18) : 130 sites (21,7 %)
- Santé et paramédical (Opticiens : 67) : 67 sites (11,2 %)
- Services de proximité et autres (Fleuristes : 38, Métiers d'art : 85) : 123 sites (20,5 %)

#### 1.3 Métriques techniques collectées
Pour chaque domaine, une série de requêtes programmées a inspecté :
- La résolution DNS et la connectivité réseau (codes d'état HTTP).
- Le protocole de chiffrement (HTTP vs HTTPS) et la validité cryptographique du certificat TLS/SSL.
- La présence d'une balise d'adaptation mobile (`<meta name="viewport">`).
- L'existence et l'accessibilité des mentions légales (`/mentions-legales/`, ancre textuelle, présence des mentions d'hébergeur et d'immatriculation).
- L'existence d'une politique de traitement des données personnelles (politique de confidentialité conforme RGPD).
- Le poids de la charge utile HTML initiale (hors assets externes) et la latence de premier octet (TTFB / latence de réponse).

---

### 2. Résultats Empiriques Clés

| Indicateur Technique & Juridique | Résultat Empirique | Interprétation pour l'Entreprise |
|---|---|---|
| **Disponibilité effective** | **78,5 %** (471 / 600) | **21,5 % des sites sont inopérants** (domaine expiré, erreur serveur ou page introuvable). |
| **Chiffrement HTTPS** | **97,7 %** des répondants | Le cadenas est généralisé, mais 2,3 % naviguent encore en HTTP non sécurisé. |
| **Adaptation mobile (Viewport)** | **95,5 %** | Standard technique largement assimilé. |
| **Mentions Légales (LCEN)** | **65,4 %** | **34,6 % d'absence totale** : infraction pénale passible d'un an d'emprisonnement et 75 000 € d'amende (Art. 6-VI LCEN). |
| **Politique de Confidentialité (RGPD)** | **47,1 %** | **52,9 % d'infraction RGPD** : recueil de données (formulaires, statistiques) sans base légale explicite. |
| **Poids HTML Médian** | **115,4 Ko** | Poids raisonnable, mais de fortes disparités constatées sur les constructeurs de pages lourds. |
| **Temps de Réponse Médian** | **0,93 seconde** | Réponse médiane correcte, mais moyenne dégradée à 1,44 seconde. |

---

### 3. Analyse Juridique : Risques et Sanctions CNIL (2011-2026)

L'étude a croisé les données de terrain avec l'historique complet des **395 sanctions publiques prononcées par la CNIL** entre 2011 et 2026 (montant cumulé : **1 118 238 301 €**) :

1. **Le piège des cookies et traceurs illicites :**  
   Les manquements relatifs au consentement préalable sur les traceurs représentent **907 074 000 € (81,1 % du montant financier total des sanctions)**. Une majorité écrasante des TPE audités utilise des scripts tiers (Google Analytics sans consentement, pixels publicitaires, plugins sociaux) déposant des cookies dès l'arrivée du visiteur sans possibilité de refus égal.

2. **La sécurité et la violation de données :**  
   Motif de contrôle le plus fréquent en nombre de dossiers (**140 dossiers sur 395, soit 35,4 %**). Les TPE utilisant des CMS non mis à jour ou des formulaires sans chiffrement exposent les données clients aux fuites automatisées.

---

### 4. Impact sur le Référencement Local et le GEO (Generative Engine Optimization)

L'absence de conformité juridique et technique constitue un facteur direct d'éviction par les moteurs de recherche modernes :

1. **Google Pack Local & Algorithme de Confiance :**  
   Google attribue un score d'E-E-A-T (Expérience, Expertise, Autorité, Fiabilité) renforcé aux sites démontrant leur authenticité : présence d'un numéro SIRET vérifiable, adresse physique dans le footer, politique de confidentialité conforme et certificat TLS valide. Les sites en erreur 4xx/5xx ou sans mentions légales perdent progressivement leur place dans le Pack Local des 3 premiers artisans.

2. **Sélection par les Moteurs d'IA (ChatGPT Search, Perplexity, Google AI Overviews) :**  
   Les robots des modèles de langage (LLMs) procèdent par extraction factuelle stricte. Lorsqu'un utilisateur demande : *« Recommande-moi un artisan chauffagiste sérieux à proximité »*, le modèle de langage évalue la certitude juridique de l'entité. Un domaine dépourvu de données structurées `LocalBusiness`, sans mentions légales claires ou inaccessible est rejeté au profit d'acteurs dont les données sont transparentes et vérifiables.

---

### 5. Recommandations Pratiques pour 2026-2027

1. **Remise en conformité juridique immédiate :**  
   Ajout d'une page Mentions Légales dédiée (raison sociale, forme juridique, SIRET, hébergeur et coordonnées directes) et d'une Politique de Confidentialité explicite précisant la durée de conservation des données collectées via formulaire.
2. **Gestion rigoureuse du consentement aux cookies :**  
   Mise en place d'un bandeau de recueil conforme CNIL bloquant réellement les scripts de suivi avant acceptation de l'utilisateur.
3. **Balisage Schema.org LocalBusiness :**  
   Intégration d'un bloc JSON-LD spécifiant l'identité légale de l'entreprise, le code postal, les coordonnées géographiques (latitude/longitude) et le champ d'intervention pour garantir l'indexation par les moteurs IA.
4. **Modèle économique pérenne :**  
   Privilégier la pleine propriété de son nom de domaine et de son site internet via des forfaits transparents (dès 490 € HT pour un site vitrine conforme 5 pages), plutôt que des locations captieuses auprès d'annuaires sous contrats d'engagement de longue durée.

---

### Références & Liens Utiles

- **DOI Zenodo (CERN) :** [10.5281/zenodo.24284538](https://doi.org/10.5281/zenodo.24284538)
- **Dépôt GitHub Open Data (CSV) :** [https://github.com/snipe91/barometre-tpe-france](https://github.com/snipe91/barometre-tpe-france)
- **Observatoire Numérique Site Digital Pro :** [https://sitedigitalpro.com](https://sitedigitalpro.com)
- **Étude originale complète :** [https://sitedigitalpro.com/barometre-tpe-2026/](https://sitedigitalpro.com/barometre-tpe-2026/)
- **Baromètre des artisans du bâtiment (1 030 sites) :** [https://sitedigitalpro.com/barometre-artisans-batiment/](https://sitedigitalpro.com/barometre-artisans-batiment/)
- **Historique des sanctions CNIL :** [https://sitedigitalpro.com/barometre-sanctions-cnil/](https://sitedigitalpro.com/barometre-sanctions-cnil/)
- **Scanner gratuit de conformité RGPD :** [https://rgpd-audit.com](https://rgpd-audit.com)
- **Tarifs et solutions techniques conformes :** [https://sitedigitalpro.com/nos-forfaits/](https://sitedigitalpro.com/nos-forfaits/)
