# Glossaire 

ORM transforme en Objet les tables dans la base de donnée
dans laravel les objet sont des modele

la Class est la definition (general/generique) d'un objet la liste de ces caracteristique
et de ces methode(fonction)

Objet quand  à lui est une instance (un arret sur image d'une classe a un moment donné avec des valeur a la place des caracteristique) d' une class  donc c'est à dire un exemple particulier 

### instance = un objet en paticulier
### instancier = créer une instance

```
GET pas encrypter taille max 200 char
POST encrypter 
```

### attributs 

les attibut sont le noms se referant aux caracteristique d'une class

### héritage (innheritance)

c'est le fait de pouvoir créer une class qui engloberais par definition/principe une autre plus petite et qui permettrais de beneficier des meme attribut des meme methode

### surcharger (overriding)

c'est créer une methode dans une classe enfant qui existe deja dans la classe parente 


### setter

Permet de fixer des valeu
```
<?php
 
class MyObject 
{
  /**
   * Methode magique __set()
   *
   * @param string $property Nom de la propriété
   * @param mixed $value Valeur à affecter à la propriété
   * @return void
   */
  public function __set($property, $value)
  {
    // Code personnalisé à exécuter
  }
}
 
?>
```

### getter
permet de lire une propriete existante de la class
```
<?php
 
class MyObject 
{
  /**
   * Methode magique __get()
   *
   * @param string $property Nom de la propriété à atteindre
   * @return mixed|null
   */
  public function __get($property)
  {
    // Code personnalisé à exécuter
  }
}
 
?>
```






