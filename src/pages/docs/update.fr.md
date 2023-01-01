# Comment mettre à jour Plutonium

## Mettre à jour le launcher Plutonium

Le launcher se met à jour tout seul lorsque vous le démarrez donc il est inutile d'essayer de le mettre à jour manuellement.  
L'updater s'ouvre pendant quelques secondes avant de démarrer le launcher si tout fonctionne normalement.
![img](/images/docs/update/update-2.png)

Si vous n'obtenez pas les mises à jours automatiquement, vous avez probablement épinglé le launcher pendant qu'il était lancé.
<br/>Pour régler ça suivez ces instructions :

1. Désépinglez Plutonium de votre barre des tâches/menu démarrer
2. Fermez votre jeu et le launcher
3. Epinglez `plutonium.exe` à votre barre des tâches/menu démarrer et démarrez le

## Vérifier si votre launcher est à jour

1. Ouvrez votre launcher et cliquez sur votre photo de profil en haut à droite
2. Ouvrez la [page de changelog](/docs/changelog/)
3. Comparez la Core version dans votre launcher et la dernière version sur le changelog.  
Si votre Core version est inférieure à celle sur le changelog alors vous n'êtes pas à jour.  

## Régler l'erreur "Failed to check for updates"

Cette erreur survient lorsque vous démarrez le launcher sans démarrer l'updater avant (souvent parce que vous avez épingler le launcher pendant qu'il était déjà lancé ou parce que quelque chose bloque la connexion à l'updater).  

Essayez ces méthodes une par une et dans l'ordre pour régler cette erreur :

### Méthode 1 (Bien épingler le launcher)
1. Rendez vous dans le dossier où `plutonium.exe` est situé (souvent dans les fichiers de votre jeu ou sur le bureau)
2. Supprimez les applications nommées `plutonium` et `plutonium.new` (si vous l'avez). Ces applications peuvent aussi avoir l'extension .exe si vous avez les extensions affichées dans Windows.
3. Suivez les instructions pour [mettre à jour le launcher](/docs/install/#plutonium-launcher)

### Méthode 2 (Changer de DNS)
[Changez votre DNS](https://lecrabeinfo.net/changer-les-dns-sur-windows-10.html) par celui de Google ou de Cloudflare par exemple.

### Méthode 3 (Antivirus)
Suivez les instructions sur la [page de documentation antivirus](/docs/antivirus/#how-do-i-fix-this-windows-defender) pour être sûr que votre antivirus ne bloque rien.

## Méthode 4 (VPN)
Si vous utilisez un VPN essayez de vous en déconnecter. Si vous n'utilisez pas de VPN essayez d'en utiliser un pour voir si cela vous permet de mettre à jour le launcher.
