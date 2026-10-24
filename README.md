# RAPPEL FANAFODY 2.0

Application Android hors-ligne de consultation de fiches médicaments et de rappels horaires.

**Auteur :** Serge Tsiatolaka RAZAFINDRABE  
**Titre :** Diplômé en Sciences infirmières  
**Contact :** 034 64 463 60 — rtfserge@gmail.com

## Contenu
- `app/src/main/assets/medicaments.json` : base fournie, 2 862 fiches.
- Recherche par nom commercial, DCI, laboratoire et présentation.
- Fiches : action, indications, posologie, contre-indications, précautions, interactions, remarques, conservation et sources.
- Photo fournie utilisée comme arrière-plan estompé.
- Création d'un rappel à une heure choisie avec notification Android.
- Aucun accès Internet requis à l'exécution.

## Générer l'application
1. Installer Android Studio (version récente) et un JDK 17.
2. Ouvrir ce dossier comme projet Gradle.
3. Laisser Gradle synchroniser les dépendances (Internet requis uniquement pour la première compilation).
4. Dans **Build > Build APK(s)**, générer l'APK de débogage. Il se trouve généralement dans `app/build/outputs/apk/debug/app-debug.apk`.

## Limites importantes
- Le projet source est fourni ; aucun APK compilé n'est inclus dans cette archive.
- Les rappels actuels sont des alarmes ponctuelles : l'interface les mémorise, mais ne reprogramme pas automatiquement une répétition quotidienne. Redémarrage du téléphone et restrictions constructeur peuvent aussi affecter les alarmes.
- Le rappel sert à notifier une heure définie par l'utilisateur, pas à déterminer une prescription. Il ne remplace pas une ordonnance, le RCP ni la validation par un professionnel habilité.
- Les fiches importées peuvent contenir des informations génériques ou non validées pour une spécialité. Toujours vérifier les sources, les contre-indications et la posologie avant toute décision clinique.
- Les résultats de recherche sont limités aux 500 premières fiches correspondantes pour préserver la fluidité ; la base complète est embarquée.