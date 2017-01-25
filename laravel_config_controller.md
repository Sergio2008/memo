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

2. Configurer la route en y ajoutant l'accès à un controller et à une de ces methode

```
Route::get('messages', 'MailController@allreturn');

```

>``Route::get` (sytaxe basique laravel)
>>`'message'` nom de domaine / message
>>>>`MailController@allreturn` MailController (nom du controller)@allreturn(nom de la methode)


