---
layout: default
title: Cas d'usage
---

## Index

- [Traitement médical personnalisé du futur](#traitement-médical-personnalisé-du-futur)
- [Analyse intelligente de résultats CFD pour la conception aéronautique](#analyse-intelligente-de-résultats-cfd-pour-la-conception-aéronautique)
- [Prédiction de pannes pour le Data Center](#prédiction-de-pannes-pour-le-data-center)

# Traitement médical personnalisé du futur

## Partenaires impliqués

- ICO
- Atos-BULL
- ARMINES

## Présentation du cas d'usage

## Résultats obtenus

# Analyse intelligente de résultats CFD pour la conception aéronautique

## Partenaires impliqués

- Dassault Aviation
- Atos-BULL
- UGA

## Présentation du cas d'usage

Ce cas d'usage vise à étudier l'utilisation d'infrastructures hybrides Cloud-HPC pour des traitement de de données en lien avec l'aéronautique. Il s'agit plus particulièrement de déporter des calculs traditionnellement fait sur une plateforme HPC vers une plateforme Cloud. Nous considérons plus spécifiquement:

- Le post-traitement des données générées par des applications parallèles d'applications CFD
- La segmentation de séries temporelles correspondant aux données de vol d'aéronefs


## Résultats obtenus

- L'exécution sur plateforme Cloud de l'application de post-traitement des données de CFD, codée en MPI, est entièrement automatisée, ce qui inclut:
  - Le dimensionnement des machines virtuelles et leur réservation automatique sur Open Stack
  - Le déploiement et l'exécution de l'application au travers de conteneurs Docker
- La mise en oeuvre et l'évaluation d'un algorithme de segmentation de séries temporelle adapté au Cloud: 
  - Algorithme mis en oeuvre en utilisant Spark (Expression du parallélisme simplifié, équilibrage de charges et tolérance aux fautes automatique)
  - Capacité à traiter des séries temporelles de 30K valeurs en moins de 5 minutes
  
  
# Prédiction de pannes pour le Data Center

## Partenaires impliqués

- EasyVirt
- ARMINES
- UGA

## Présentation du cas d'usage

Dans ce cas d'usage, l'objectif est de construire des modèles d'IA
permettant de détecter des comportements anormaux dans des centres de
données au travers de la collecte de métriques système sur l'activité
des machines virtuelles. La plateforme HPC est utilisée pour accélérer
la phase d'apprentissage des modèles.


## Résultats obtenus

Nous avons conçu et développé une solution capable de détecter une très grande majorité des anomalies en générant très peu de faux positifs, en proposant une solution d'apprentissage non supervisée, basé sur deux briques de bases:

- KDetect: un algorithme de clustering itératif permettant d'identifier efficacement les séries temporelles anormales dans un ensemble de séries temporelles non annotées.
- Une brique Deep Learning, utilisant TensorFlow, qui construit un modèle capable d'analyser de nouvelles séries temporelles à partir des sorties de l'algorithme KDetect.
    
