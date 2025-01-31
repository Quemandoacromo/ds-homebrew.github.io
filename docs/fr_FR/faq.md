# FAQ

## Dois-je faire une mise à jour du système ?

It is **not** recommended to update your DSi unless you know there are purchased DSiWare. Il est toujours possible de suivre ce guide si vous le faites, mais le seul avantage de la mise à jour est la possibilité d'accéder à la boutique Nintendo DSi pour retélécharger des titres déjà achetés. Tous les autres avantages, comme l'intégration de Facebook dans l'application Appareil photo Nintendo DSi, ne sont plus utilisables ou ne sont pas suffisamment importants pour justifier les inconvénients :

- Installing System Updates is known to occasionally **brick** consoles, with roughly the same frequency as when installing Unlaunch
- Il n'est plus possible d'utiliser des exploits plus anciens, ce qui peut être nécessaire si vous ne pouvez pas utiliser les exploits recommandés
- La compatibilité des linkers est réduite, mais cela peut être contourné si vous installez Unlaunch

## Quel est le meilleur exploit ?

Unlaunch est globalement le meilleur exploit pour la DSi, le seul inconvénient étant qu'il y a un risque mineur de brick à l'installation. En général, il est recommandé d'utiliser Memory Pit pour installer Unlaunch. Si vous voulez éviter tout risque, il est recommandé d'utiliser plutôt Flipnote Lenny car il a moins de problèmes que Memory Pit avec les homebrews, tout en étant tout aussi sûr et simple à supprimer. Vous trouverez ci-dessous une liste des avantages et des inconvénients de chaque exploit :

### Memory Pit

Avantages :

- Rapide et simple d'utilisation
- Aucun risque d'endommager la console, la désinstallation est aussi simple que de retirer la carte SD ou de supprimer un fichier
- Compatible avec toutes les consoles DSi, à moins qu'elles n'aient un appareil photo cassé et qu'elles n'aient pas terminé le tutoriel sur l'appareil photo

Inconvénients :

- Nécessite le lancement de l'appareil photo DSi chaque fois que vous voulez accéder à un homebrew
- Incompatible avec certains titres en mode DSi et homebrews car la WRAM n'est ouverte qu'au processeur ARM7
- L'accès au Slot-1 (la carte de jeu DS) est bloqué dans les homebrews
- L'accès au DSP est bloqué, ce qui entraîne une dégradation du son dans GBARunner2
- Les photos sur la carte SD ne peuvent pas être visualisées dans l'appareil photo DSi lorsque Memory Pit est installé, car c'est le déclencheur de l'exploit
  - The only way to view SD card photos while Memory Pit is installed, is to launch a ROM dump of the DSi Camera application using **TW**i**L**ight Menu++ to boot it via nds-bootstrap (v0.61.3 or later)

### stylehax

Avantages :

- Meilleure compatibilité avec les titres en mode DSi et homebrews que Memory Pit
- Facile à utiliser
- Aucun risque d'endommager la console
- Utilisable sur les consoles avec un appareil photo cassé
- Meilleur son dans GBARunner2

Inconvénients :

- Nécessite un accès à Internet
- Nécessite de charger le Nintendo DSi Browser chaque fois que vous voulez accéder à un homebrew, ce qui prend un peu plus de temps que Memory Pit
- L'accès au Slot-1 (la carte de jeu DS) est bloqué dans les homebrews

### Flipnote Lenny

Avantages :

- Meilleure compatibilité avec les titres en mode DSi et homebrews que Memory Pit
- Aucun risque d'endommager la console, la désinstallation est aussi simple que de retirer la carte SD ou de supprimer un dossier
- Utilisable sur les consoles avec un appareil photo cassé
- Meilleur son dans GBARunner2

Inconvénients :

- Nécessite le chargement de Flipnote Studio chaque fois que vous voulez accéder à un homebrew, ce qui prend un peu plus de temps que Memory Pit
- L'accès au Slot-1 (la carte de jeu DS) est bloqué dans les homebrews

### Unlaunch

Avantages :

- Permet de lancer les homebrews et DSiWare immédiatement au démarrage du système, avec des boutons de raccourci facultatifs
- Accès complet au système sans aucune restriction, y compris :
  - Accès au Slot-1 permettant de dumper les cartes de jeu et de charger des linkers incompatibles
  - Meilleur son dans GBARunner2
- Supprime les verrouillages régionaux sur les cartes de jeu optimisées/exclusives DSi
- Protection contre la plupart des risques de brick de la DSi
- Les jeux optimisés DSi peuvent être exécutés en mode DSi sans ROM donatrice
- Les anciens homebrews peuvent être exécutés via nds-bootstrap-hb

Inconvénients :

- Very minor risk of **bricking** the console when installing
- Another, slightly higher, risk of bricking if you decide to [uninstall it](uninstalling-unlaunch.html)
- Non compatible avec les consoles de développement

## Est-ce que je perdrai des fonctionnalités en moddant mon système ?

Si vous installez Unlaunch ou utilisez Flipnote Lenny, vous ne perdrez aucune fonctionnalité. If you use Memory Pit, you will be unable to view photos on the SD card using the DSi Camera, unless you launch a ROM dump of the DSi Camera application using **TW**i**L**ight Menu++ to boot it via nds-bootstrap.

- To regain the ability to view your SD card photos when launching the DSi Camera from the DSi Menu, install Unlaunch or switch to a different exploit, then delete Memory Pit's `pit.bin` file
  - If `tip.bin` exists in the same folder, rename it back to `pit.bin`

## Comment puis-je jouer aux dumps de cartes de jeu Nintendo DS ?

La lecture des dumps de cartes de jeu sur la console nécessite l'utilisation d'un linker ou de nds-bootstrap, un programme qui permet de jouer à partir de la carte SD interne en redirigeant les lectures et les écritures du Slot-1 vers celle-ci.

- Avec TWiLight Menu++, vous pouvez naviguer sur votre carte SD pour trouver des fichiers ROMs à jouer avec nds-bootstrap. L'avantage d'utiliser TWiLight Menu++ est d'avoir un menu de triche, des paramètres par jeu et d'éviter les restrictions apportées par les forwarders. En d'autres termes, vous pouvez déposer vos fichiers ROMs directement et les lire sans aucune configuration. Il n'y a pas de limite de 39 titres, ni hiyaCFW ou Unlaunch ne sont nécessaires et il n'y a aucune restriction sur l'espace libre de la carte SD que vous pouvez avoir
- hiyaCFW users can create forwarders for the SDNAND's DSi Menu using the [DS Game Forwarders](https://wiki.ds-homebrew.com/ds-index/forwarders?tab=tab-dsi-sd-card) guide on the DS-Homebrew Wiki, but it has some limitations. Il y a une limite stricte de 39 titres, et ils sont moins pratiques à réaliser qu'en utilisant TWiLight Menu++
  - If you do not have hiyaCFW and would like to use forwarders, you can follow the [hiyaCFW installation guide](https://wiki.ds-homebrew.com/hiyacfw/installing) on the DS-Homebrew Wiki

## Comment puis-je mettre à jour mes homebrews ?

- **Unlaunch** - Follow the instructions on the [Installing Unlaunch](installing-unlaunch.html) page
  - You do **not** need to uninstall Unlaunch before doing this
- **hiyaCFW** - Replace `hiya.dsi` on the root of the SD card from the [updated release](https://github.com/RocketRobz/hiyaCFW/releases)
- **TWiLight Menu++** - Follow the instructions on the [DS-Homebrew Wiki](https://wiki.ds-homebrew.com/twilightmenu/updating-dsi)
- **nds-bootstrap** - Copy `nds-bootstrap-hb-release.nds` & `nds-bootstrap-release.nds` to the `_nds` folder on the root of your SD card
  - Si vous utilisez TWiLight Menu++, il y a beaucoup de chance que la dernière version de nds-bootstrap soit incluse avec celui-ci
- **GodMode9i, dumpTool, Forwarder3-DS, etc** - Follow the instructions used to download them

D'autres homebrews peuvent utiliser d'autres méthodes de mise à jour.

## Je suis nouveau ou je voudrais refaire mon installation. Par où dois-je commencer ?

- Si vous n'avez pas encore modifié votre console ou si vous cherchez à mettre à jour Unlaunch sur votre système, nous vous recommandons de commencer par le début du guide et de suivre les pages. Assurez-vous de lire tout ce qui figure sur la page d'accueil
- If you have the latest version Unlaunch, follow the [TWiLight Menu++ install guide](https://wiki.ds-homebrew.com/twilightmenu/installing-dsi) to set up TWiLight Menu++ on your system

## Comment puis-je supprimer le contrôle parental ?

- The [mkey generator](https://mkey.salthax.org) can generate the code required to remove parental controls

## Puis-je changer la région de ma Nintendo DSi ?

Oui, il existe plusieurs méthodes différentes selon ce que vous voulez changer :

- La méthode la plus sûre et la plus simple est tout simplement d'installer TWiLight Menu++, il peut utiliser n'importe quelle langue officielle et plus encore sans nécessiter de modifications de la NAND
- If you want to actually change the system region and are using hiyaCFW, open the config menu, and change the region setting (not possible with CHN and KOR NANDs)
  - If this breaks touch input, revert the region setting back to the original, and you can instead use Yoti's [hiyalang](https://github.com/Yoti/cli_hiyalang/releases) for Asian DSi systems. For American DSi systems use [this version of hiyalang](https://github.com/Simonsator/cli_hiyalang/releases/)
- Lastly, if you want to change the region on the actual system NAND, you can use Mighty Max's [DSi Language Patcher](https://gbatemp.net/threads/release-dsi-language-patcher.582836/)

## Qu'est-il arrivé au guide d'installation de hiyaCFW ?

Because hiyaCFW does not serve much functional purpose and was a problematic and confusing part of the guide for many users, it was moved to the [DS-Homebrew Wiki](https://wiki.ds-homebrew.com/hiyacfw/installing).

- Si le lien vers la page en question provient d'un autre guide, les instructions que vous suiviez étaient très probablement périmées. Veuillez plutôt utiliser ce guide, car il est maintenu en permanence par les développeurs de ces projets

## Qu'est-il advenu de Lazy DSi Downloader ? Comment puis-je installer un CFW sans lui ?

Lazy DSi Downloader était un programme qui vous permettait essentiellement de sauter le processus d'installation manuelle en téléchargeant et en plaçant les fichiers et dossiers nécessaires sur votre carte SD. Toutefois, en raison de la manière dont il a été programmé et distribué, de nombreux utilisateurs ont rencontré divers problèmes et ont fini par devoir procéder à une installation manuelle, car cela était plus rapide et/ou plus facile que de réparer ce qui causait le problème.

To avoid more users encountering these issues, we no longer recommend using Lazy DSi Downloader, and instead [doing the manual setup](get-started.html) is the recommended way to go.

- Si vous avez été redirigé vers ce guide par un tiers qui recommandait l'utilisation de Lazy DSi Downloader, les instructions que vous avez suivies étaient probablement obsolètes. Utilisez plutôt ce guide, qui est constamment mis à jour par les développeurs de ces projets.

## Quel type de carte SD dois-je utiliser ?

- Vous devez acheter une carte SD d'une marque de confiance
- Une carte SD de taille normale ou une carte microSD avec un adaptateur fonctionneront toutes les deux
- Toute capacité comprise entre 1 Go et 2 To fonctionnera. Pour un usage général, 8 Go suffisent
  - Certains logiciels, comme hiyaCFW, peuvent avoir des temps de chargement plus longs avec des cartes SD de plus grande capacité
- La classe de vitesse 8 ou plus est recommandée

## Puis-je utiliser ma carte SD DSi sur d'autres systèmes ?

En général, oui, à deux exceptions près :

- hiyaCFW ne fonctionnera que sur le système pour lequel il a été configuré
- Même si vous utilisez nds-bootstrap ou un linker, les codes amis dans les jeux DS en ligne seront réinitialisés si vous tentez de vous connecter en utilisant une autre console

## Comment passer à une nouvelle carte SD après avoir configuré un homebrew ?

Format your new SD card using the [SD Card Setup](sd-card-setup.html) instructions, then simply move your data from the old SD card to the new one.

## Puis-je toujours utiliser mon système normalement sans la carte SD insérée après avoir configuré un homebrew ?

Oui. Si vous n'avez pas installé Unlaunch, votre système ne sera pas du tout modifié. If you _did_ install Unlaunch, you may need to [configure Unlaunch](installing-unlaunch.html#section-iii-post-unlaunch-configuration) to automatically boot the original DSi Menu under specified conditions.

## The [Unlaunch page](https://problemkaputt.de/unlaunch.htm) says that version 2.0 is not known to be safe. Dois-je utiliser une version antérieure à la place ?

The Unlaunch page has not been updated since version 2.0 was released in 2019. La grande majorité des utilisateurs ne rencontrent aucun problème avec cette version, qui est donc considérée comme sûre.

## Comment puis-je exécuter un DSiWare dumpé ?

La méthode recommandée est de simplement les lancer avec TWiLight Menu++, en raison de la méthode simple de glisser-déposer et du fait qu'il n'y a pas de limite arbitraire. Lorsque nds-bootstrap est défini comme méthode de lancement, il bénéficie également des avantages des triches et des captures d'écran, ainsi que de tout autre avantage fourni par le menu du jeu.

However, for the few titles that are incompatible, you can use [NTM](https://github.com/Epicpkmn11/NTM/releases) to install them on either internal memory or [hiyaCFW's SDNAND](https://wiki.ds-homebrew.com/hiyacfw/installing). En plus de l'absence des avantages ci-dessus, il y a également une limite de 39 titres dont la taille ne peut pas dépasser 128 Mio/1 024 blocs. Pour SysNAND, il y a également un très faible risque de bricker le système lors de l'écriture sur la NAND interne.
