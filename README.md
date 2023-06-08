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

### Lancer le serveur
```
symfony serve
```