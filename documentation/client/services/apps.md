# Le service "apps"

Le service **apps** permet d'accéder aux différents éléments d'informations concernant les Apps disponibles sur le portail SNAP!.

## Utilisation

```javascript
Snap.ready(function(err, services) {

  // Commencer à utiliser le service
  services.apps.getAppsList(function(err, apps) {
    if(err) {
      // Quelque chose s'est mal passé...
    } else {
      // Faire quelque chose avec _apps_
    }
  });

});
```

## Méthodes

### apps.getAppsList(callback)

Récupère la liste des Apps disponibles sur le portail SNAP!

** Arguments **

- `callback(err, apps)` __Function__ La fonction de rappel qui sera invoquée lors de la réponse du service
  - `err` __Object__  Si différent de `null`, une erreur s'est produite lors de l'appel au service
  - `apps`  __[String,...]__ Tableau comprenant les identifiants des différentes applications disponibles sur le portail.

** Exemple **

```javascript
services.apps.getAppsList(function(err, apps) {
  if(err) {
    throw err; // Une erreur s'est produite
  }
  console.log(apps); // On affiche la liste dans la console
});
```

### apps.getAppManifest(appName, callback)

Retourne le [manifeste](../app-manifest.md) de l'application donnée si il existe.

** Arguments **

- `callback(err, manifest)` __Function__ La fonction de rappel qui sera invoquée lors de la réponse du service
  - `err` __Object__  Si différent de `null`, une erreur s'est produite lors de l'appel au service
  - `manifest`  __Object__ Le manifeste de l'application ou `null` si l'application n'a pas de manifeste.

** Exemple **

```javascript
services.apps.getAppManifest('home', function(err, manifest) {
  if(err) {
    throw err; // Une erreur s'est produite
  }
  console.log(manifest); // On affiche le manifest de l'application 'home' dans la console
});
```
