# Projet : Classification supervisée des essences forestières à partir de la BD Forêt® version 2.0 et des images Sentinel-2

## Contexte

La **BD Forêt® version 2.0** est une base de données géographique de référence pour décrire les formations végétales forestières et naturelles en France. Elle repose sur une photo-interprétation des images en infrarouge couleurs de la **BD ORTHO®** et fournit une description précise des essences forestières et de la densité de leur couverture pour des zones supérieures à 5 000 m² (0,5 hectare). Ce référentiel est largement utilisé par les acteurs des secteurs de la forêt-bois, de l’environnement, de l’aménagement du territoire et du développement durable. Il intervient dans divers projets comme :

- L’évaluation de la ressource et de la qualité de l’environnement,
- La prévention des risques,
- La gestion durable des forêts,
- La connaissance de la biodiversité et des continuités écologiques.

Cependant, la **BD Forêt®** présente des limites : elle n’est pas régulièrement mise à jour et ne permet pas une cartographie des essences forestières à une échelle intra-peuplement.

Avec l’utilisation de compétences en télédétection et des séries temporelles d’images Sentinel-2, ce projet vise à surmonter ces limites.

---

## Objectifs

1. **Évaluer l’utilisation de la BD Forêt® version 2.0 comme source d’échantillons de référence** pour effectuer une classification supervisée de séries temporelles d’images Sentinel-2.
2. **Réaliser une classification supervisée à l’échelle du pixel** et agréger les résultats à l’échelle des peuplements de la BD Forêt®.
3. **Évaluer la qualité des cartes produites** à l’échelle des pixels et des peuplements.

### Étapes du projet

1. **Téléchargement des images Sentinel-2** : Acquisition des données satellites nécessaires.
2. **Pré-traitement des images** : Correction radiométrique, géométrique, et génération des indices pertinents.
3. **Préparation des échantillons à partir de la BD Forêt®** : Extraction et structuration des données de référence.
4. **Classification supervisée** : Création et application d’un modèle de classification pour identifier les essences forestières.
5. **Agrégation des résultats** : Passage des informations classifiées à une échelle plus large (peuplements).
6. **Évaluation des performances** : Comparaison des cartes produites avec des données de validation.

## Dépôt Git

Tous les scripts développés doivent être déposés dans ce dépôt Git. Ce dépôt servira pour :

1. **Sauvegarder les travaux** : Connectez votre dépôt Git à vos instances VSCode pour une sauvegarde régulière.
3. **Travailler collaborativement** : Profitez des fonctionnalités Git pour faciliter le travail d’équipe.

### À rendre à la fin du projet :

- **Lien vers le dépôt Git**, contenant tous vos scripts et éventuels documents associés.

---

## Connexion entre Onyxia et Github

- Une fois que vous avez lancé VSCode (https://datalab.sspcloud.fr/launcher/ide/vscode-python?name=vscode-python-projet&version=2.1.15&s3=region-ec97c721&init.personalInit=%C2%ABhttps%3A%2F%2Fframagit.org%2Fcours1%2Fsigmam2_telea%2F-%2Fraw%2Fmain%2Fint_env_telea_project.sh%3Fref_type%3Dheads%C2%BB&autoLaunch=true) depuis Onyxia, ouvrez le terminal et configurez le git :
  - git config --global user.name "VotreNom"
  - git config --global user.email "VotreEmail@example.com"
- Dès lors, clonez le dépot github :
  - git clone https://github.com/tpottelet/Projet_Teledetection.git

## Importer les images

- Créer un dossier "images" dans "data"
- Dans le terminal, écrire "mc cp -r s3/thomaspottelet/diffusion/images /home/onyxia/work/data"

## Télécharger Git LTS pour les fichiers volumineux

- Github n'accepte pas les fichiers faisant plus de 100Mo. Pour palier à celà, il faut installer Git LTS sur le lien suivant : https://git-lfs.com/
- Une fois téléchargé, suivre les étapes suivantes sur le terminal vscode :
  - git lfs install
  - git lfs track "*.psd"
  - git add .gitattributes

## Notes importantes

- Sauvegardez vos données localement à la fin de chaque session.
- Suivez une méthodologie rigoureuse pour le traitement des données et la validation des résultats.
- N’hésitez pas à travailler en équipe pour bénéficier des apports collaboratifs.

---

## Ressources supplémentaires

- Scripts Python disponibles dans vos environnements de travail.
- Documentation Sentinel-2 et BD Forêt® pour approfondir vos connaissances.

---

**Bon courage !!**
