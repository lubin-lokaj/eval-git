#Registre 

Récupération du dépôt distant sur le dépôt local : `git clone https://github.com/lubin-lokaj/eval-git.git`
```shell
git config user.email "lubin.lokaj@gmail.com"   
git config user.name "lubin-lokaj"
```

```shell
git branch lubin   
git checkout lubin   

git touch LOKAJ_Lubin_registre 

git add LOKAJ_Lubin_registre

git commit -m "création du registre et test"

git push -u origin lubin   
``` 
(ça a push sur ma branche les 3 fichiers de base plus le registre, j'ai décidé de supprimer la branche)   

```shell
git checkout main   
git branch -d lubin   

git push origin --delete lubin   
```

J'ai réessayé en créant un dossier registre avec le fichier dedans, mais ça a aussi mis les 3 fichiers de base. J'ai donc re supprimé   

```shell
git checkout main   
git branch -d lubin   

git push origin --delete lubin   
```

J'ai recréé une branche : mobile-lubin   

```shell
git branch mobile-lubin   
git checkout mobile-lubin   
git add LOKAJ_Lubin_registre   
git commit -m "Création du fichier, ajout des premières manips et test"   
git push -u origin mobile-lubin   
```

J'ai changé l'extension d'un fichier txt à md (en ayant changé le contenu avant) `mv LOKAJ_Lubin_registre LOKAJ_Lubin_registre.md`

J'ai remis ce fichier sur le git

```shell
git add LOKAJ_Lubin_registre.md
git commit -m "Changement du contenu et de l'extension de txt à md"
git push -u origin mobile-lubin
```

J'ai esnuite supprimé le fichier déjà existant sur git

```shell
git rm LOKAJ_Lubin_registre
git commit -m "Suppression du fichier"
git push -u origin mobile-lubin
```

Récupération des fichiers html et du css 

```shell
git pull origin html_janis
git pull origin html-andrea
git pull origin branch_css_LEBIE
```

Réalisation du fichier mobile.css et envoi sur github

```shell
git add mobile.css
git commit -m "Réalisation du fichier css pour mobile
git push -u origin mobile-lubin
```


Fusion des branches 

```shell
git checkout main
git merge html_janis
git merge html-andrea
git merge branch_css_LEBIE
git merge mobile-lubin
```

Pour celle d'andréa on a du forcer : `git merge NOM_DE_LA_BRANCHE_SOURCE --allow-unrelated-histories`
