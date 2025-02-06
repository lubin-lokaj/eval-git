#  REGISTRE DE ILEY LEBIE

## Création du registre
Je créer mon registre dans mon bureau:
```shell
touch LEBIE.txt
```

##  Clonage du dépôt GitHub
Pour avoir accès au dossier qui a été créé dans github je fais la commande:
```shell
git clone "https://github.com/lubin-lokaj/eval-git.git"
```

##  Navigation dans le dossier et authentification
Je vais dans le dossier eval-git et je m'authentifie:
```shell
cd Documents
cd eval-git
git config user.email "iley.lebie@gmail.com"
git config user.name "iley24"
```

---

##  Création de ma branche
Je creer ma branche et je bascule dessus:
```bash
git checkout -b ileyLEBIE
```

##  Vérification de la création de la branche
Pour verifier que ma branche s'est bien crée, j'ai push un fichier .txt sur ma branche pour le voir afficher sur github:

```bash
touch text.txt
git add text.txt
git commit -m "Ajout d'un fichier pour créer la branche"
git push -u origin ileyLEBIE
```
mon identifiant et mon token en mdp

Je vois bien ma branche ileyLEBIE  affichée sur github.


## Renommage de la branche pour un nom fonctionnel
Vous nous avez informé qu'il fallait que le nom des branches soit
 fonctionnel donc j'ai renomé:

```shell
git branch -m ileyLEBIE branch_css_LEBIE
git commit -m "Modification du nom de la branche iley"
git push -u origin ileyLEBIE
```

##  Récupération de la partie HTML
```shell
git pull origin html_janis
```
Je récupère la branche contenant la partie HTML sur mon ordinateur.

## Push de ma partie css sur le depot

Je mets le tout sur vscode et je fais ma partie css. Une fois terminée j'enregistre et je push la partie css sur ma branche.
```shell
git add style.css
git commit -m "Ajout de la partie CSS"
git push -u origin branch_css_LEBIE
```
## Fusion de ma branche avec main
je me position dans la branche main et je fais la commande:
```shell
git merge branch_css_LEBIE
```
## Depot de mon registe sur le main
```shell
git add LEBIE.md
git commit -m "Ajout de mon registre"
git push -u origin main
```

