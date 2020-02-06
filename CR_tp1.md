#Premier TP d'Admninistration Système#

##Exercice 2##

###Manuel###

1) La commande "which" renvoie le chemin d'un éxécutable mis en argument.
2) Lorsqu'on lit une page du manuel, on peut rechercher du texte en tapant "/textevoulu" en lingue de commande.
3) On sort du manuel en appuyant sur la touche "q".
4) La page d'introduction de la section 6 nous inquide que celle-ci parle de jeux et programmes de divertissements présents sur le système.

###Arborescence###

1) Pour aller le répertoire /var/log on utilise la commande "cd /var/log".
2) Pour remonter d'un étage dans l'arborescence et accéder à /var on utilise la commande "cd ..".
3) Pour retourner à son dossier personnel, on utilise la commande "cd ~" (ou "cd  ").
4) Pour revenir au dernier répertoire utiliser (ici var) on utilise la command "cd -".
5) La commande "cd /root" est refusée au motif de ne pas avoir la permission.
6) La commande "sudo cd /root" n'est pas reconnue, il faut d'abord rentrer "sudo -s", puis son mot de passe, et on peut ensuite accéder au root par "cd ~".
7) On utilise les commandes mkdir et touch pour créer respectivement les répertoires et fichiers: D'abord "mkdir Dossier1"
puis "touch Dossier1/Fichier1",
"mkdir -p Dossier2/{Dossier2.1,Dossier2.2}"
finalement "touch Dossier2/Dossier2.2/{Fichier2,Fichier3}".
8) On a pu supprimer le fichier avec "rm Dossier1/Fichier1", mais "rm Dossier1" ne fonctionne pas, refusant au motif que c'est un répertoire.
9) Il faut utiliser la commande "rmdir Dossier" pour supprimer un répertoire.
10) La commande "rmdir Dossier2" refuse de s'éxécuter sur le motif que le répertoire n'est pas vide.
11) Il faut utiliser la commande "rm -r Dossier2" pour supprimer le Dossier2 et tout son contenu.

###Commandes Importantes###

1) La commande "date" permet d'afficher l'heure, la commande "time _command_" permet de mesurer le temps de réalisation de la commande.
2) Le fichier commançant par . sont cachés des recherches normales. (ls)
3) /usr/bin/ls
4) Affiche les dossiers et leus informations (droits, dernière modif). Pas d'entrée manuel, ll alias de "ls -alF".
5) "ls bin"
6) Affiche le contenu du repertoire parent
7) pwd
8) elle écrit 'yo' dans le fichier plop (qui peut être créer). les données de plop sont écrasées
9) n'écrase pas, ajoute à la fin
10) Donne la nature de l'élément
11) "echo 'Hello Toto' > toto" . Ce qui est écrit sur tot passe sur titi. Effacer toto ne change pas titi.
12) Les deux on même contenu, supprimer titi vide tutu.
13) "cat var/log/syslog" ctrl+s, ctrl+q
14) "head -n 5 var/log/syslog"
"tail -n 15 var/log/syslog"
"head -n 20 var/lo/syslog | tail -n 10"
15) affiche la mémoire tempon page par page
16) contient les mots de passe, "man ect/passwd"
17) "cut -c1 /ect/passwd" | sort -r"
18) "getent passwd | grep -c "bin/bash"
19) "cat usr/bin/man | grep "conversion | wc -l"
20) 
