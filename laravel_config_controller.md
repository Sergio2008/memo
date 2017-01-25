* LARAVEL configuration de controller

** Model view controller

| Model         | View          | Controller |
| ------------- |:-------------:| ----------:|
| 		        | 			    |  			 |
|		        |       		|    		 |
| 			    |       		|     		 |

*** View et controller

1. Configurer le .env pour cibler la  base de donnée

>Nom de la base
>>Nom d'utulisateur
>>>Mots de passe

2. Configurer la route en y ajoutant l'accès à un controller et à une de ces methodes(fonction)

```
Route::get('messages', 'MailController@allreturn');

```

>`Route::get` (sytaxe basique laravel)
>>`'message'` nom de domaine / message
>>>>`MailController@allreturn` `MailController` (nom du controller)`@allreturn`(nom de la methode)

3. Configurer le controlleur

Créer le controlleur 

`php artisan make:controller OrderController -- ressource`

OrderController est le nom donné au Controller

ou copier un existant et le modifier

Créer une fonction

```
public function indexspe($id)
    {
        $message = DB::select('select content , object , id , sender from message  where id = :id', ['id' => $id]);
        

    return view('pages.message1', ['message' => $message[1]]);
    }
```
>$message = affecter
