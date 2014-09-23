Créer une première "App"
========================

Structure de base
-----------------

A son plus simple niveau, une "App" est *un dossier* contenant un fichier `index.html`.
Celui ci représentera la page d'accueil de l'application.

Il est également possible de définir un fichier `manifest.json` qui apportera des informations supplémentaires
à SNAP! concernant le fonctionnement de votre application. Les détails concernant les informations présentes
dans ce fichier sont consultables [ici](manifest-app.md).

**Exemple d'arborescence**

```bash
mon_application/
  |-> index.html (obligatoire)
  |-> manifest.json (optionnel)
```

**index.html**

```
<html>
  <body>
    <h1>Ma première application SNAP</h1>
  </body>
</html>
```

"Installer" sa nouvelle App
---------------------------

Afin de pouvoir utiliser votre nouvelle application, déplacez votre dossier `mon_application` dans le sous dossier `apps` déjà présent dans le répertoire de l'application SNAP!

Cela devrait ressembler à peu prêt à ceci *(d'autres dossiers et/ou fichiers peuvent être présents)* :
```bash
snap/
  |-> config/
  |-> apps/
  |  |-> home/
  |  |-> wiki/
  |  |-> mon_application/
  |-> lib/
```

Tester
------

Lancez SNAP!.

En arrivant sur la page d'accueil, vous devriez voir:
![Écran d'accueil](images/premiere_app_img_1.png "Écran d'accueil")

Et en cliquant sur le bouton "Mon_application"
![Page principale de votre application](images/premiere_app_img_2.png "Page principale de votre application")
