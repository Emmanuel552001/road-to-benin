# Road to Benin — Site complet FR / EN

Ce dossier contient tout le code source du site, directement modifiable.
Site statique HTML / CSS / JavaScript : aucune compilation, aucun compte Sites,
aucune base de données et aucune dépendance à installer pour le déployer.

## Fichiers à modifier

- index.html : page française, textes, structure et descriptions des images.
- en.html : page anglaise, textes, structure et descriptions des images.
- style.css : couleurs, polices, tailles, mise en page et adaptation mobile.
- app.js : textes français et fonctionnement des quatre escales.
- app-en.js : textes anglais et fonctionnement des quatre escales.
- language.js : bouton EN / FR, conservation de la section consultée.
- assets/ : toutes les images, y compris les photos supplémentaires du PDF.

Modifiez les deux langues pour garder les contenus cohérents.
Les escales choisies sont conservées entre les langues dans sessionStorage.
Les textes ne sont pas traduits automatiquement.

## Tester sur son ordinateur

1. Décompressez le ZIP dans un dossier.
2. Ouvrez ce dossier dans votre éditeur de code, par exemple VS Code.
3. Lancez un serveur local à la racine du dossier (Live Server dans VS Code,
   ou, si Python est installé : python -m http.server 8000).
4. Ouvrez http://localhost:8000/ pour le français et
   http://localhost:8000/en.html pour l’anglais.

Un serveur local permet de vérifier correctement la navigation entre les pages.

## Redéployer ailleurs

Envoyez le contenu de ce dossier sur n’importe quel hébergement de fichiers
statiques. index.html doit se trouver à la racine du dossier publié, à côté de
en.html, des fichiers CSS / JS et du dossier assets.

Pour un hébergement demandant une configuration :
- type de projet : site statique / HTML ;
- commande de compilation : aucune ;
- dossier à publier : le dossier contenant index.html.

Le bouton anglais pointe vers en.html. Certains hébergeurs peuvent afficher
une URL simplifiée /en : cela est normal. Les images et les fichiers de style
utilisent des chemins relatifs pour permettre aussi un déploiement en sous-dossier.

L’accès privé de la version Sites est une configuration de cet hébergeur,
pas du code du site. Sur votre nouvel hébergement, configurez séparément
une protection d’accès si vous en souhaitez une.

## Polices et ressources

Toutes les images sont incluses. Les polices DM Sans et Playfair Display sont
chargées depuis Google Fonts via la première ligne @import de style.css.
Elles nécessitent Internet ; des polices de remplacement sont prévues.
Pour supprimer cette dépendance, retirez l’import et utilisez des polices
système, ou hébergez vous-même les polices avec leur licence.

Les textes et photographies proviennent du carnet fourni pour ce projet.
Le PDF original ne fait pas partie des fichiers nécessaires au site.

## Contenu du package

Le package contient les fichiers du site bilingue publié, sans identifiants
d’hébergement, jetons d’accès, configuration privée Sites ou historique Git.
Les fichiers HTML / CSS / JS sont les sources : aucune version compilée
supplémentaire n’est nécessaire.
