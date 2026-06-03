# X360 Mobile - Émulateur Xbox 360 pour Android

<p align="center">
  <img src="https://x360mobile.com/logo.png" alt="Logo X360 Mobile" width="180" style="border-radius: 20%;"/>
</p>

<p align="center">
  <b>Un émulateur Xbox 360 natif et expérimental pour Android, basé nativement sur Xenia Canary.</b>
</p>

<p align="center">
  <a href="https://www.x360mobile.com"><b>Site Officiel : www.x360mobile.com</b></a>
</p>

<p align="center">
  Choose Language / Scegli la lingua / Sprache wählen / Choisir la langue / Seleccionar idioma:
  <br>
  <a href="README.md">English</a> |
  <a href="README.it.md">Italiano</a> |
  <a href="README.de.md">Deutsch</a> |
  <b>Français</b> |
  <a href="README.es.md">Español</a>
</p>

---

Bienvenue sur le dépôt officiel de **X360 Mobile**, un émulateur Xbox 360 natif et expérimental conçu spécifiquement pour la plateforme Android. Développé à l'aide des technologies modernes ARM64 et Vulkan 1.3, X360 Mobile est le **pionnier de l'intégration native du célèbre cœur de développement Xenia Canary sur Android**, apportant des optimisations avancées et des performances haut de gamme directement sur vos appareils mobiles.

> [!NOTE]
> **Objectif du dépôt :** 
> Afin de protéger le code source et de préserver nos optimisations propriétaires de performances, **X360 Mobile est closed-source (code source fermé)**. Ce dépôt officiel ne contient pas le code source de l'émulateur. Il sert à la fois d'**archive officielle des versions et de plateforme de distribution principale** pour la publication des fichiers APK, la gestion des rapports de bug (Issues) et le partage des guides d'utilisation.

---

## Caractéristiques Principales

* **Fondation Native Xenia Canary :** Le tout premier émulateur Android conçu nativement autour de Xenia Canary dès sa conception, plutôt que de migrer ultérieurement depuis Xenia Master, garantissant une architecture et des performances supérieures.
* **Backend Vulkan Moderne :** Exploite les API Vulkan 1.3 pour offrir une utilisation optimale du matériel, des taux de rafraîchissement élevés (FPS) et une charge système minimale.
* **Superpositions Tactiles Personnalisées :** Manettes virtuelles entièrement personnalisables avec retour haptique, réponse analogique fluide et dispositions adaptées à toutes les tailles d'écran.
* **Prise en Charge des Manettes Physiques :** Compatibilité plug-and-play immédiate pour les manettes externes via Bluetooth ou USB-OTG (y compris les manettes Xbox Series X|S, DualSense, DualShock 4 et les principales manettes mobiles du marché).
* **Profils Spécifiques par Jeu :** Ajustez individuellement par jeu les résolutions, les options de compilation des shaders et les limites de mémoire pour tirer le meilleur de votre appareil.
* **Optimisations Mobiles :** Traduction dynamique intégrée du code d'assemblage PowerPC en instructions natives ARM64 avec des micro-optimisations spécifiques pour les processeurs Snapdragon et Dimensity.

---

## Configuration Système Requise

L'émulation de la Xbox 360 est expérimentale et extrêmement lourde sur le plan informatique, nécessitant une traduction matérielle complexe en temps réel. Veuillez consulter le tableau ci-dessous pour évaluer les performances attendues sur votre appareil.

| Spécification | Configuration Minimale | Recommandée (Pour des vitesses fluides) |
| :--- | :--- | :--- |
| **Système d'Exploitation** | Android 11 (64 bits) | Android 13 ou plus récent (64 bits) |
| **Processeur & GPU** | Qualcomm Snapdragon avec GPU Adreno (séries 600/700/800) | Qualcomm Snapdragon haut de gamme (recommandé Snapdragon 8 Gen 1 ou plus récent) |
| **RAM (Mémoire)** | 6 Go de RAM | 8 Go - 12 Go de RAM (ou plus) |
| **Stockage (Vitesse)** | Stockage haute vitesse (recommandé UFS 3.1 ou supérieur) | Stockage ultra-rapide UFS 3.1/4.0 |

> [!WARNING]
> Les appareils équipés de processeurs dotés de GPU Mali, de GPU Xclipse de Samsung (basés sur AMD RDNA), de GPU Adreno obsolètes (antérieurs à la série 600) ou de puces d'entrée de gamme subiront de graves limites de performances, des bugs visuels, une forte surchauffe (thermal throttling) ou des crashs. Un processeur Qualcomm Snapdragon moderne avec GPU Adreno est fortement recommandé pour un résultat optimal.

---

## Guide de Démarrage Rapide

1. **Téléchargez l'APK :** Rendez-vous dans notre section [Releases](https://github.com/Ashnar2602/X360-Mobile---OFFICIAL/releases) et téléchargez le dernier fichier `.apk` stable.
2. **Autorisez les Sources Inconnues :** Si vous y êtes invité, autorisez votre navigateur ou votre gestionnaire de fichiers à installer des applications provenant de sources inconnues dans les paramètres de sécurité d'Android.
3. **Installez et Lancez :** Installez le fichier APK téléchargé et lancez **X360 Mobile**.
4. **Configurez les Dossiers :** Créez un dossier dédié sur le stockage interne ou externe de votre appareil (par exemple, `/Emulation/Xbox360/Games`) et placez-y vos fichiers de jeux légalement obtenus.
5. **Formats de Jeux :** L'émulateur prend officiellement en charge les formats `.iso`, `.xex` et les dossiers décompressés (unpacked).
6. **Chargez et Jouez :** Indiquez à l'émulateur le chemin de votre dossier de jeux, sélectionnez un titre et lancez la partie !

---

## Foire Aux Questions (FAQ)

### X360 Mobile est-il gratuit ?
**Oui.** X360 Mobile est gratuit à télécharger et à utiliser. Nous ne facturons aucun frais et n'intégrons aucune publicité intrusive qui gâcherait l'expérience de jeu.

### Pourquoi le projet est-il closed-source ?
Nous avons fait le choix de garder X360 Mobile fermé afin d'éviter les forks frauduleux, les versions modifiées malveillantes (ex. injection de logiciels publicitaires ou espions dans nos builds), et de protéger notre pipeline exclusif de conversion ARM64 ainsi que les optimisations de notre compilateur. Nous voulons nous assurer que nos utilisateurs reçoivent uniquement des paquets sécurisés, hautement optimisés et signés officiellement directement depuis ce dépôt ou notre site officiel.

### X360 Mobile est-il lié au projet de bureau Xenia ?
X360 Mobile est basé sur l'incroyable code source de **Xenia Canary** (un projet open-source pour PC). Nous avons porté, réécrit et optimisé les moteurs de rendu et d'exécution d'origine pour les faire fonctionner sous Android. Nous respectons profondément les développeurs originaux de Xenia et visons à offrir le même niveau d'excellence sur les appareils mobiles.

### Quels jeux puis-je faire tourner actuellement ?
La compatibilité s'améliore constamment. Actuellement, **plus de 300 titres ont été testés**, dont environ **40 % sont entièrement jouables**.

Pour consulter une liste complète et à jour de compatibilité, veuillez visiter notre site officiel à l'adresse [www.x360mobile.com](https://www.x360mobile.com). Bien que les classiques Arcade, les jeux indépendants et les jeux 3D légers fonctionnent très bien, les jeux AAA plus gourmands (comme *Red Dead Redemption*, *Halo 3* ou *Gears of War*) sont bootables et peuvent atteindre des vitesses jouables sur les derniers processeurs phares Snapdragon, même s'ils peuvent encore présenter de légers bugs visuels ou de légères baisses de FPS.

---

## Signaler un Bug

Si vous rencontrez des plantages, des bugs graphiques ou des problèmes de compatibilité :
1. Rendez-vous dans la section [Issues](https://github.com/Ashnar2602/X360-Mobile---OFFICIAL/issues).
2. Vérifiez si le problème a déjà été signalé par un autre utilisateur.
3. Si ce n'est pas le cas, ouvrez un nouveau ticket en utilisant notre modèle et incluez :
   * Le modèle de votre appareil et son processeur (ex. Samsung Galaxy S23, Snapdragon 8 Gen 2).
   * La version exacte d'Android et la quantité de RAM.
   * Le titre du jeu et son format (.iso ou .xex).
   * Une description détaillée du bug et, si possible, des captures d'écran ou des vidéos.

---

## Mentions Légales et Exclusions de Responsabilité

* **Xbox 360** est une marque déposée de Microsoft Corporation. **X360 Mobile** n'est en aucun cas affilié, autorisé, sponsorisé ou approuvé par Microsoft Corporation, ses filiales ou ses partenaires.
* Tous les titres de jeux, images et logos de marques sont des marques commerciales de leurs propriétaires respectifs.
* **X360 Mobile** n'inclut aucun fichier de jeu, logiciel système (dashboard) ou ROM sous droit d'auteur. Les utilisateurs sont légalement tenus de posséder des copies physiques de leurs jeux et d'effectuer eux-mêmes les sauvegardes pour leur usage personnel et non commercial.
* En téléchargeant et en utilisant ce logiciel, vous acceptez nos conditions d'utilisation et reconnaissez que l'émulation est une technologie expérimentale utilisée à vos propres risques.

---

<p align="center">
  © 2026 X360 Mobile Team. Tous droits réservés. <br>
  Pour les actualités, mises à jour et plus encore, visitez le site <a href="https://www.x360mobile.com">www.x360mobile.com</a>.
</p>
