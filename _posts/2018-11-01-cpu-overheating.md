---
title:  "CPU overheating characterization in HPC systems: a case study"
tags: ['index', 'HPC']
---

Avec l'augmentation de la taille des supercalculateurs, le nombre d'évènements anormaux a aussi augmenté. Certains de ces évènements conduisent au dysfonctionnement d'une application. D'autres simplement posent des problèmes d'éfficacité du système. La surchauffe du CPU est l'un des évènements impactant négativement la performance d'un système : quand un CPU surchauffe, sa fréquence diminue. Ce papier étudie le problème de surchauffe de CPU dans les supercalculateurs. 
Dans la première partie, nous analysons les données collectées sur un an d'un supercalculateur de la top500 afin de comprendre dans sous quelles conditions la surchauffe CPU intervient.
Notre analyse montre que les évènements conduisant à une surchauffe sont dus à certaines applications spécifiques. 
Dans la seconde partie, nous évaluons l'impact tels évènements sur la performance des applications MPI.
En utilisant 6 benchmarks HPC représentatifs, nous montrons que pour la majorité des applications, la baisse de fréquence d'un CPU impacte le temps d'exécution des exécutions distribuées proportionnellement à la durée et à l'ampleur de la baisse de fréquence. 
Ce papier a été publié au **workshop FTXS co-localisé avec la conférence SuperComputing 2018**. 