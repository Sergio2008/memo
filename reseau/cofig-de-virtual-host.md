[retour à la liste des mémos](https://github.com/Sergio2008/memo/blob/master/README.md)

# Configuration du virtual Host

## Prerequis

* Avoir apache installer `apt-get install apache2`

* Verifier les mise à jour ` apt-get update `

* Faire les mise à jour `apt get upgrade`

## Créer un fichier `.conf` dans `/etc/apache2/sites-available/`

### Et le completer

```
<VirtualHost *:80>
    ServerAdmin admin@example.com
    ServerName example.com
    ServerAlias www.example.com
    DocumentRoot /var/www/example.com/public_html
    ErrorLog ${APACHE_LOG_DIR}/error.log
    CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>
```

### Activer la configuration

`a2ensite example.com.conf`

### Redemarrer le serveur

>`systemctl restart apache2`
>>ou `systemctl reload apache2`

### Attention au droit d'écriture des fichier
