<h1 align="center" style="box-shadow: 10px 5px 5px red">Premier TP d'Administration Système</h1>                                   
<p>RIOUAL Matthieu :computer:</p>
<p>MORNEAU Hugo :computer:</P>


## Exercice 2

### Manuel

1. La commande `which` renvoie le chemin d'un éxécutable mis en argument.

2. Lorsqu'on lit une page du manuel, on peut rechercher du texte en tapant `/textevoulu` en lingne de commande.

3. On sort du manuel en appuyant sur la touche `q`.

4. La page d'introduction de la section 6 nous inquide que celle-ci parle de jeux et programmes de divertissements présents sur le système.

### Arborescence

1. Pour aller le répertoire /var/log on utilise la commande `cd /var/log`.

2. Pour remonter d'un étage dans l'arborescence et accéder à /var on utilise la commande `cd ..`.

3. Pour retourner à son dossier personnel, on utilise la commande `cd ~` (ou `cd  `).

4. Pour revenir au dernier répertoire utiliser (ici var) on utilise la command `cd -`.

5. La commande `cd /root` est refusée au motif de ne pas avoir la permission.

6. La commande `sudo cd /root` n'est pas reconnue, il faut d'abord rentrer `sudo -s`, puis son mot de passe, et on peut ensuite accéder au root par `cd ~`.

7. On utilise les commandes mkdir et touch pour créer respectivement les répertoires et fichiers: D'abord `mkdir Dossier1`
puis `touch Dossier1/Fichier1`,
`mkdir -p Dossier2/{Dossier2.1,Dossier2.2}`
finalement `touch Dossier2/Dossier2.2/{Fichier2,Fichier3}`.

8. On a pu supprimer le fichier avec `rm Dossier1/Fichier1`, mais `rm Dossier1` ne fonctionne pas, refusant au motif que c'est un répertoire.

9. Il faut utiliser la commande `rmdir Dossier` pour supprimer un répertoire.

10. La commande `rmdir Dossier2` refuse de s'éxécuter au motif que le répertoire n'est pas vide.

11. Il faut utiliser la commande `rm -r Dossier2` pour supprimer le Dossier2 et tout son contenu.

### Commandes Importantes

1. La commande `date` permet d'afficher l'heure, la commande `time _command_` permet de mesurer le temps de réalisation de la commande.

2. Les fichiers commançant par . sont cachés des recherches normales. (par ls)

3. Le programme `ls` se situe en /usr/bin/ls

4. `ll` Affiche les répertoire, les fichiers et leurs informations (droits, dernière modif...). Elle n'a pas d'entrée manuel, ll est un alias (un raccourci) de `ls -alF`.

5. `ls bin` permet d'afficher le contenu du répertoire bin depuis le répertoire parent.

6. La commande `ls ..` affiche le contenu du répertoire parent.

7. La commande `pwd` affiche le path du répertoire courant.

8. La commande `echo yo > plop` écrit 'yo' dans le fichier 'plop' (le créant si il n'existe pas). les données de plop sont écrasées par la commande, après 2 éxécutions le fichier 'plop' contiendra 'yo'.

9. La commande `echo yo >> plop` ajoute 'yo' à la fin du fichier 'plop' (le créant si il n'existe pas). En partant sans fichier 'plop', après 2 éxécutions le fichier 'plop' contiendra 'yoyo'.

10. La commande `file nom` donne la nature de l'objet nom (répertoire, fichier...)

11. On créer le fichier toto avec la commande `echo 'Hello Toto' > toto`. On créé ensuite un lien titi vers ce fichier
avec la commande `ln toto titi`, ce qui a pour effet que ce qui est écrit sur toto est copié sur titi. Effacer toto ne change pas titi.

12. On utilise la commande `ln -s titi tutu` pour créer un lien symbolique entre titi et tutu. Les deux désignent le même fichier, supprimer titi rend tutu inutile car son contenu n'existe plus.

13. On affiche à l'écran var/log/syslog avec `cat var/log/syslog`. Les raccourcis `ctrl+s` et `ctrl+q` permettent d'arrêter le défilement de l'écran.

14. La commande `head -n 5 var/log/syslog` permet d'afficher les 5 premières lignes du fichier 'syslog'.
La commande `tail -n 15 var/log/syslog` permet d'afficher les 5 dernières lignes.
La commande `head -n 20 var/lo/syslog | tail -n 10` permet d'affiche de la ligne 10 à la ligne 20.

15. affiche la mémoire tempon page par page

16. contient les mots de passe, `man ect/passwd`

17. `cut -c1 /ect/passwd" | sort -r`

18. `getent passwd | grep -c bin/bash`

19. `cat usr/bin/man | grep conversion | wc -l`

20. 
