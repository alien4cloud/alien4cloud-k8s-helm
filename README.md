# alien4cloud-k8s-helm
Helm chart TOSCA integration

Si chaque start commence par aller résoudre ses dépendances en 
faisant des lookups dont la liste lui est fournie par avance ::

Map
Nom de la variable -> Expression lookup

Il y a des choses qu'on ne sait pas à l'avance, ok
Mais on doit pouvoir savoir à l'avance comment récupérer cette information
Si obtenir la valeur d'une capability, c'est juste executer un script, faire un lookup, on doit pouvoir le définir

C 'est porté par la capability d'un noeud
Une property de capability porte le comment on la récupère (loopup k8s)


Comment je stocke dans mon values ?

get_property SELF, toto
get_property TARGET requirement capa propertyName
