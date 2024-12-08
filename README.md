# Decoupage-de-reseaux-IP
### Le découpage symétrique

|       | Adresse réseau|Adresse de broadcast|Adresse de début de plage|Adresse de fin de plage|
|---    |:-:            |:-:                 |:-:                      |:-:                    |
|informatique|172.16.1.0/26|172.16.1.63|172.16.1.1|172.16.1.62|
|développement|172.16.1.64/26|172.16.1.127|172.16.1.65|172.16.1.126|
|Administratif|172.16.1.128/26|172.16.1.191|172.16.1.129|172.16.1.190|
|Technicien |172.16.1.192/26|172.16.1.255|172.16.1.193|172.16.1.244|

### besoin/info de base :
Le réseau est en 172.16.1.0/24.
Le Pôle informatique (6 bureaux, environ 50 équipements au total)  
Le Pôle développement (6 bureaux, environ 12 équipements au total)  
Le Pôle Administratif (4 bureaux, environ 20 équipements au total)  
Le Pôle Technicien (4 bureaux, environ 15 équipements au total)  
### calcul :  
Selon le tableau donnée dans l'exo il faut bosser avec 2^6 pour que le pole informatique est de quoi avoir tout leurs equipements.le CIDR sera /26 car 32-6=26.  
Ici ont taf qu'avec 2^6 pour l'addressage ip je vous laisse donc regardée le tableau ci dessus c'est plus tot simple et linéaire.(62 plages ip dispo)

### Le découpage asymétrique
|       | Adresse réseau|Adresse de broadcast|Adresse de début de plage|Adresse de fin de plage|
|---    |:-:            |:-:                 |:-:                      |:-:                    |
|informatique|172.16.1.0/26|172.16.1.63|172.16.1.1|172.16.1.62|
|Administratif|172.16.1.64/27|172.16.1.95|172.16.1.65|172.16.1.94|
|Technicien|172.16.1.96/27|172.16.1.127|172.16.1.97|172.16.1.126|
|développement|172.16.1.128/28|172.16.1.143|172.16.1.129|172.16.1.142|

### besoin/info de base :
Le réseau est en 172.16.1.0/24.
Le Pôle informatique (6 bureaux, environ 50 équipements au total)  
Le Pôle développement (6 bureaux, environ 12 équipements au total)  
Le Pôle Administratif (4 bureaux, environ 20 équipements au total)  
Le Pôle Technicien (4 bureaux, environ 15 équipements au total)  

### calcul :
Selon le tableau donnée dans l'exo il faut bosser avec 2^6 pour que le pole informatique est de quoi avoir tout leurs equipements.  
le CIDR sera /26 car 32-6=26 uniquement pour le pole informatique cette fois.(62 plages ip dispo)  
celui du developement sera /28 car 32-4=28.(14 plages ip dispo)  
quand au deux dernier pole il aurons tout deux le meme CIDR /27 car 32-5=27.(30 plages ip dispo)  
Pour ce qui est du calcul des adresse ip résseau ont ce refere au CIDR et on continue les calcul dans cette directiuon je vous laisse donc vous référer au tableau ci dessus :D.  
