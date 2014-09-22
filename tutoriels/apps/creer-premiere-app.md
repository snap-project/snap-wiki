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
mon_application
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

"Installer" son application
---------------------------
