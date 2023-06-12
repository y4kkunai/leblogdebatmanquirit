# Projet Le Blog de Batman qui rit

### Cloner le projet

```
git clone https://github.com/Axelyakk/leblocdebatmanquirit.git
```

### Déplacer le terminal dans le dossier cloné
```
cd leblogdebatmanquirit
```

### Installer les vendors (pour recréer le dossier vendor)
```
composer install
```

## Création d'une base de données
Configurer la connexion à la base de données dans le fichier .env (voir cours), puis taper les commandes suivantes :
```
symfony console doctrine:database:create
symfony console doctrine:migrations:migrate

```
### Création des fixtures

```
symfony cosole doctrine:fixtures:load

```
Cette commande créera : 
* un compte admin (email: a@a.a , password: 'aaaaaaaA7/')
* 10 comptes utilisateurs (email aléatoire , password : 'aaaaaaaA7/')
* 50 articles


### Lancer le serveur
```
symfony serve
```