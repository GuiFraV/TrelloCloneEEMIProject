# EEMI KanBan Symfony 6

**Comment réaliser un kanban avec symfony 6 ?**

1er Etape : Initialisation du projet symfony avec la version 6.2 et PHP 8.

`symfony new nom_du_projet --version="6.2.*" --webapp`

_le flag --webapp permet d'installer l'application complète de symfony 6 !_

2eme Etape : Création et configuration une BDD dans phpmyadmin.

    - Création d'un fichier .env.dev.local
    - Ajout de la connexion string au fichier .env.dev.local
    - Ensuite créer la BDD `symfony console doctrine:database:create`


3eme Etape : Création d'un HomeController.

`symfony console make:controller`

4eme Etape : Création d'un entity User pour stocker les données des utilisateurs.

`symfony console make:user` -> pour créer l'entity User
`symfony console make:migration` -> pour créer un fichier de migration obligatoire 
`symfony console doctrine:make:migration` -> push les données vers la bdd

5eme Etape : Création d'un authentificateur (formulaire d'inscription et formulaire de connexion).

