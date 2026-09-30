ReadMe TP1 ;

# Etape 1 : 
## Qst1 :
La machine virtuelle est un environnement qui reproduit une machine en utilisant une image, en lui allouant des propres ressources virtuelles ( processeur, memoire, stockage , reseau). 

## Qst 2 :
Parmi les avantages on a :
- Mutualisation des ressources (pas de gaspillage).
- Sécurisation des données. 

## Qst 3 :
Travailler sur une machine virtuelle autre que notre ordinateur nous donne la flexibilité de travailler avec d'autres OS et c'est exportable, on peut faire des snapshots et utiliser la VM dans une autre machine physique. 


# Etape 2 : 
## QST1 :
Un conteneur permet d'isoler juste une application, sans virtualiser une machine complète. 

## QST 2 :
La machine virtuelle est au niveau machine c'est une forme virtuelle d'une machine entière avec des ressources virtuelles, par contre conteneur est au niveau application. Le conteneur est moins isolé que la machine virtuelle parceque il partage l'OS hôte.

## QST 3:
Le Cloud met à disposition un grand nombre de ressources, il est utile d'utiliser des conteneurs pour heberger des applications, car cela permet de separer la ressource necessaire pour chaque applications surtout si le cloud est réparti sur plusieurs serveurs.



# ETAPE 3 : 
## QST 1 :
Dockerfile c'est la description d'environement avec les dépendences et la commande de démarrage, c'est plus simple que d'écrire manuellement le conteneu, et il assure que l'image construite donne un modèle reproductible.
'

## QST 2 :

L'image Docker c'est le modèle reproductible qu'on le réutiliser plusieurs fois tandis que le conteneur Docker c'est une instance en execution créée d'aprés l'image.


# ETAPE 4:
## QST1 : 
Docker Compose c'est un orchestrateur il permet de gérer plusieurs conteneur au meme temps facilement au lieu de les gérer à la main.


## QST 2 :
Le fichier YAML est un fichier de configuration sert à definir les services de l'application.


## QST 3 :
Docker compose est trés bien pour gérer plusieurs Conteneur sur la même machine , on va rencontrer des problèmes si l'application devient trés grande ou répartie sur plusieurs machines.