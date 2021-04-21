---
layout: post
title:  "Git - Les commandes essentielles"
date:   2021-04-21 15:48:00 +0200
categories: [dev, git]
---
__pour voir les changement__

`git status`

### pour ajouter les nouveaux fichiers ou les fichiers modifiers
git add xxx

# commit dans la branche en cours
git commit -m "commentaires"

# passer sur la branche master
git checkout master

# fusion de la branche de dev dans le master
git merge branche_dev

# pousser le master dans le depot distant
git push origin master

# dans ce cas on pousse et on créé une nouvelle branche sur le dépot distant
git push -u repository_distant ma_branche_de_developpement

# créer une nouvelle branche à partir du master
git checkout -b nouvelle_branche

# pour vérifier que l'on est bien dans la branche souhaitée
git branch

# export
git archive --format zip --output=$HOME/export-mon-depot-git.zip master