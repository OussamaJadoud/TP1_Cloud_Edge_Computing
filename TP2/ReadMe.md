# Etape 1 : 
##Qst1 : 
Le réseau privé permet d'isoler les utilisateurs dans infrastructeur patagée tout en permettant en permettant la communication des machines internes.
Le routeur externe permet la connection de réseau privée avec le monde externe/internet.

##Qst2: 
Pour permettre au client d'utiliser les ressources dont il a besoin, et aussi pour payer juste les ressources utilisées.

##Qst3 : 
Depuis internet ou un autre reseau, la requette va passer par le routeur externe qui va l'adresser vers le reseau privée exactement à la machine virtuelle.



# Etape 2 : 
##Qst1 : 
- Créer et telecharger la clé SSH.
- Associer la VM à une IP flottante pour qu'elle soit accessible depuis l'exterieur ( la machine hôte ).
- Taper la commande suivante dans la machine hôte; ssh-i vm-discovery-key.pem ubuntu@<IP_FLOTTANTE> (-i pour confirmer la possession d'un clé privé).

##Qst2 :
- La IP privé sert juste pour la connection interne dans un réseau privé.

- IP flottante : pour connecter la machine au monde exterieur. 

- Groupes de Sécurité joue le rôle d'un Pare Feu. Il permet de specifier l'ensemble des regles de securité d'entrée et sortie de la VM.

##Qst3 :

Parce que les addresses IP coûtent chères et les addresses IP flotantes sont plus manipulables. 



#ETAPE 3 :
##QST 1 :
IP publique met la machine joignable depuis l'exterieur, mais le groupe de sécurité agit comme un pare feu bloquant tout port non autorisé pour securisé la machine des attaques. 

##QST 2 :
- Le pc envoie la requette vers  http://<IP_FLOTTANTE>:5000.

- La requette est captée par le routeur exterieur de Openstack et l'envoie au réseau privé.

- La requette est reorientée vers la machine virtuelle associé l'adresse flottante et puis dirigé vers le numero de port associé à l'application "Hello-api".



#ETAPE 4 :
##QST1 : 
L'image officielle est vierge, tandis que snapshot contient toutes les modifications qu'on a apporté sur l'image officielle.
Par exemple Snapshot contient 2 core, contient l'application "Hello-api"...

##QST2 : 
Le redimensionnement permet la flexibilité, si nous sommes besoin d'espace oubien les applications commencent à bugger on peut ajouter plus de RAM...

##QST3 :
Un administrateur système prefere de faire une snapshot pour conserver toutes ses modifications apportées sur l'image viergs donc il n'aura pas besoin de
repartir à zero pour duppliquer son environnement.





 




