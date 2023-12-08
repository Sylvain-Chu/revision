
# Administration Système Linux

## Questions de cours

### À quoi sert la variable d'environnement `PS1` ?
- **Réponse**: À configurer l'apparence de l'invite de commande ("prompt").

### Commande pour obtenir les 5 premiers mots de `listeMots`
- **Réponse**: `sort listeMots | head -n 5`

### Commande pour afficher le code de sortie de la dernière commande exécutée
- **Réponse**: `echo $?`

### Que fait la commande `!!` ?
- **Réponse**: Elle rappelle la commande précédente.

### Par quelle ligne commence généralement un script Bash ?
- **Réponse**: `#!/bin/bash`

### Que signifie le caractère "." en début de nom de fichier ?
- **Réponse**: Il indique qu'il s'agit d'un fichier caché.

### Commande(s) pour aller dans son répertoire personnel sans taper son chemin
- **Réponse**: `cd ~` ou simplement `cd`

### Que fait la commande `cd -` ?
- **Réponse**: Elle nous ramène au dernier répertoire dans lequel on se trouvait.

### Commande pour afficher le contenu d'un fichier page par page
- **Réponse**: `less fichier` ou `more fichier`

### Commande pour remonter dans le répertoire parent
- **Réponse**: `cd ..`

### Recherche d'un mot dans une page de manuel
- **Réponse**: On utilise `/mot` après avoir ouvert la page man.

### Que contient la variable d'environnement `PATH` ?
- **Réponse**: C'est l'emplacement des binaires des commandes

### Comment sortir du manuel ?
- **Réponse**: En appuyant sur la touche `q`.

### Qu'est-ce que GNU/Linux ?
- **Réponse**: Le noyau Linux augmenté d'utilitaires issus du projet GNU.

### Commande pour s'assurer que le fichier `monFichier` existe avant de poursuivre un traitement
- **Réponse**: `touch monFichier`

### Destination du résultat de la commande `commande > /dev/null`
- **Réponse**: Dans le néant absolu, rien n'est conservé.

### Commande pour afficher le nombre de lignes d'un fichier
- **Réponse**: `wc -l fichier`

### Ce que la commande `wc` ne permet pas de faire
- **Réponse**: Trier un fichier.

### Que représente en général le caractère "$" en début de ligne de commandes ?
- **Réponse**: L'invite shell (ou prompt) d'un utilisateur ordinaire.

### Deux éditeurs de texte accessibles dans un environnement serveur
- **Réponse**: `vim` et `nano`

### 3 fonctionnalités principales du noyau Linux
- **Réponse**: Interface entre matériel et programmes, exécution de plusieurs programmes simultanément, support pour différents types de processeur, gestion de fichiers, et catalogue de fonctions réseau.

### Commande pour effacer l'écran
- **Réponse**: `clear` ou `CTRL + L`

### Commande pour envoyer un processus en arrière-plan
- **Réponse**: `bg`

### Rôle d'un serveur DNS
- **Réponse**: Traduire un nom de domaine en une adresse IP.

### Un gestionnaire de paquet permet de
- **Réponse**: Télécharger depuis internet.

### Valeur octale des droits `rw-rw-r-x`
- **Réponse**: 665

### Commande pour afficher le nombre de lignes d'un fichier
- **Réponse**: `wc -l`

### Contenu de la variable d'environnement `PATH`
- **Réponse**: Liste de répertoires dans lesquels le shell recherche les commandes exécutées.

### Commande qui a remplacé `ifconfig` dans les versions récentes de Debian et Ubuntu
- **Réponse**: `ip`

### Un fichier et un lien symbolique sur ce fichier ont le même inode
- **Réponse**: Faux

### Utilité de la commande `pwd`
- **Réponse**: Affiche le dossier courant.

### Contenu du fichier `/etc/motd`
- **Réponse**: Un message qui s’affiche lorsqu’un utilisateur ouvre une session.

### Signification du caractère "." en début de nom de fichier
- **Réponse**: Indique un fichier caché.

### Utilité du swap
- **Réponse**: Décharge la mémoire RAM sur le disque dur en cas de saturation.

### Référence de l’adressage CHS
- **Réponse**: Adressage des données d'un disque dur.

### Commande pour lancer le processus `toto` en arrière-plan
- **Réponse**: Symbole `&` ou `bg toto`

### Outil pour manipuler la table des partitions
- **Réponse**: `fdisk`

### Syntaxe pour spécifier à `grep` de rechercher des lignes commençant par le mot "système"
- **Réponse**: `^[système]`

### Le point-virgule (;) sépare plusieurs commandes exécutées dans l'ordre
- **Réponse**: Faux

### Fichier spécifiant les partitions à monter au démarrage
- **Réponse**: `/etc/fstab`

### Un volume logique LVM peut être à cheval sur deux disques physiques
- **Réponse**: Vrai

### Deux types de partitionnement d’un disque dur
- **Réponse**: MBR (Master Boot Record) et GPT (GUID Partition Table)

### Commande pour lister les modules chargés dans le noyau
- **Réponse**: `lsmod`

### Valeur littérale des droits `643`
- **Réponse**: `rw-r--wx`

### Que désigne `tty3`?
- **Réponse**: La 3ème console virtuelle

### Résultat de `wc unFichier` (11176 61033 670293 unFichier)
- **Réponse**: Nombre de lignes, de mots et de caractères dans `unFichier`

### Commande pour mettre en pause un processus
- **Réponse**: CTRL+Z

### Un pipe permet de
- **Réponse**: Envoyer la sortie d’une commande à une autre commande.

### Commande pour changer de répertoire courant
- **Réponse**: `cd`

### Effet de la séquence de touches Echap+. (point)
- **Réponse**: Affiche le dernier argument de la commande précédente.

### Utilisation de guillemets avec `grep`
- **Réponse**: Nécessaire lorsque l'élément recherché est une expression régulière.

### Commande pour monter une partition
- **Réponse**: `mount`

### Commande pour renommer un fichier
- **Réponse**: `mv`

### Tâches dévolues à un administrateur système
- **Réponse**: Configuration du matériel, installation du système d'exploitation, gestion des applications, création d'utilisateurs et de groupes, administration du réseau, sécurité du système, configuration du noyau, planification de la continuité, planification des capacités.

### Référence du fichier `/dev/sdb1`
- **Réponse**: Première partition du premier disque.

### Ensemble formé par un noyau Linux et des outils de gestion
- **Réponse**: Distribution Linux.

### Commande permet de modifier le mot de passe d’un utilisateur
- **Réponse**: `passwd`

### Après avoir tapé la commande ln -s fichier lien, on supprime fichier. Qu’affiche la commande cat lien? 
- **Réponse**: Le même contenu que celui de fichier avant suppresion

### Quelle commande permet d'envoyer un signal à un processus ?
- **Réponse**: `kill`

###   Pourquoi les serveurs n’ont pas d’interface graphique?
  
• Les serveurs ne sont pas équipés d’écrans, de claviers ou de souris. Au maximum, ils se connectent à  un terminal partagé mais presque tous accessibles à distance via la console texte ou la console virtuelle.  
•  Le bureau graphique représente un énorme risque pour la sécurité sans aucun avantage. Il ne fait que  gaspiller de l'espace disque, des cycles CPU et de la RAM. Il comprend également un grand nombre de  packages, qui ajoutent de la complexité aux mises à niveau et aux correctifs -  certains fournisseurs  commerciaux ne prennent même pas en charge les mises à niveau entre les versions de Linux si le  bureau est installé.

### Je tape la commande ls dans mon terminal. Expliquer comment Bash procède pour localiser la  commande ?
- **Réponse**: La variable d’environnement PATH stock les chemins d’accès à toutes les commandes. Il va donc parcourir tous  les chemins possible jusqu’à trouer la commande correspondante.

### D’après les informations suivantes, l’utilisateur bob peut-il exécuter la commande more /data/abc.txt?  
drwxr-xr-x. 17 root root  4096 23:38 /  
dr-xr-x---. 10 eve compta 128  03:38 /data  
-rwxr-xr--. 1 bob  bob 100  21:08 /data/abc.txt  
  
- **Réponse**: La commande `more`permet de lire le contenu d’un fichier texte page par page. Pour pouvoir exécuter cette  commande, il faut avoir les droit de lecture sur le fichier. On peut voir les permissions sur ce fichier (-rwxr-xr--).  Cela nous indique que tout le monde a les droits de lecture sur ce fichier, bob peut donc exécuter la commande  `more`.

### Différences entre UNIX et Linux :

- **Réponse**: Linux peut être installer sur différents types d'appareils (ordi, portables etc.) alors que UNIX est utilisé pour les serveurs internet, les postes de travail et et les PC.
    
### Qu’est-ce qu’une table de partitions (à quoi sert-elle, que contient-elle...)? Comment afficher son contenu ?     
- **Réponse**: Une table de partitions est une table maintenue sur les disques durs et d'autres supports de stockage qui enregistre les partitions du disque. 
Elle contient des informations telles que la taille de chaque partition, son emplacement, le type de système de fichiers, et d'autres métadonnées nécessaires pour la gestion du stockage.
Commandes : `fdisk -l`, `parted -l`, ou `lsblk` pour afficher la table de partitions.

### Sous Linux, on peut copier, déplacer ou supprimer des fichiers. Expliquez (précisément) pourquoi le fait de déplacer un fichier sur la même partition peut être beaucoup plus rapide que copier ce fichier puis supprimer l’original (notamment pour les fichiers volumineux) ?
Lorsque vous déplacez un fichier sur la même partition, le système ne déplace réellement que la référence au fichier dans le système de fichiers. Aucun changement n'est apporté aux données réelles du fichier, ce qui est très rapide.
En revanche, copier puis supprimer l'original implique deux opérations majeures : copier l'ensemble des données du fichier vers un nouvel emplacement (ce qui peut prendre beaucoup de temps pour les fichiers volumineux), puis supprimer l'original. Ces étapes rendent le processus considérablement plus lent, surtout avec des fichiers volumineux.

### Utilité du Caractère x dans l'Instruction `if [ x$saisie == x$password ]` :

Le caractère `x` est utilisé ici pour éviter des erreurs dans le script lorsque l'une des variables (`$saisie` ou `$password`) est vide. Sans le `x`, si l'une des variables est vide, le shell pourrait interpréter la commande d'une manière inattendue, pouvant mener à une erreur de syntaxe. En ajoutant `x`, vous vous assurez que chaque côté de l'opérateur `==` est non vide, permettant une comparaison sûre.

### Différence Entre Les Commandes :
`commande1 ; commande2` : Exécute `commande1` puis `commande2` indépendamment du succès ou de l'échec de `commande1`.
`commande1 && commande2` : Exécute `commande2` seulement si `commande1` réussit (c'est-à-dire, se termine avec un code de sortie 0).
`commande1 || commande2` : Exécute `commande2` seulement si `commande1` échoue (c'est-à-dire, se termine avec un code de sortie non nul).

### Explication de la Commande `cut -d ',' -f 6 people.csv | tr a-z A-Z | tac -r -s 'x\|[^x]' | sort` :
```
id,firstname,lastname,email,age,profession
100,Tabbatha,Velick,Tabbatha.Velick@yahoo.com,52,developer 
102,Arlina,Wu,Arlina.Wu@yahoo.com,52,developer 
103,Maye,Flita,Maye.Flita@yahoo.com,46,police officer 
104,Max,Juan,Max.Juan@yahoo.com,31,developer 
106,Netty,Pauly,Netty.Pauly@yahoo.com,58,doctor 
109,Gui,Cohdwell,Gui.Cohdwell@yahoo.com,32,firefighter
```
`cut -d ',' -f 6 people.csv` : Sélectionne le 6ème champ (profession) de chaque ligne du fichier `people.csv`, en utilisant la virgule comme délimiteur.
`tr a-z A-Z` : Convertit toutes les lettres minuscules en majuscules dans la sortie de `cut`.
`tac -r -s 'x\|[^x]'` : Cette partie de la commande est un peu inhabituelle. Normalement, `tac` renverse l'ordre des lignes (le contraire de `cat`). Cependant, l'option `-r` active l'expression régulière et `-s 'x\|[^x]'` définit le séparateur de ligne. Si l'intention était de simplement inverser l'ordre des lignes, `tac` seul suffirait. Ici, l'utilisation de `-r -s 'x\|[^x]'` semble être une erreur ou une confusion, car elle cherche à utiliser 'x' ou tout caractère non 'x' comme séparateur, ce qui n'a pas de sens dans ce contexte.
`sort` : Trie les lignes de la sortie dans l'ordre alphabétique.

## Exercices
### Exercices 1 : Bash
On vous demande d’écrire un script Bash nommé `size` qui affiche la taille (en octets) d’un fichier passé en paramètre sur la ligne de commandes. Par exemple : 
La taille du fichier `mon_fichier` est : 12345 octets. La commande permettant de récupérer la taille d’un fichier est `stat -c %s fichier`.

Quelques consignes doivent être respectées :
- Si l’utilisateur ne passe aucun fichier, ou passe plus d’un fichier en paramètre, le script doit afficher un message rappelant comment l’utiliser.
- Le script doit être situé dans votre dossier personnel (`/home/VOTRE_NOM`).

1. **Quelle commande permet de se repositionner dans son dossier personnel (quel que soit le dossier où l’on se trouve)?**
Utilisez la commande `cd ~` ou simplement `cd` pour revenir à votre dossier personnel, peu importe où vous êtes dans le système de fichiers.
2. **A quoi sert la ligne #!/bin/bash située au début de chaque script Bash?**
Cette ligne est appelée "shebang". Elle indique au système d'exploitation que le script doit être exécuté avec l'interpréteur spécifié, ici `/bin/bash`. Elle doit être la première ligne du script.
3. **Ecrire le script demandé.**
```bash
#!/bin/bash

if [ "$#" -ne 1 ]; then
    echo "Usage: $0 filename"
    exit 1
fi

FILE=$1
if [ -f "$FILE" ]; then
    SIZE=$(stat -c %s "$FILE")
    echo "La taille du fichier $FILE est : $SIZE octets"
else
    echo "Fichier non trouvé."
fi

```

4. **Quelle commande permet de rendre ce script exécutable ?**
Utilisez `chmod +x size` pour rendre le script exécutable.
5. **Comment exécuter, depuis votre dossier personnel, ce script sur un fichier toto situé dans le sous-dossier dossier ?**
Depuis votre dossier personnel, utilisez `./size dossier/toto` pour exécuter le script sur le fichier `toto` situé dans le sous-dossier `dossier`.
6. **Vous est-il possible d’appeler ce script depuis le dossier /tmp ? (Si oui, expliquez comment, sinon expliquez pourquoi).**
Oui, c'est possible si le chemin vers le script est spécifié. Exemple : `/home/VOTRE_NOM/size fichier` depuis `/tmp`. Sans un chemin absolu ou relatif, le script ne sera pas trouvé.
7. **Rappeler le rôle de la variable d’environnement PATH. Comment afficher son contenu?**
`PATH` est une variable d'environnement qui spécifie les répertoires où le shell recherche les commandes exécutables. Utilisez `echo $PATH` pour afficher son contenu.
8. **Sur votre machine, le contenu de PATH est le suivant. De quoi s’agit-il ?**
   `/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
   Il s'agit d'une liste de répertoires où le système recherche les programmes exécutables. L'ordre indique la priorité de recherche.
9. **Pourquoi est-il fortement déconseillé d’ajouter le dossier ”.” à la liste de la question précédente?**
Ajouter "." (répertoire courant) à `PATH` est déconseillé pour des raisons de sécurité. Cela pourrait permettre l'exécution accidentelle de scripts ou de programmes malveillants présents dans le répertoire courant. 
10. **Afin de partager votre script avec tous les utilisateurs de la machine, vous souhaitez le déplacer dans le dossier /usr/local/bin. Quelle commande permet de réaliser ceci ?**
Utilisez `sudo mv /home/VOTRE_NOM/size /usr/local/bin/` pour déplacer le script. Vous aurez besoin des droits administrateurs pour cela.
11. **Il se trouve que les systèmes Linux disposent déjà d’un programme nommé size, situé dans le dossier /usr/bin. Si un utilisateur tape la commande size unfichier, quel programme size est appelé, celui installé de base ou celui que vous avez créé ? Expliquez.**
Le programme `size` dans `/usr/bin` sera appelé en premier car `/usr/bin` apparaît avant `/usr/local/bin` dans `PATH`. Le shell utilise le premier `size` qu'il trouve dans l'ordre de `PATH`.


