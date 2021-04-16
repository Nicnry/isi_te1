# Resumé TE1 ISI (recto)

## chapitre 1
phreaking = ancien type de piratage (sur rsx téléphonique)


## chapitre 2 - Introduction
Conséquences de la sécurité (perte) :
- financière
- réputation
- image de marque
- avantage compétitif
- temps
Exemple :
- Perte de données
- Fuite de données

Risques :
- Cyber attacks
- Activités criminel
- Degâts naturels
- Terrorisme

### Système d'information
un ensemble de personnes, de procédure, guides, directives, processus et de ressources qui recueillent de l'information en la stockant, la transformant et la distribuant au sein d'une organisation

### Modèle en oignon
![Modèle en oignon](./img/oignon.jpg)
1. Physique :
    - sécurité physique

(sécurité technique)

2. Réseau :
    - architecture et éléments réseau, adressage IP.
3. Protocoles :
    - Protocoles de communication, middleware.
4. Hosts :
    - systèmes d'exploitation et applications hosts.
5. Applications :
    - langages de programmation, applications spécifiques/dédiées, données spécifiques.

Chaque couche doit implémenter ses propres concepts de sécurités, est obligée de faire confiance à la couche inférieur et controle l'accès à la couche supérieur

### Sécurité de l'information
#### Définition
- Protéger l’information.
- Et donc protéger le système traitant l’information.
- Contre des opérations non-autorisées telles que : accès, utilisations, fuites, modifications, destructions ou interruption de disponibilité.

#### CIA
- Confidentialité (Confidentiality) :
    - s'assurer que l'information est accessible seulement à ceux qui sont autorisés à y avoir accès;
- Intégrité (Integrity) :
    - protéger l'exactitude et la complétude de l'information et des méthodes de traitement;
- Disponibilité (Availability) :
    - s'assurer que les utilisateurs autorisés ont accès à l'information et aux ressources associées au moment et au lieu exigés.

### Contrôle d'accès - AAA
- Authentification (Authentication) :
    - s'assurer que la personne est bien celle qu’elle prétend être;
    - déterminer son identité et éventuellement son rôle;
- Autorisation/permission (Authorization) :
    - détermine en fonction de l’identité (ou rôle), que cela soit une personne ou un système, si l’accès (ou le traitement) est autorisé;
    - Cette décision doit respecter la politique au travers des droits du contrôle d’accès;
- Comptabilisation/traçabilité (Accounting/auditing) :
    - s’assurer qu’il soit possible de suivre les accès/traitement qui ont été effectués;
    - journalisation (logging);

### 3 domaines de la SSI
#### Sécurité physique
- But
    - la protection physique,
    - la prévention physique,
    - et la récupération physique.
- Exemples
    - bâtiments, incendies, inondations, salle des serveurs,
    - contrôle de l'accès physique,
    - électricité, climatisation,
    - câblage et réseaux physiques, bornes wifi,
    - sécurité des machines telles que les serveurs, ordinateurs portables, smartphones, supports amovibles, imprimantes
#### Sécurité organisationnelle
- But
    - La sécurité organisationnelle couvre les aspects sociaux, légaux, organisationnels et humains liés à la SSI.
    - Des règles, procédures et directives sont définies et appliquées afin de réglementer comment une organisation recueille, traite, stocke, protège et distribue les informations sensibles.
- Exemples
    - procédures (gestion des accès),
    - contrats (employés, clients, partenaires),
    - responsabilités (cahiers des charges),
    - formations et sensibilisations,

#### Sécurité technique
- But
    - La sécurité technique concerne le traitement, le stockage et la communication de l'information numérique (ou analogique).
    - Couches concernées du modèle en oignon : "Réseau", "Protocoles", "Hosts" et "Applications"
- Exemples
    - sécurité des données en transit sur les réseaux informatiques et de télécommunication,
    - sécurité des bases de données,
    - sécurité logicielle, applications, middleware, systèmes d'exploitation,
    - sécurité des fichiers de configuration,

### Conséquences d'un dommage
- (C) perte de confidentialité (et/ou)
- (I) perte d'intégrité (et/ou)
- (D) perte de disponibilité de l'information.

### Cycle de vie
- une prévention (via une protection) contre les incidents de sécurité,
- la détection (via une surveillance) de ces dernières,
- la réaction (analyse, confinement),
- la récupération (reprise, sanctions éventuelles), puis analyse «post mortem» suite aux dommages survenus.

### Fondamentaux en sécurité
1. La sécurité globale est aussi forte que le maillon le plus faible
2. La sécurité parfaite est impossible
3. La sécurité est un processus (pas un produit)
4. La sécurité est inversement proportionnelle à la complexité
5. Participation des utilisateurs

### Stratégie d'architecture
1. Interdiction par défaut
2. Moindre privilège
3. Défense en profondeur
4. Séparation des fonctions
5. Segmentation
6. Economie de mécanismes
7. Goulet d’étranglement
8. Interruption/erreur sûre
9. Eviter la sécurité par obscurité

## chapitre 3 - Insecurité des systèmes
une **menace** peut exploiter une **vulnerabilité** en causant des **dommages** ce qui crée un **incident** il faut donc étudier et surveiller les **vulnérabilités**
### Types de menaces
#### Menaces accidentelles (erreurs) :
- Mauvaises manipulations : déclassification ou destruction accidentelle d'une information, perte d'un laptop, etc.
- Négligence, incompétence, fatigue, stress...
#### Menaces environnementales :
- d'origine naturelle : tremblements de terre, cyclones, avalanches, foudre, inondations, etc... (typique de zones géographiques)
- d'origine industrielle : industries chimiques (corrosion, pollution), chantiers, émissions radioélectriques
parasites, etc.
#### Menaces délibérées (intentionnelles) :
- d’origine criminelle : les risques relatifs dépendent alors des compétences, des types d’intention et des
motivations de l'agresseur.
### Types de vulnerabilites
#### Matériel
- maintenance insuffisante des équipements de stockage (disques saturés/morts, sans alerte).
#### Logiciel
- Sondage (CMU) : en moyenne il y a 20-30 bugs/failles par 1000 lignes de codes...
- Exploitation / utilisation : cas WEF (oubli ? incompétences ?)
#### Réseau
- trafic sensible non protégé, accès Wifi ouverts, etc.
#### Personnel (RH)
- absence, manque de formation, faute, contournement de procédure, etc.
#### Site (physique)
- alimentation électrique instable, antivols, etc.
#### Organisation
- procédure d'enregistrement / d'accréditation d'un utilisateur, etc.

### Attaquants
- black, grey, white hat (méchant, dépend de l'envie, gentil)

#### Motivations
- S'amuser, souvent sans autre but
- Curiosité
- Prise de contrôle, pouvoir, ego
- Acquérir des connaissances techniques
- Morales : politique, écologie, social, «robin des bois», etc.
- Ressources gratuites : accès, machines, etc.
- Argent, escroqueries, espionnage industriel/économique
- Terrorisme, espionnage, guerre informatique
- (Apprentissage, tests d’intrusions, améliorations sécuritaires, etc.)

#### Compétences
80% "script kiddies", 15% "Eduqués" et 5% Experts

#### Demarche intrusions
![Demarche intrusion](./img/demarche_intrusion.jpg)

## chapitre 4 - Collecte d'informations
Il existe 3 moyens pour la collecte d'information
### Recherches sur le web
Informations susceptibles d'être trouvées (réseaux sociaux) :
- Contacts
- Numéros de téléphones, emails, adresses postales
- Documents publiquement accessibles
- Il peut même être utile de trouver les restaurants/cafétérias proches de l’entreprise pour pouvoir
espionner les conversations des employés
- Vulnérabilités, messages d'erreurs trop verbeux, fichiers de logs (FW, VPNs, ...)
- Fichiers de configuration contenant des mots de passe
- Documents / répertoires sensibles

créer des requête complexes pour trouver des vulnérabilités ou des informations sensibles (Google hacking) :
- Recherche de pages appartenant à un site Internet :
    - site:heig-vd.ch
- Recherche de pages pointant sur un site Internet :
    - link:heig-vd.ch
- Recherche de fichiers sur la Sécurité au format PDF :
    - filetype:pdf sécurité
- Recherche de serveurs web autorisant le directory listing :
    - site:heig-vd.ch in9tle:"index of /"
- Autres commandes comme inurl, in9tle, "config", "setup"
- Page mise en cache...
Outils : Gooscan, Athena, SiteDigger
### Questionnement de services Internet
Whois (« qui est ? ») (`whois [ip or domain]`)
- Service de recherche permeLant d'obtenir des informations sur
- des adresses IP
- des noms de domaine
- Interrogation des registres Internet :
- les Registres Internet régionaux (RIR)
- les registres de noms de domaine, Network Information Center (NIC), (.com, .ch, ...)
- Informations à usages variés,
- coordination entre ingénieurs réseaux pour résoudre un problème technique,
- la recherche du titulaire d'un nom de domaine par une société qui souhaiterait l'obtenir,

DNS (`nslookup` ou `host` ou `dig`) :
- Interrogation direct au(x) serveur(s) DNS

Reconnaissance réseau (`traceroute` Linux ou `tracrt` Windows) 
### Social engineering
- Forme d'acquisi:on déloyale d'information et d'escroquerie
- Utilisée pour obtenir d'autrui, un bien, un service ou des informa:ons clefs.
- Exploite les failles humaines et sociales de la structure cible
- Utilisant ses connaissances, son charisme, l'imposture ou le culot, le pirate abuse de la confiance, de l'ignorance ou de la crédulité des personnes possédant ce qu'il tente d'obtenir.

## chapitre 5 - Scanning et énumération
## chapitre 6 - Intrusions de systèmes
## chapitre 7 - Spams
## chapitre 8 - E-mails forgés
## chapitre 9 - Codes malveillants
## chapitre 10 - Attaques réseaux
## chapitre 11 - Attaques Web
## chapitre 12 - Escalade de privilèges, pillage, nettoyage des traces
## chapitre 13 - Dénis de service
Objectif : Nuire à la disponibilité d'un système d'information
Exemples de techniques connues :
- «SYN flooding»
    - bcp de paquets SYN pour surcharger la RAM (contré par timeout plus court ou limiter les connexions en suspens)
- Smurf
    - bcp de ping indirect sur adresses broadcast (contré par filtrer ping en broadcast)
- Déni de service distribué (DDoS)
    - utiliser des machines esclaves (plusieurs esclaves/maitres = botnet)

Protextion DoS
- défense au niveau du FAI / ISP (FAI : fournisseur d’accès Internet)
- éviter les vulnérabilités des systèmes (OS, applications, ...)
- filtrage au niveau des pare-feux et routeurs (utilisation de seuils...)
- redondance des équipements