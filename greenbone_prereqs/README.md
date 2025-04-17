# greenbone_prereqs

Ce rôle installe les prérequis système pour compiler et installer Greenbone/OpenVAS :
- Création de l’utilisateur système et du groupe `gvm`
- Ajout de l’utilisateur courant au groupe
- Création des répertoires nécessaires
- Installation des dépendances de compilation
- Importation de la clé GPG Greenbone

## Utilisation

```yaml
- hosts: all
  become: true
  roles:
    - greenbone_prereqs
