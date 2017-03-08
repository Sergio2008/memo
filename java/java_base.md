****
Print java
System.out.println();
****
int ecris simplement

``` 
7 
```

bolean ecris simplement

``` 
true 
```

char  entre simple quote

``` 
'true '
```
text  entre double quote

``` 
"true "
```
****
creer une variable

```
int myNumber = 42;
		boolean isFun =true; 
		char movieRating = 'A'; 
```
****
creer une class et son contructeur 
```
class Car {

    //The class constructor for the Car class
    public Car() {

    }
}
```
* Plus en detail
```
class Dog {
```

/*declare une variable*/

```
  int age;
``` 

/* declare un constructeur */

```
 
  public Dog(int dogsAge) {
```

   /* affecte un param ^ a cette variable */
   
 ```
    age = dogsAge;
      
    }

```

/* fonction lancer par default */
	
```
	public static void main(String[] args) {
```

/* instantie un chien avec le param */

```
    Dog spike = new Dog(7);

	}
}
```
#### HashMap
```

public static void main(String[] args) {

```
/* Crée une liste HashMap avec une clée string et une valeur en integer*/ 
```
		HashMap<String, Integer> restaurantMenu = new HashMap<String, Integer>();
```
/* Ajoute des elements à la liste */ 
```

		restaurantMenu.put("Turkey Burger", 13);
		restaurantMenu.put("Naan Pizza", 11);
		restaurantMenu.put("Cranberry Kale Salad", 10);
		
```
/* sort la taille de la liste */
```

		System.out.println(restaurantMenu.size());
		
```
/*  for each sur le HashMapp */
```

		for (String item : restaurantMenu.keySet()) {
		


			System.out.println("A " + item + " costs " + restaurantMenu.get(item) + " dollars.");

		}

	}
```
*** lol ***
****************

creer une liste (d'entier dans l'exemple)

```
ArrayList<Integer> weeklyTemperatures = new ArrayList<Integer>();
```

ajouter des valeur à une liste
```
weeklyTemperatures.add(89);
weeklyTemperatures.add(94);
```
ajouter à un endroit précis(à l'index 2)
```
weeklyTemperatures.add(2,89);

```

afficher une variable de la liste

```
System.out.println( weeklyTemperatures.get(1) );
```
taille de la liste
```
weeklyTemperatures.size()
```
****
raccourci (for each)
```
for (Integer temperature : weeklyTemperatures) {
	System.out.println(temperature);
}
```

