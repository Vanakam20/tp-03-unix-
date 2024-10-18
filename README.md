# tp-03-unix-

# Exercices Bash

## Exercice 1 : Paramètres

```bash
#!/bin/bash

# Compter le nombre de paramètres
nombre_parametres=$#

# Récupérer le nom du script
nom_script=$0

# Récupérer le troisième paramètre s'il existe
troisieme_parametre=${3:-"Non disponible"}

# Afficher les paramètres
echo "Bonjour, vous avez rentré $nombre_parametres paramètre(s)."
echo "Le nom du script est $nom_script."
echo "Le 3ème paramètre est $troisieme_parametre."
echo "Voici la liste des paramètres : $@"

chmod +x analyse.sh
./analyse.sh param1 param2 param3 param4

