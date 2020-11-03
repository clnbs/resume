# Curriculum vitea

## Sommaire
* [Introduction](#introduction)
* [Mes projets open source](#mes-projets-open-source)
* [Expériences précédentes](#expriences-prcdentes)
  * [L'école d'ingénieur](#lcole-dingnieur)
  * [Sunchain](#sunchain)
    * [Les projets de Sunchain](#les-projets-de-sunchain)
    * [Mes missions à Sunchain](#mes-missions--sunchain)
    * [En résumé](#en-rsum)
  * [Entreprenariat](#Entreprenariat)
* [Compétences](#comptences)

## Introduction

*Click [here](README.md) to find the english version.*

Vous pouvez me demander une lettre de recommandation par mail. Je suis actuellement à la recherche d'un poste en télétravail uniquement.

Comme vous l'avez sans doute constaté, je n'ai pas donné mon adresse personnelle car je veux réduire mon empreinte sur l'Internet. Si vous êtes intéressé par mon profil, je vous communiquerai toute information complémentaire dans les plus brefs délais. Vous pouvez me contacter par mail à <colin.bois@rocketmail.com>.

Vous pouvez trouver mon curriculum vitea [ici](assets/CV_fr.pdf).

## Mes projets open source
Je suis actuellement en train de travailler sur un seul projet :
 - [Autorace](https://github.com/clnbs/autorace) - Un jeu de course extensible (uniquement en anglais)
 
## Expériences précédentes
Dans cette section, je vais détailler les projets ou les expériences notables auxquelles j'ai pris part lors de ma courte carrière.

### L'école d'ingénieur
Pendant mon école d'ingénieurs, j'ai étudié plusieurs matières liées aux sciences informatiques :
 - les bases des systèmes Linux
 - les bases du Java, Python, PHP entre autres
 - la robotique côté logiciel
 - la maitrise du modèle OSI avec une bonne compréhension des couches basiques  (TCP, UDP, PPP, ARP, SMTP, IMAP, HTTP, etc ...)
 - maitrise des réseaux IPv4
 - une bonne compréhension des réseaux IPv6
 - programmation bas niveau
 - une bonne maitrise du langage c/c++
 - une maitrise de la programmation IoT (full stack, des capteurs jusqu'à la restitution des données)
 - maitrise du management d'équipe sur des méthodes agiles (Kanban, SCRUM, etc ...) avec plusieurs outils (Gitlab, Redmine, etc ...)
 - les bonnes pratiques de développement
 - théorie des graphes
 - théorie des langages
 - être un maker
 - maitrise des intelligences artificielle avec une certification :
   - algorithmes de classification
   - algorithmes de régression
   - algorithmes par cluster
   - algorithmes d'apprentissage machine
   
Toutes les compétences étaient testées pendant des projets de groupe. Ces projets étaient complexes avec des jalons très brefs pour savoir si nous étions capables de gérer le stress tout en étant capable de fournir une solution viable. 

### Sunchain
Mon expérience à Sunchain est, de loin, la plus satisfaisante expérience en tant qu'employé. Ma période à Sunchain a été un vrai challenge ainsi qu'une source d'inspiration.

> __Pendant que vous lisez les détails de mon expérience à Sunchain, gardez à l'esprit que j'étais le seul informaticien de l'équipe__

#### Les projets de Sunchain
Le projet initial de Sunchain est de partager de l'énergie provenant d'une centrale solaire construite entre plusieurs parties prenantes. Pour atteindre ce but, une blockchain par consortium a été déployée afin de collecter les données de production de la centrale et de consommation des participants pour finalement "séparer" l'énergie renouvelable.

Un futur projet de consommation d'énergie en itinérance via la blockchain de Sunchain était également dans les cartons.   

#### Mes missions à Sunchain
Lorsque j'ai été embauché, un prototype basique était déjà construit entièrement en Go, mais le développement était sous traité. Ma première mission consistait alors à internaliser les compétences informatiques afin de rendre la gestion de projets plus agile et être au plus proche des besoins de Sunchain. À l'époque, je n'avais jamais entendu parler de conteneurisation, de système haute disponibilité, micro-services ni du langage Go et je savais à peine de la technologie blockchain existait. J'ai dû apprendre par moi-même comme j'étais le seul informaticien de l'équipe, presque sans mentor : le freelance qui avait construit le MVP me donnait des conseils de temps en temps. Lorsque j'ai eu l'impression d'avoir accumulé assez de compétences, j'ai été en charge du management de l'infrastructure et de la disponibilité de service. J'ai été aussi chargé de la rédaction des solutions techniques adressées aux clients pour répondre aux cahiers des charges.

Ma deuxième mission était de construire un système de secours qui calculait le partage d'énergie entre les participants à la même manière des smarts contracts validés côté métier. Ce système de secours ne devait pas se reposer sur le système existant. Même si le style de code était loin d'être parfait, j'étais fière de mon système car c'était mon premier logiciel utilisé dans une entreprise.

Ma troisième mission était de développer une interface graphique pour les usagers afin de rendre visuelle l'énergie produite par la centrale, la quantité d'énergie attribuée aux participants, etc. Comme je suis un mauvais designer, nous avons fait développer cette interface par une entreprise tierce mais j'étais chargé de l'intégration dans notre infrastructure ainsi que du déploiement, de la validation des choix technologique et de la sécurité.

Ma quatrième mission était de remplacer les Raspberry PI, reliées au plus près aux compteurs, qui nous servaient de gateway et de demande de transaction blockchain lors de la phase de prototypage. J'ai effectué de longues veilles technologiques afin de trouver la meilleure board SoC avec un fort accent sur la sécurité matérielle et logicielle. Une fois la sélection faite, j'ai dû compiler un OS sur mesure, basé sur Debian à l'aide de Yocto Project. Cette expérience m'a permis d'apprendre en profondeur la programmation bas niveau ainsi que sur les systèmes d'exploitation Linux. La courbe d'apprentissage d'un tel projet peut être brutale, surtout lorsqu'on apprend seul.

Ma cinquième mission, reliée à la quatrième, était d'étendre les possibilités de connexion aux compteurs électriques en développent des solutions filaires et sans fil en fonction de la topographie du terrain de déploiement. J'ai déployé et opéré un réseau LoRaWAN pour les communications sans fil et étendu la connectivité filaire en ajoutant aux connexions USB des connexions RS-232, ModBus et un multiplexeur fabriqué en interne. Le multiplexeur a été fabriqué par un collègue ingénieur en électronique embauché pour l'occasion et j'ai écrit son firmware ainsi que son driver et son API en Go. Le multiplexeur était relié à plusieurs compteurs en RS-232 et à la gateway en I2C. Cette partie a été un véritable chalenge car nous devions être à la pointe de la technologie IoT avec des mises à jour sur le terrain sans intervention physique, être "chaos monkey" compatible avec un back-end haute disponibilité ; encore aujourd'hui, je suis fière de ce que nous avons accompli sur cette tâche.

Ma sixième et dernière mission principale était de changer la stack technologique DevOps et de mieux utiliser les services d'AWS. À cette période, Sunchain commençait à gagner des clients avec de la disponibilité de service contractuelle et, au même moment, j'ai commencé à me sentir comme un imposteur. Je n'avais pas, ou plus, confiance en mes compétences techniques et managériales. De plus, au même moment, je finissais mon école d'ingénieur et rédigeais mon mémoire de fin d'études ce qui me demandait beaucoup de temps de travail (de 12 à 14 h de travail par jours en semaine et 8 h durant les weekends au total) ce qui m'a rendu très stressé. Je ressentais également un besoin de faire des choses pour moi et de consolider les connaissances acquises durant ces trois ans passés à Sunchain et à l'école. J'ai donc notifié mes supérieurs de ma volonté de partir de l'entreprise et nous avons engagé un DevOps expérimenté que j'ai formé à notre système d'information en trois mois, au bout desquels il a finalement pris ma place.

#### En résumé
J'ai appris énormément lors de mes années "Sunchain" dans de nombreux domaines informatiques.

En tant que cadre informatique : 
 - veille technologique dans plusieurs domaines : projets open source (LoRaWAN par Brocaar, Hyperledger, Docker et Yocto Poject), les SoC, techniques managériales et bonnes pratiques de développement, IoT et outils de clusteurisation.
 - architecturisation de systèmes hautes disponibilités pour des applications cloud et les possibilités d'évolution
 - choix du stack technologique
 - cycle de vie d'un produit informatique de sa phase de prototype à sa phase de pré-industrialisation
 
En tant que manageur :
 - écrire des propositions techniques pour des clients
 - être une source de proposition pour une entreprise
 - management de stagiaires de tout niveau (bac +2 à bac +5)
 - gestion d'un budget
 
En tant que développeur :
 - management de la base de code d'une entreprise
 - sécurité informatique de l'infrastructure
 - être un autodidacte
 - appliquer un style de code et les best practices

### Entreprenariat
*En construction*

## Compétences 

![roadmap](assets/roadmap.png)
