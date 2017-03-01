# MCD modèle conceptuel des données (aussi appelé schéma Entité/Association)


c'est une representation graphique des info memoriser par un si (Systeme d'information)

Il le fait grace a deux notion principale les entite et les association

![Zozor](http://merise.developpez.com/faq/images/MCD_UML_1.gif)

L'élaboration du MCD passe par les étapes suivantes :
. La mise en place de règles de gestion (si celles-ci ne vous sont pas données),
. L'élaboration du dictionnaire des données,
. La recherche des dépendances fonctionnelles entre ces données,
. L'élaboration du MCD (création des entités puis des associations puis ajout des cardinalités).

1. 
il vous faut recueillir les besoins des futurs utilisateurs
vous devez être en mesure d'établir les règles de gestion des données à conserver.

2.
Le dictionnaire des données est un document qui regroupe toutes les données que vous aurez à conserver dans votre base (et qui figureront donc dans le MCD). Pour chaque donnée, il indique :

    Le code mnémonique : il s'agit d'un libellé désignant une donnée (par exemple «titre_l» pour le titre d'un livre)
    La désignation : il s'agit d'une mention décrivant ce à quoi la donnée correspond (par exemple «titre du livre»)
    Le type de donnée :
        A ou Alphabétique : lorsque la donnée est uniquement composée de caractères alphabétiques (de 'A' à 'Z' et de 'a' à 'z')
        N ou Numérique : lorsque la donnée est composée uniquement de nombres (entiers ou réels)
        AN ou Alphanumérique : lorsque la donnée peut être composée à la fois de caractères alphabétiques et numériques
        Date : lorsque la donnée est une date (au format AAAA-MM-JJ)
        Booléen : Vrai ou Faux
    La taille : elle s'exprime en nombre de caractères ou de chiffres. Dans le cas d'une date au format AAAA-JJ-MM, on compte également le nombre de caractères, soit 10 caractères. Pour ce qui est du type booléen, nul besoin de préciser la taille (ceci dépend de l'implémentation du SGBDR).
    Et parfois des remarques ou observations complémentaires (par exemple si une donnée est strictement supérieure à 0, etc).

3.
Les dépendances fonctionnelles
▲

Soit deux propriétés (ou données) P1 et P2. On dit que P1 et P2 sont reliées par une dépendance fonctionnelle (DF) si et seulement si une occurrence (ou valeur) de P1 permet de connaître une et une seule occurrence de P2.

Cette dépendance est représentée comme ceci :

P1 → P2

On dit que P1 est la source de la DF et que P2 en est le but.

Par ailleurs, plusieurs données peuvent être source comme plusieurs données peuvent être but d'une DF. Exemples :

P1,P2 → P3
P1 → P2,P3
P1, P2 → P3,P4,P5

