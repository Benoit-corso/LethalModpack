### __Pour ceux que ca intéresse, j'ai fait un modpack vanilla+, ce que fait ce package:__
```
- Mis a jour de BepInEx en v5.4.23.2
- Tout les mods contenus sont a jour pour Lethal Company v64 et vérifiés (sans bugs)
- Inclus Emotes, Cosmetics, Suits.
- Inclus quelques ennemies et planetes.
- Inclus des hotfixes pour plus de performance, stabilité et QoL.
- Il reste quelques erreurs (faux positifs pour la plupart) dans la console.
```
Il a pour but d'être une base a de nouveau modpacks tout en restant stable.

Je précise, que la majeure partie du travail réside a sélectionner les mods qui sont toujours valide a ce jour.

Pour ceux qui veulent uniquement jouer, les 3 premiers étapes sont suffisante.

### Prérequis:
```
- Lethal Company v64 (dernière mise a jour en date - 16/10/2024)
- r2modman
```
## Grand 1
Vous devez importer le modpack avec ce code: __019296ce-8d68-f227-4c8c-ddf603bd7703__
## Grand 2
il faut ouvrir le zip que je vous fourni, puis aller dans:
```
%AppData%\r2modmanPlus-local\LethalCompany
```
## Grand 3
Et enfin écraser les fichiers en faisant un copier-coller. (comme sur l'image - Ecraser.png)

___

__Si jamais vous souhaitez ajouter d'autres mods__ (tout d'abord faites attention aux dépendances)
Des le premier mod installé r2modman aka thunderstore, risque de remplacer le nouveau BepInEx, dans le doute il faut extraire la dernière version de BepInEx dans le profile:
```
%AppData%\r2modmanPlus-local\LethalCompany\profiles\Very Lethal Company
```
__Pour les mods qui ajoutent uniquement des assets__ (sans nouvelle dépendance - Dependance.png) c'est ok vous n'avez rien a faire.

___

Sinon veillez bien a patcher le mod en question pour qu'il utilise le nouveau BepInEx:
```
%AppData%\r2modmanPlus-local\LethalCompany\profiles\Very Lethal Company\BepInEx\plugins\<nom-du-mod>\manifest.json
```
Et également le mods.yml, pour la même raison.
```
%AppData%\r2modmanPlus-local\LethalCompany\profiles\Very Lethal Company\mods.json
```
Voir: MauvaisManifest.png, BonManifest.png
Généralement, il faudra juste remplacer "BepInEx-BepInExPack-5.4.2100" par "NoxCorp-BepInExPack-5.4.2302"
un ctrl+f avec le bloc note est largement suffisant.
___

Si il y a du monde convaincu par tout ca, je ferais un script pour patcher automatiquement les fichiers, j'ai demandé a thunderstore ils ne veulent pas ajouter la mise a jour, donc je me suis permis de vous partager cela.
