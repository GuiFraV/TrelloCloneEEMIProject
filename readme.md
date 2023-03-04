# EEMI KanBan Symfony 6

**Comment réaliser un kanban avec symfony 6 ?**

1er Etape : Initialisation du projet symfony avec la version 6.2 et PHP 8.

`symfony new nom_du_projet --version="6.2.*" --webapp`

_le flag --webapp permet d'installer l'application complète de symfony 6 !_

2eme Etape : Créer une entité User qui contient les informations de l’utilisateur, comme son nom, son prénom, son email et son mot de passe.

    - Création d'un fichier .env.dev.local
    - Ajout de la connexion string au fichier .env.dev.local
    - Ensuite créer la BDD `symfony console doctrine:database:create`
