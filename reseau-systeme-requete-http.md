[retour à la liste des mémos](https://github.com/Sergio2008/memo/blob/master/README.md)
#Reseau systeme
***
##Requete http
***

f12 => reseau

requete sont composer :

***
### Méthode
***

```
* Requete GET       : recuperation d'information
* Requete HEAD    : recuperation d'information (moins utuliser recupere pas tout)
* Requete POST    : creer une information
* Requete PUT     : Sert a modifier une donnée (mais les donnée diovent etre complete)
* Requete PATCH   : Sert a modifier une donnée(peut ne pas etre)
* Requete OPTION  : 
* Requete TRACE   : Test 
* Requete CONNECT : Utuliser un proxy
* Requete DELETE  : Supprimer une info
```

***
### Code de retour / Code d'etat
***

```
* 200 : OK
* 301 et 302 : Redirection (301 sert à recuperer le referencement en cas de changement d'adresse d'une page)
* 304 : La page vient du cash
* 500 : Probleme tech 
* 404 : La pae n'existe pas
```
