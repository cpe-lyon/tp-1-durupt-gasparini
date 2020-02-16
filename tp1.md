<h1>TP 1 - Installation d’Ubuntu Server et prise en main du shell
<h2>Exexcice 1
<h2>Exexcice 2 </h2>
<h4>Manuel </h4>

1. **which**
2. Afin de rechercher un élèment, on met un slash suivi du texte rechercher. Ex: **man which /option**
3. on quitte le manuel en appuyant sur **q**
4. Section 6 of the manual describes the games and funny little programs available on the system

<h4>Navigation dans l’arborescence des fichiers</h4>

1. On se rend dans le dossier **/var/log** avec la commande **cd /var/log**
2. remontez dans le dossier parent (/var) en utilisant un chemin relatif avec la commande **cd ..**
3. retournez dans le dossier personnel avec la commande **cd ./log**
4. revenez au dossier précédent (/var) sans utiliser de chemin avec la commande **cd -**
5. l'accès au dossier **/root** est refusé (**permission denied**)
6. La commande **sudo** permet d'avoir temporairement des droit d'admin
7. **mkdir** chemin du dossier : pour créer un dossier**
	**touch** chemin du fichier : 		pour créer un fichier
	
8. La commande **rm** permet de supprimer un fichier
	**rmdir** pour les dossiers
9. Il est impossible de supprimer un dossier non vide 
10.**rm -r** permet de supprimer en une seule commande Dossier2 et son contenu 

<h4>Navigation dans l’arborescence des fichiers</h4>


1. **time** est utilisé pour determiner combien dure une tâche (test de performance pour des scripts ou des commandes, **date** donne la date et l'heure.

2. **ls** : liste les fichier du dossier courant, **la** : liste les alias  (les fichiers avec un . sont des alias)

3. le programme **ls** se situe dans le dossier **/bin**

4.  donne les alias
il n'existe pas d’entrée dans le manuel pour **ll**
**ll** est un alias de **ls -alF**

5. afficher les fichiers contenus dans le dossier **/bin** : **ls /bin**

6. **ls** liste les fichiers du dossier courant

7. **pwd** donne le chemin complet du dossier courant

8. Que fait la commande **echo 'yo' > plop** exécutée 2 fois ? écrit un fichier **plop** et écrit **yo** à l’intérieur du fichier en écrasant le contenu

9. Que fait la commande **echo 'yo' >> plop** exécutée 2 fois ? écrit à la ligne un deuxième **yo**

10. la commande **file** détermine le type de fichier

11. **titi** prend les modifications / à la suppression de **toto**, **titi** existe encore

12. **tutu** est aussi modifié / **titi** est modifié / **titi** est supprimé mais pas **tutu**

13. **cat /var/log/syslog** --> **cat** permet d'afficher le contenu d'un fichier à l'écran / **CTRL + z** stoppe / **CTRL + c** arrête / CTRL+s met en pause /  **CTRL+q** reprise

14. **head -5 /var/log/syslog**--> Affiche les 5 premières lignes du fichier
	**tail -15 /var/log/syslog** --> Affichez les 15 dernières lignes du fichier
	**head -20 /var/log/syslog | tail -10** --> affiche les lignes 10 à 20

15. **dmesg | less** : Afficher et contrôler le tampon des messages du noyau page par page

16. le fichier **/etc/passwd ** contient le fichier des utilisateurs du système
**sudo man /etc/passwd** --> commande pour afficher le manuel

17. Affichez seulement la première colonne triée par ordre alphabétique inverse : **sudo cut -c1 /etc/passwd | sort -r**
18. **sudo cat /etcpasswd | awk ‘ED {print NR}’** --> donne le nombre d’utilisateurs ayant un compte sur cette machine

19. **find**

20. **find / -name “passwd” -print**

21. **find / -name “passwd” -print | >> ~/list_passwd_files.txt**

22. Dans votre dossier personnel, utilisez la commande **grep** pour chercher où est défini l’alias ll vu précédemment : **grep ~ ^ll**

23. **ocate history.log**

24. le fichier n’apparait pas











