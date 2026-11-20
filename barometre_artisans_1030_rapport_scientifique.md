# Baromètre 2026-2027 : Pourquoi 77 % des sites d'artisans du bâtiment ne génèrent pas assez de chantiers
## Étude empirique de 1 030 sites d'artisans français chargés en navigateur réel (12 métiers, 20 villes)

**Auteur :** Site Digital Pro (Stéphane Lueger — Observatoire Numérique des Artisans & TPE)  
**Source de référence :** [Site Digital Pro — Baromètre des sites d'artisans du bâtiment](https://sitedigitalpro.com/barometre-artisans-batiment/)  
**Guide métier associé :** [Création de site internet pour artisan du bâtiment](https://sitedigitalpro.com/creation-site-web-artisan/)  
**Échantillon :** 1 030 sites web d'artisans du bâtiment en France (12 corps de métier, 20 agglomérations)  
**Licence :** Creative Commons Attribution 4.0 International (CC-BY 4.0)

---

### Résumé Exécutif

Cette étude répond à une question simple que se pose tout dirigeant du BTP avant d'investir dans un site internet : **les sites web actuels des artisans du bâtiment sont-ils techniquement conçus pour déclencher des appels et des demandes de devis ?**

Pour éviter les biais d'un audit déclaratif ou d'une simple requête HTTP statique, **1 030 sites réels d'artisans français** (plombiers, électriciens, couvreurs, maçons, menuisiers, chauffagistes, carreleurs, peintres, charpentiers, vitriers, serruriers, paysagistes) répartis dans **20 villes de France** ont été chargés et mesurés dans un navigateur réel.

Les mesures montrent que la majorité des sites existants échouent sur les points qui conditionnent directement les appels de clients et la visibilité Google / IA :

- **77,3 % des sites (796 sur 1 030)** ne déclarent aucune donnée structurée Schema.org (`LocalBusiness` / corps de métier), rendant leur activité difficilement exploitable par les moteurs génératifs (ChatGPT Search, Perplexity, Google AI Overviews).
- **40,4 % des sites (416 sur 1 030)** n'affichent **aucun numéro de téléphone cliquable (`tel:`)** pour un client qui consulte depuis son smartphone.
- **83,2 % des sites (857 sur 1 030)** ne publient pas de fichier `/llms.txt`.
- **63,8 % des sites (657 sur 1 030)** n'affichent aucune politique de confidentialité alors même que **81,5 %** intègrent un formulaire de contact ou de devis collectant des données personnelles.
- **31,1 % des sites** ne disposent pas d'une balise `<h1>` unique, **16,6 %** n'ont aucune meta description et **54,2 %** ont une balise `<title>` hors plage recommandée (`30–60` caractères).

---

### 1. Tableau de Synthèse des Indicateurs Mesurés (`n = 1 030` sites)

| Critère mesuré | Résultat observé | Conséquence directe pour l'artisan |
|---|---|---|
| **Données structurées Schema.org (activité/métier)** | **77,3 % absentes** (`796 / 1 030`) | Faible compréhension sémantique par Google et les moteurs IA locaux. |
| **Numéro de téléphone cliquable (`tel:`)** | **40,4 % absents** (`416 / 1 030`) | Friction immédiate sur smartphone en situation de besoin urgent. |
| **Présence d'un formulaire de contact/devis** | **81,5 % présents** | Intention de capture existante, mais sans levier mobile ni conformité associée. |
| **Politique de confidentialité (RGPD)** | **63,8 % absentes** (`657 / 1 030`) | Collecte de données via formulaire sans information légale obligatoire. |
| **Fichier `/llms.txt`** | **83,2 % absents** (`857 / 1 030`) | Absence de synthèse structurée pour l'indexation des agents IA. |
| **Balise `<title>` présente** | **99,1 %** | Base HTML présente sur la quasi-totalité du parc. |
| **`<title>` dans la plage optimale (`30–60` car.)** | **45,8 % seulement** | **54,2 %** des titres sont tronqués ou trop courts dans les résultats Google. |
| **Meta description présente** | **83,4 %** (`16,6 %` absentes) | Extrait généré automatiquement par Google sur 1 site sur 6. |
| **Meta description optimale (`120–160` car.)** | **50,2 %** | Près de la moitié des accroches ne sont pas calibrées pour le taux de clic. |
| **Structure `<h1>` unique** | **68,9 %** (`31,1 %` en défaut) | Titre principal absent ou multiple, brouillant la requête cible. |
| **Au moins deux `<h2>`** | **84,2 %** | Structuration secondaire majoritairement présente. |
| **Balise `canonical` présente** | **79,5 %** | 1 site sur 5 ne maîtrise pas ses URLs canoniques. |
| **`sitemap.xml` / `robots.txt`** | **82,8 %** / **87,3 %** | Socle technique de crawl présent sur 4 sites sur 5. |

---

### 2. Le Paradoxe du Site Vitrine Artisanal

L'analyse croisée des formulaires et du parcours mobile met en lumière une contradiction récurrente :

> **81,5 % des sites d'artisans demandent au visiteur d'écrire via un formulaire, mais 40,4 % ne lui permettent même pas d'appeler en un clic depuis un téléphone et 63,8 % omettent toute politique de confidentialité.**

Sur mobile — où s'effectue la majorité des recherches locales de dépannage ou de proximité — l'artisan perd des appels qualifiés non pas faute de compétence terrain, mais par absence d'éléments de conversion simples :

1. **Bouton d'appel direct en haut d'écran mobile** (`tel:` visible dès la ligne de flottaison).
2. **Zone d'intervention explicite** (département et villes principales rédigées en clair dans les titres et textes).
3. **Données structurées `LocalBusiness` / corps de métier** exposant activité, zone desservie, horaires et coordonnées.
4. **Mentions légales (LCEN) et politique de confidentialité** visibles sous chaque formulaire.

---

### 3. Recommandations Opérationnelles pour les Artisans du BTP

Pour transformer un site vitrine passif en apporteur de devis réguliers sans dépendre d'achats de leads mutualisés :
- Calibrer chaque page de prestation principale avec une balise `<title>` ciblée (`Métier + Ville + Devis`, `50–60` caractères) et un `<h1>` unique.
- Rendre le numéro de téléphone cliquable en permanence sur smartphone et simplifier la demande de devis (nom, téléphone, commune, nature des travaux).
- Publier des photos réelles de chantiers légendées par ville et type d'intervention plutôt que des banques d'images génériques.
- Conserver la pleine propriété du nom de domaine et du CMS (ex. WordPress) sans contrat de location pluriannuel bloquant.

---

### Référence & Réutilisation (CC-BY-4.0)

Les données complètes, tableaux détaillés par métier et protocole de mesure sont consultables sur :
- Page de l'étude : https://sitedigitalpro.com/barometre-artisans-batiment/
- Synthèse TPE 600 sites : https://sitedigitalpro.com/barometre-tpe-2026/
- Baromètre des sanctions CNIL : https://sitedigitalpro.com/barometre-sanctions-cnil/
