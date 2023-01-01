# Comment installer Plutonium

## Launcher Plutonium

1. Téléchargez [plutonium.exe](https://cdn.plutonium.pw/updater/plutonium.exe)

Vous pouvez enregistrer le launcher où vous le souhaitez, dans un endroit pratique comme votre bureau ou le dossier du jeu.

2. Ouvrez le launcher, si Smart Screen apparaît, cliquez sur **Plus d’informations** puis **Exécuter**

![smartscreen 1](/images/docs/install/QVb7Cv4.png)
![smartscreen 2](/images/docs/install/E4lDWsb.png)

Le launcher va maintenant démarrer le processus d'installation des fichiers du client.

![launcher self update / installation](/images/docs/install/9aHmzEk.png)

3. Entrez vos identifiants saisi sur le forum pour vous connecter. Si vous n'avez pas encore de compte sur le forum, vous pouvez en créer un [ici](https://forum.plutonium.pw/register).

![launcher login page](/images/docs/install/sA951Dt.png)

4. Configurez le jeu auquel vous voulez jouer.

## T6 (Black Ops 2)

### Je veux juste mettre à jour / J’ai déjà BO2 installé

Si vous avez déjà installé le jeu à partir de Steam ou si vous avez déjà télécharger le jeu depuis le site de Plutonium, vous pouvez ignorer cette partie et passer à la section **[Installation des DLC](#installation-des-dlc-bo2)**.

### Installation du jeu de base (BO2)

Cette section explique comment télécharger une copie de BO2.  
Ignorez cette section si vous avez déjà une copie du jeu depuis Steam ou Plutonium.

**Veuillez noter que nous vous recommandons fortement d’acheter le jeu si vous ne le possédez pas, c’est le meilleur moyen d’obtenir une copie des fichiers du jeu qui sont à jour et non corrompus ou modifiés d’une manière ou d’une autre. Les sites de ventes de clés ont souvent des prix intéressants.**

1. Dans l’explorateur de fichiers Windows, accédez à Ce PC, puis à **Disque local (C:)** et créez un nouveau dossier appelé **Jeux**

![Explorer steps 1-2](/images/docs/install/bmMI4UH.png)

![Explorer step 3](/images/docs/install/1MphGAa.png)

![Explorer step 4](/images/docs/install/cRa2jC2.png)

<Alert variant="warning">
  
Le torrenting de fichiers protégés par le droit d’auteur peut ne pas être légal dans votre pays, même si vous possédez déjà une licence valide!
Nous ne sommes pas responsables des problèmes juridiques et vous recommandons d'acheter le jeu ou d'utiliser un VPN lors du téléchargement d'un torrent.

</Alert>

2. Téléchargez/ouvrez votre client torrent.  
qBittorent Windows x64 est recommandé : [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

3. Téléchargez le [fichier torrent](/pluto_t6_full_game.torrent).

4. Ouvrez le fichier torrent `pluto_t6_full_game.torrent` (téléchargé à l’étape précédente).  
Votre client torrent va s'ouvrir et vous demander où vous voulez enregistrer le jeu.  
**SÉLECTIONNEZ LE DOSSIER JEUX CRÉÉ À L’ÉTAPE 1 COMME EMPLACEMENT D’ENREGISTREMENT**

5. Démarrez le téléchargement et attendez que le téléchargement soit terminé.  
Vous saurez qu’il est terminé lorsque la barre de progression passe à `100%` et que le statut passe à `Émission` ou `Partage`.

Une fois le téléchargement terminé, vous aurez téléchargé votre copie du jeu, voici un exemple de dossier de jeu de base terminé:

![Completed Game Folder](/images/docs/install/B8g1bXI.png)

### Installation des DLC (BO2)

<Alert variant="warning">

Si vous avez installé le jeu via le torrent fourni dans les instructions précédentes alors [passez à la configuration dans le launcher](#configurer-t6-dans-le-launcher-plutonium).  
**Cette partie ne concerne que les personnes qui utilisent leurs fichiers Steam et qui ne possèdent pas les DLC**.  
Ce torrent ne fourni que les cartes des DLC. Vous ne pouvez pas jouer au jeu seulement avec ces fichiers. Si vous voulez télécharger le jeu alors [lisez au dessus](#installation-du-jeu-de-base-bo2)!  
Gardez en tête que si un serveur charge une carte des DLC et que vous ne l'avez pas installé vous serez exclu, si vous le pouvez il est donc préférable de les installer.

</Alert>

1. Téléchargez/ouvrez votre client torrent.
qBittorent Windows x64 est recommandé : [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

2. Téléchargez le [fichier torrent](/t6_dlcs.torrent).

3. Ouvrez le fichier torrent `t6_dlcs.torrent` (téléchargé à l’étape précédente).  
Votre client torrent va s'ouvrir et vous demander où vous voulez enregistrer le jeu.  
**SÉLECTIONNEZ LE DOSSIER CALL OF DUTY BLACK OPS II DANS VOS JEUX STEAM**

![img](/images/docs/install/9ff55628c526220795c0f23f3a6aa719.png)

4. Sélectionnez `"ne pas créer de sous-dossier"` dans la liste déroulante `"agencement du contenu"` (dans les anciennes versions de qBittorrent il faudra décocher `"créer un sous dossier"` ou `"conserver la structure du dossier"`)
![img](/images/docs/install/f32c04d072946509231016a435e9c521.png)

5. Démarrez le téléchargement et attendez que le téléchargement soit terminé.  
Vous saurez qu’il est terminé lorsque la barre de progression passe à `100%` et que le statut passe à `Émission` ou `Partage`.

### Configurer T6 dans le launcher Plutonium

Naviguez dans l'onglet Black Ops 2 et cliquez sur **SETUP** et sélectionnez le dossier contenant les fichiers de Black Ops II.  
Le dossier que vous devrez sélectionner s'appelera très probablement `pluto_t6_full_game` ou `Call of Duty Black Ops II`.  
Ne sélectionnez pas votre dossier Games ou Jeux ou le dossier Documents. **Sélectionnez le dossier qui contient les fichiers de Black Ops II !**

![Launcher set-up 1](/images/docs/install/5FOePMY.png)

* **Si vous utilisez vos fichiers Steam, il se trouvera à cet emplacement :** `{Lettre disque}\Program Files (x86)\Steam\steamapps\common\Call of Duty Black Ops 2`

* **Si vous utilisez le torrent** le dossier a sélectionner sera nommé `pluto_t6_full_game`
![Launcher set-up 2](/images/docs/install/hdjiIhN.png)

**(Si jamais vous avez besoin de resélectionner le dossier du jeu, cliquez simplement sur Game Settings à côté du bouton PLAY)**
![Launcher reselect hint](/images/docs/install/MnkAcr8.png)

Pour ceux qui ont du mal à localiser le dossier du jeu, voici à quoi ressemble le contenu du dossier du jeu:

![Completed Game Folder](/images/docs/install/B8g1bXI.png)

### Erreur T6 : Chemin du jeu non valide

Si cette erreur s'affiche alors le dossier que vous avez sélectionné pendant le setup ne contient pas les fichiers du jeu.

![img](/images/docs/install/46KPMDc.png)

Si vous voyez cette erreur alors vous avez sélectionné votre disque tout entier au lieu du dossier du jeu.  
`C:\` n'est pas le dossier de Black Ops II.

![img](/images/docs/install/error-401.png)

Dans les deux cas, pour régler cette erreur vous devez cliquer sur Game settings dans le launcher et sélectionner le dossier qui contient les fichiers de Black Ops II.  
Si vous n'arrivez pas à le trouver alors lisez à nouveau le [guide depuis le début](#t6-black-ops-2).

![img](/images/docs/install/MnkAcr8.png)

Vous avez maintenant terminé l'installation de BO2.  
Pour lancer BO2 ouvrez le launcher et cliquez sur PLAY.

---

## IW5 (Modern Warfare 3)

### Je veux juste mettre à jour / J’ai déjà MW3 installé

Si vous avez déjà installé le jeu à partir de Steam ou si vous avez déjà télécharger le jeu depuis le site de Plutonium, vous pouvez ignorer cette partie et passer à la section **[Installation des DLC](#installation-des-dlc-mw3)**.

### Installation du jeu de base (MW3)

Note : Cette section explique comment télécharger une copie GRATUITE de MW3.  
Ignorez cette section si vous avez déjà une copie du jeu depuis Steam ou Plutonium.

**Veuillez noter que nous vous recommandons fortement d’acheter le jeu si vous ne le possédez pas, c’est le meilleur moyen d’obtenir une copie des fichiers du jeu qui sont à jour et non corrompus ou modifiés d’une manière ou d’une autre. Les sites de ventes de clés ont souvent des prix intéressants.**

Ouvrez Steam, si vous n’avez pas installé Steam, vous pouvez le télécharger [ici](https://store.steampowered.com/about/?l=french).

#### Méthode 1

Cliquez sur ce lien pour lancer l’installation de Call of Duty: Modern Warfare 3 - Serveur dédié dans Steam [steam://install/42750](steam://install/42750).

#### Méthode 2 (si la méthode 1 ne fonctionne pas)

1. Allez dans `BIBLIOTHÈQUE` et dans la liste déroulante sélectionnez `OUTILS`

![img](/images/docs/install/fzKXqGs.png)

2. Séléctionnez `Call of Duty: Modern Warfare 3 - Dedicated Server` puis cliquez sur l’icône en forme de rouage, puis `Propriétés`.

![img](/images/docs/install/ln7ml3F.png)

3. Dans l'onglet `LANGUE` assurez-vous que la langue est `English` ou `Anglais`. C'est très important car malheureusement le serveur dédié Steam MW3 ne peut pas installer toutes les langues ce qui provoquerait des erreurs à cause de fichiers manquants.

![img](/images/docs/install/NXLe3YD.png)

<Alert variant="tip">
  
Si vous voulez le jeu en français, nous vous suggérons d’acheter le jeu et ses DLC sur un site de vente de clés ou lors d’une promotion Steam.

</Alert>

4. Sélectionnez `INSTALLER` puis `Suivant` et enfin `Terminer`.

![img](/images/docs/install/LVhQAtW.png)

![img](/images/docs/install/pQB76hJ.png)

Maintenant, attendez simplement que le téléchargement se termine.  
Vous pouvez surveiller la progression en cliquant sur le bouton `TÉLÉCHARGEMENTS` en bas dans Steam. Une fois le téléchargement terminé, vous aurez une copie de MW3.

### Installation des DLC (MW3)

Cette section explique comment télécharger et installer les DLC pour avoir l'éxperience MW3 complète.  
Si vous ne voulez pas installer les DLC, vous pouvez alors [passez à la configuration dans le launcher](#configurer-iw5-dans-le-launcher-plutonium).  
Vous pouvez au choix télécharger les DLC en utilisant le lien MEGA ou le torrent. **Vous n'avez pas besoin des deux, prennez le téléchargement qui vous arrange.**  
Notez que ce téléchargement est optionnel. Ils ne sont nécessaires que pour jouer aux cartes DLC.  
Gardez à l'esprit que si un serveur charge une carte DLC et que vous ne l'avez pas installé vous serez exclu, il est donc recommandé d'installer les DLC si possible.  
A noter que ce téléchargement ne fourni que les cartes DLC. Vous ne pouvez pas jouer au jeu seulement avec ces fichiers. Si vous voulez télécharger le jeu alors [lisez au dessus](#installation-du-jeu-de-base-mw3)!

#### MEGA

1. Téléchargez l’archive zip des DLC via [ce lien](https://mega.nz/folder/CYUkGSrJ#HVa6Cik59Bgi9pp5NBW4fg).

![img](/images/docs/install/Zqx80uj.png)

2. Une fois le téléchargement terminé, ouvrez le zip `MW3 DLC [EN].zip`

![img](/images/docs/install/4ty889E.png)

![img](/images/docs/install/9wYQgJ3.png)

3. Localisez le dossier contenant les fichiers de MW3.
Par défaut, Steam l’aura installé à l’emplacement suivant : `C:\Program Files (x86)\Steam\steamapps\common\Call of Duty Modern Warfare 3`  
Vous pouvez également trouver votre dossier via Steam si nécessaire

![img](/images/docs/install/K7dj3mP.png)

4. Retournez dans le zip `MW3 DLC [EN].zip` et faites glisser les dossiers `main` et `zone` dans le dossier content les fichiers de MW3.
Si il est vous est demandé de remplacer des fichiers sélectionnez `Remplacer les fichiers`.

![img](/images/docs/install/3m5tWAj.png)

![img](/images/docs/install/yKw8Rl2.png)

#### Torrent

1. Téléchargez/ouvrez votre client torrent.  
qBittorent Windows x64 est recommandé : [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

2. Téléchargez le [fichier torrent](/iw5m_dlcs.torrent).

3. Ouvrez le fichier torrent `iw5m_dlcs.torrent` (téléchargé à l’étape précédente).  
Votre client torrent va s'ouvrir et vous demander où vous voulez enregistrer les DLC.  
**SÉLECTIONNEZ LE DOSSIER CALL OF DUTY MODERN WARFARE 3 DANS VOS JEUX STEAM**

Par défaut, Steam l’aura installé à l’emplacement suivant : `C:\Program Files (x86)\Steam\steamapps\common\Call of Duty Modern Warfare 3`
Vous pouvez également trouver votre dossier via Steam si nécessaire

![img](/images/docs/install/K7dj3mP.png)

![img](/images/docs/install/mw3_torrent_folder.png)

4. Sélectionnez `"ne pas créer de sous-dossier"` dans la liste déroulante `"agencement du contenu"` (dans les anciennes versions de qBittorrent il faudra décocher `"créer un sous dossier"` ou `"conserver la structure du dossier"`)

![img](/images/docs/install/f32c04d072946509231016a435e9c521.png)

5. Décochez `iw5m_dlcs` et cochez seulement `main` and `zone`.

![img](/images/docs/install/mw3_torrent_settings.png)

6. Démarrez le téléchargement et attendez que le téléchargement soit terminé.  
Vous saurez qu’il est terminé lorsque la barre de progression passe à `100%` et que le statut passe à `Émission` ou `Partage`.

Vous avez maintenant terminé l'installation des DLC de MW3.

### Configurer IW5 dans le launcher Plutonium

Naviguez dans l'onglet Modern Warfare 3 et cliquez sur **SETUP** et sélectionnez le dossier contenant les fichiers de Modern Warfare 3.  
Le dossier que vous devrez sélectionner s'appelera `Call of Duty Modern Warfare 3`.  
Ne sélectionnez pas votre dossier Games ou Jeux ou le dossier Documents. **Sélectionnez le dossier qui contient les fichiers de Modern Warfare 3 !**
![img](/images/docs/install/qDJ7OeD.png)

* **Si vous utilisez les fichiers Steam, il se trouvera à cet emplacement :** `{Lettre disque}\Program Files (x86)\Steam\steamapps\common\Call of Duty Modern Warfare 3`.

![img](/images/docs/install/qtgfVmJ.png)

**(Si jamais vous avez besoin de resélectionner le dossier du jeu, cliquez simplement sur Game Settings à côté du bouton PLAY)**

![img](/images/docs/install/MnkAcr8.png)

Pour ceux qui ont du mal à localiser le dossier du jeu, voici à quoi ressemble le contenu du dossier du jeu :

![img](/images/docs/install/7FOyDlg.png)

### Erreur IW5 : Chemin du jeu non valide

Si cette erreur s'affiche alors le dossier que vous avez sélectionné pendant le setup ne contient pas les fichiers du jeu.

![img](/images/docs/install/mw3-wrong-folder.png)

Si vous voyez cette erreur alors vous avez sélectionné votre disque tout entier au lieu du dossier du jeu.
`C:\` n'est pas le dossier de Modern Warfare 3.

![img](/images/docs/install/error-401.png)

Dans les deux cas, pour régler cette erreur vous devez cliquer sur Game settings dans le launcher et sélectionner le dossier qui contient les fichiers de Modern Warfare 3.  
Si vous n'arrivez pas à le trouver alors lisez à nouveau le [guide depuis le début](#iw5-modern-warfare-3).

![img](/images/docs/install/MnkAcr8.png)

Vous avez maintenant terminé l'installation de MW3.  
Pour lancer MW3 ouvrez le launcher et cliquez sur PLAY.

---

## T4 (World at War)

### Je veux juste mettre à jour / J’ai déjà WAW installé

Si vous avez déjà installé le jeu à partir de Steam ou si vous avez déjà télécharger le jeu depuis le site de Plutonium, vous pouvez ignorer cette partie et passer à la section **[Configurer T4 dans le launcher Plutonium](#configurer-t4-dans-le-launcher-plutonium)**.

### Installation du jeu de base (WAW)

Cette section explique comment télécharger une copie de WAW. Ignorez cette section si vous avez déjà une copie du jeu depuis Steam ou Plutonium.

**Veuillez noter que nous vous recommandons fortement d’acheter le jeu si vous ne le possédez pas, c’est le meilleur moyen d’obtenir une copie des fichiers du jeu qui sont à jour et non corrompus ou modifiés d’une manière ou d’une autre. Les sites de ventes de clés ont souvent des prix intéressants.**

1. Dans l’explorateur de fichiers Windows, accédez à Ce PC, puis à **Disque local (C:)** et créez un nouveau dossier appelé **Jeux**

![PC Explorer](/images/docs/install/bmMI4UH.png)
![Games Folder](/images/docs/install/1MphGAa.png)
![Games Folder Completed](/images/docs/install/cRa2jC2.png)

<Alert variant="warning">

Le torrenting de fichiers protégés par le droit d’auteur peut ne pas être légal dans votre pays, même si vous possédez déjà une licence valide!
Nous ne sommes pas responsables des problèmes juridiques et vous recommandons d'acheter le jeu ou d'utiliser un VPN lors du téléchargement d'un torrent.

</Alert>

3. Téléchargez/ouvrez votre client torrent.
qBittorent Windows x64 est recommandé : [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

4. Téléchargez le [fichier torrent](/pluto_t4_full_game.torrent).

5. Ouvrez le fichier torrent `pluto_t4_full_game.torrent` (téléchargé à l’étape précédente).  
Votre client torrent va s'ouvrir et vous demander où vous voulez enregistrer le jeu.  
**SÉLECTIONNEZ LE DOSSIER JEUX CRÉÉ À L’ÉTAPE 1 COMME EMPLACEMENT D’ENREGISTREMENT**

6. Démarrez le téléchargement et attendez que le téléchargement soit terminé.  
Vous saurez qu’il est terminé lorsque la barre de progression passe à `100%` et que le statut passe à `Émission` ou `Partage`.

Une fois le téléchargement terminé, vous aurez téléchargé votre copie du jeu, voici un exemple de dossier de jeu de base terminé:

![Completed T4 Folder](/images/docs/install/NoAuNW8.png)

---

### Configurer T4 dans le launcher Plutonium

Naviguez dans l'onglet World At War et cliquez sur **SETUP** et sélectionnez le dossier contenant les fichiers de World At War.  
Le dossier que vous devrez sélectionner s'appelera très probablement `pluto_t4_full_game` ou `Call of Duty World At War`.  
Ne sélectionnez pas votre dossier Games ou Jeux ou le dossier Documents. **Sélectionnez le dossier qui contient les fichiers de World At War !**
![WAW in launcher](/images/docs/install/4xzmAUX.png)

* **Si vous utilisez vos fichiers Steam, il se trouvera à cet emplacement :** `{Lettre disque}\Program Files (x86)\Steam\steamapps\common\Call of Duty World At War`

* **Si vous utilisez le torrent** le dossier a sélectionner sera nommé `pluto_t4_full_game`

**(Si jamais vous avez besoin de resélectionner le dossier du jeu, cliquez simplement sur Game Settings à côté du bouton PLAY)**

---

### Erreur T4 : Chemin du jeu non valide

Si cette erreur s'affiche alors le dossier que vous avez sélectionné pendant le setup ne contient pas les fichiers du jeu.

![Invalid Game Directory](/images/docs/install/vlwamKe.png)

Si vous voyez cette erreur alors vous avez sélectionné votre disque tout entier au lieu du dossier du jeu.
`C:\` n'est pas le dossier de World at War.

![img](/images/docs/install/error-401.png)

Dans les deux cas, pour régler cette erreur vous devez cliquer sur Game settings dans le launcher et sélectionner le dossier qui contient les fichiers de World at War.  
Si vous n'arrivez pas à le trouver alors lisez à nouveau le [guide depuis le début](#t4-world-at-war).

![img](/images/docs/install/MnkAcr8.png)

Vous avez maintenant terminé l'installation de WAW.  
Pour lancer WAW ouvrez le launcher et cliquez sur PLAY.

## T5 (Black Ops 1)

### Je veux juste mettre à jour / J’ai déjà BO1 installé

Si vous avez déjà installé le jeu à partir de Steam ou si vous avez déjà télécharger le jeu depuis le site de Plutonium, vous pouvez ignorer cette partie et passer à la section **[Installation des DLC](#installation-des-dlc-bo1)**.

### Installation du jeu de base (BO1)

Cette section explique comment télécharger une copie de BO.  
Ignorez cette section si vous avez déjà une copie du jeu depuis Steam ou Plutonium.

**Veuillez noter que nous vous recommandons fortement d’acheter le jeu si vous ne le possédez pas, c’est le meilleur moyen d’obtenir une copie des fichiers du jeu qui sont à jour et non corrompus ou modifiés d’une manière ou d’une autre. Les sites de ventes de clés ont souvent des prix intéressants.**

1. Dans l’explorateur de fichiers Windows, accédez à Ce PC, puis à **Disque local (C:)** et créez un nouveau dossier appelé **Jeux**

![PC Explorer](/images/docs/install/bmMI4UH.png)
![Games Folder](/images/docs/install/1MphGAa.png)
![Games Folder Completed](/images/docs/install/cRa2jC2.png)

<Alert variant="warning">

Le torrenting de fichiers protégés par le droit d’auteur peut ne pas être légal dans votre pays, même si vous possédez déjà une licence valide !  
Nous ne sommes pas responsables des problèmes juridiques et vous recommandons <a href="steam://install/42700">d'acheter le jeu sur Steam</a> ou d'utiliser un VPN lors du téléchargement d'un torrent.

</Alert>

2. Téléchargez/ouvrez votre client torrent.  
qBittorent Windows x64 est recommandé : [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

3. Téléchargez le [fichier torrent](/pluto_t5_full_game.torrent).

4. Ouvrez le fichier torrent `pluto_t5_full_game.torrent` (téléchargé à l’étape précédente).  
Votre client torrent va s'ouvrir et vous demander où vous voulez enregistrer le jeu.  
**SÉLECTIONNEZ LE DOSSIER JEUX CRÉÉ À L’ÉTAPE 1 COMME EMPLACEMENT D’ENREGISTREMENT**


5. Démarrez le téléchargement et attendez que le téléchargement soit terminé.  
Vous saurez qu’il est terminé lorsque la barre de progression passe à `100%` et que le statut passe à `Émission` ou `Partage`.

**Une fois qu'il est écrit Emission ou Partage vous pouvez supprimer le torrent de votre client torrent**

Une fois le téléchargement terminé, vous aurez téléchargé votre copie du jeu, voici un exemple de dossier de jeu de base terminé:

![Completed T5 Folder](/images/docs/install/NoAuNW9.png)

---

### Installation des DLC (BO1)

<Alert variant="warning">

Si vous avez installé le jeu via le torrent fourni dans les instructions précédentes alors [passez à la configuration dans le launcher](#configurer-t5-dans-le-launcher-plutonium).  
**Cette partie ne concerne que les personnes qui utilisent leurs fichiers Steam et qui ne possèdent pas les DLC**.  
Ce torrent ne fourni que les cartes des DLC. Vous ne pouvez pas jouer au jeu seulement avec ces fichiers. Si vous voulez télécharger le jeu alors [lisez au dessus](#installation-du-jeu-de-base-bo1)!  
Gardez en tête que si un serveur charge une carte des DLC et que vous ne l'avez pas installé vous serez exclu, si vous le pouvez il est donc préférable de les installer.

</Alert>

1. Téléchargez/ouvrez votre client torrent.
qBittorent Windows x64 est recommandé : [https://www.fosshub.com/qBittorrent.html](https://www.fosshub.com/qBittorrent.html)

2. Téléchargez le [fichier torrent](/t5_dlcs.torrent).

3. Ouvrez le fichier torrent `t5_dlcs.torrent` (téléchargé à l’étape précédente).  
Votre client torrent va s'ouvrir et vous demander où vous voulez enregistrer le jeu.  
**SÉLECTIONNEZ LE DOSSIER CALL OF DUTY BLACK OPS DANS VOS JEUX STEAM**

![img](/images/docs/install/bo1-qb.png)

4. Sélectionnez `"ne pas créer de sous-dossier"` dans la liste déroulante `"agencement du contenu"` (dans les anciennes versions de qBittorrent il faudra décocher `"créer un sous dossier"` ou `"conserver la structure du dossier"`)

![img](/images/docs/install/f32c04d072946509231016a435e9c521.png)

5. Démarrez le téléchargement et attendez que le téléchargement soit terminé.  
Vous saurez qu’il est terminé lorsque la barre de progression passe à `100%` et que le statut passe à `Émission` ou `Partage`.

---

### Configurer T5 dans le launcher Plutonium

Naviguez dans l'onglet Black Ops et cliquez sur **SETUP** et sélectionnez le dossier contenant les fichiers de Black Ops.  
Le dossier que vous devrez sélectionner s'appelera très probablement `pluto_t5_full_game` ou `Call of Duty Black Ops`.  
Ne sélectionnez pas votre dossier Games ou Jeux ou le dossier Documents. **Sélectionnez le dossier qui contient les fichiers de Black Ops !**
![BO1 in launcher](/images/docs/install/bo1-select-launcher.png)

* **Si vous utilisez vos fichiers Steam, il se trouvera à cet emplacement :** `{Lettre disque}\Program Files (x86)\Steam\steamapps\common\Call of Duty Black Ops`

* **Si vous utilisez le torrent** le dossier a sélectionner sera nommé `pluto_t5_full_game`

**(Si jamais vous avez besoin de resélectionner le dossier du jeu, cliquez simplement sur Game Settings à côté du bouton PLAY)**

---

### Erreur T5 : Chemin du jeu non valide

Si cette erreur s'affiche alors le dossier que vous avez sélectionné pendant le setup ne contient pas les fichiers du jeu.

![Invalid Game Directory](/images/docs/install/vlwamKe.png)

Si vous voyez cette erreur alors vous avez sélectionné votre disque tout entier au lieu du dossier du jeu.
`C:\` n'est pas le dossier de World at War.

![img](/images/docs/install/error-401.png)

Dans les deux cas, pour régler cette erreur vous devez cliquer sur Game settings dans le launcher et sélectionner le dossier qui contient les fichiers de World at War.  
Si vous n'arrivez pas à le trouver alors lisez à nouveau le [guide depuis le début](#t5-black-ops-1).

![img](/images/docs/install/MnkAcr8.png)

---

Vous avez maintenant terminé l'installation de BO1.  
Pour lancer BO1 ouvrez le launcher et cliquez sur PLAY.
