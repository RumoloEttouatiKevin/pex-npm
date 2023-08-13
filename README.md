# PEX-npm

## Installation de npm

- [Installer npm](https://github.com/RumoloEttouatiKevin/personal-documentation/blob/main/Linux/install-Ubuntu22.04-with-VirtualBox7.0.10.md#11-installation-de-npm) sur Ubuntu

## Initialisation d'un nouveau projet

- `npm init`
  - Saisir les informations demandé
    - ? (git repository) est l'url ssh du repo (ex : **[git@github.com:RumoloEttouatiKevin/pex-npm.git](https://github.com/RumoloEttouatiKevin/pex-npm)**)
    - ? (author) son identité (j'utilise celle de github -> **Rumolo-Ettouati Kévin**)
    - ? (license) [code de la licence](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository) choisi (j'utilise généralement -> **MIT**)

Un dossier **node_modules** vient à être créé à la racine du projet, celui-ci contiendra tous les paquets/dépendance installé. Il faut penser à l'ignorer si l'on souhaite poussé le projet sur un repo distant type **GitHub**.

## Ajouter un package JS

Installation d'un paquet en utilisant npm.

Exemple :

- `npm install create-nuxt-app`
- `npm install datatables.net-dt`

## Installation d'un projet en local

La quasi totalité des projets ne fournissent pas le dossier **node_modules** pour éviter de les alourdir inutilement, une fois le projet en local, il faut donc installer les paquets pour que celui-ci soit fonctionnel.

!! Les informations des paquets installé dans un projet et leurs versions sont dans le fichier **package-lock.json**, c'est avec celui-ci que npm pourra installer le projet en local.

- `npm install`

## Ajout d'un package en local sans impacter le projet

Ceci peut être l'occasion de tester un paquet sans forcément l'associer au projet courant. Ce package ne serra pas ajouté aux informations du fichier **package-lock.json**.

- `npm install bootstrap@5.3.1 --no-save`

## Lister les packages du projet

- `npm list`

## Supprimer un package du projet

- `npm uninstall bootstrap`

## Mise à jour des packages

- Pour savoir si il y a des mise à jour disponible pour les packages du projet.
  - `npm outdated`
- Pour mettre à jour les packages du projet.
  - `npm update`

## Exécuter un script d'un package ou du projet

- `npm run test` **test** étant le nom du script à exécuter.
