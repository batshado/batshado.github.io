---
layout: post
title:  "Git - Les commandes essentielles"
date:   2021-04-21 15:48:00 +0200
author: batshado
categories: [dev, git]
---
#### Voir les changements
`git status`


#### Valider l'ajout de nouveaux fichiers ou la modification de fichiers existants
`git add xxx`


#### Effectuer un _commit_ dans la branche en cours avec ajout d'un commentaire
`git commit -m "commentaires"`


#### Changer de branche (par exemple passer sur la branche _master_)
`git checkout master`

#### Fusion d'une branche avec la branche courante
`git merge branche_dev`

#### Mettre à jour le dépot distant (dans cet exemple c'est la branche master distante)
`git push repository_distant master`

#### Mettre à jour le dépot distant et créer une nouvelle branche distante
`git push -u repository_distant ma_nouvelle_branche_distante`

#### Créer une nouvelle branche à partir de la branche courante
`git checkout -b nouvelle_branche`

#### Pour dans quelle branche nous sommes (et aussi voir la liste des branches locales)
`git branch`

#### Créer un export
`git archive --format zip --output=$HOME/export-mon-depot-git.zip master`