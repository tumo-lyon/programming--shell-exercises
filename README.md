# Exercices shell

Réalise ces exercices en commandes shell pour te familiariser avec celles-ci.

### Cheatsheet des commandes vues aujourd'hui

| Commande | Utilité | Exemple |
| -------- | ------- | ------- |
| `ls`       | Liste le contenu d'un répertoire |
| `ls -l`    | Liste le contenu d'un répertoire avec des détails |
| `mkdir`    | Crée un répertoire | `mkdir mon_dossier`
| `cd`      | Change de répertoire | `cd mon_dossier`
| `touch`    | Crée un fichier vide | `touch mon_fichier.js`
| `rm`       | Supprime un fichier | `rm mon_fichier.js`
| `rm -r`    | Supprime un dossier de manière récursive | `rm -r mon_dossier`
| `pwd`      | Montre le répertoire actuel |
| `cp`       | Copie un fichier | `cp mon_fichier.js mon_fichier_copie.js`
| `cp -r`    | Copie un dossier de manière récursive | `cp -r dossier_source dossier_destination` |
| `tar -cf`  | Crée une archive | `tar -cf monArchive.tar mon_fichier.js mon_dossier `
| `tar -xf`  | Extrait une archive | `tar -xf monArchive.tar` |


### Cheatsheet des commandes Git

| Commande | Utilité | Exemple |
| -------- | ------- | ------- |
| `git status` | Affiche le status du répositoire actuel |
| `git log` | Affiche le log de tous les commits |
| `git add` | Ajoute un fichier/dossier à être commit | `git add mon_fichier.txt dossier_source`
| `git commit -m` | Commit les fichiers avec un message | `git commit -m "Bugs réglés et code trié"`
| `git push` | Push les changements locaux sur le serveur |


## 1. Crée un fichier texte 

Dans le dossier racine de ce projet, créer un fichier nommé `HelloTumo.txt`.

Tu peux vérifier qu'il a bien été créé avec `ls`.

## 2. Crée un dossier

Maintenant crée un dossier `Prenom-Nom` à ton nom.

Tu peux vérifier qu'il a bien été créé avec `ls`.

Ensuite 'rentre' dans ce dossier. 

## 3. Copier un fichier

En restant dans ton nouveau dossier, copie le fichier `HelloTumo.txt` dans celui-ci.

Tu peux vérifier qu'il a bien été créé avec `ls`.

Ensuite reviens au dossier racine.

## 4. Décompresser une archive

Décompresse l'archive `myCodeProject.tar` dans un dossier `myCodeProject`.

Tu peux vérifier qu'il a bien été créé avec `ls`.

## 5. Copier un dossier

Copie le dossier (Récursivement) `source` qui réside dans `myCodeProject`, dans un dossier `Prenom-Nom/sorted_source`.

Tu peux ensuite aller dans ce dossier `Prenom-Nom`.

## 6. Trier les fichier

Maintenant il va falloir trier les fichier dans le dossier `Prenom-Nom/sorted_source`, car le stagiaire a fais des bêtises avec le code source. Celui-ci a fais des copier-coller sans faire attention et maintenant le code source est mélangé à plein de copies.

Supprimes tous les fichiers qui sont des copies (Les fichiers terminants par `copy.ts`).

Pour vérifier que tu as bien trié les fichiers, exécute la commande suivante dans le dossier `sorted_source`:

```
ls -l | wc -l
```

La commande dois retourner '35'.


#### Note:
Si tu as supprimé des fichiers qu'il ne fallait pas ou que tu rencontres un problème, supprimes le dossier `sorted_source` et recommence à l'étape 5.


## 7. Crée une archive

Maintenant que ton code est trié, compresses ton dossier `Prenom-Nom` dans une archive `Prenom-Nom.tar` à la racine du projet.

## 8. Commit

Enfin, ajoute toutes les modifications avec Git, et fais un commit.

## Bonus 

Si tu as le temps, recommence à zéro et refais toutes les étapes mais cette fois-ci, fait un commit à chacune d'entre-elles pour détailler tes actions.

**Lectures bonus:**
Pipes - https://www.howtogeek.com/438882/how-to-use-pipes-on-linux/

Redirections - https://www.gnu.org/software/bash/manual/html_node/Redirections.html

