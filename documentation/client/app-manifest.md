## Le fichier "manifest.webapp"

Les Apps peuvent avoir à la racine de leur répertoire un fichier `manifest.webapp`. Ce fichier au format JSON contient des métadonnées décrivant l'App et son contexte.

Dans la mesure du possible, SNAP! essaye de suivre le format [manifest.webapp](https://developer.mozilla.org/en-US/Apps/Build/Manifest?redirectlocale=en-US&redirectslug=Web%2FApps%2FManifest)  décrit sur le [Mozilla Developper Network](https://developer.mozilla.org/).

*Plus d'informations à venir.*

**Exemple:** manifeste de l'application "home" par défaut
```json

{
  "name": "Accueil",
  "description": "Page d'accueil de SNAP!",
  "default_locale": "fr",
  "locales": {
    "en": {
      "name": "Home",
      "description": "Home App"
    }
  }
}
```
