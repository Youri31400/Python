# Installation de Python 3.8 sur Ubuntu

Pour installer Python 3.8 sur Ubuntu, suivre les étapes ci-dessous:

1. **Mettre à jour le système**

    Ouvrir un terminal et exécuter la commande suivante pour mettre à jour la liste des paquets et installer les mises à jour disponibles :

    ``` 
    sudo apt update && sudo apt upgrade -y
    ```

2. **Installer les dépendances**

    Installer les paquets nécessaires pour ajouter un nouveau dépôt avec la commande suivante :

    ``` 
    sudo apt install -y software-properties-common
    ```

3. **Ajouter le dépôt "deadsnakes" PPA**

    Le PPA "deadsnakes" contient plusieurs versions de Python, y compris Python 3.8. Ajouter le PPA avec la commande suivante :

    ``` 
    sudo add-apt-repository ppa:deadsnakes/ppa
    ```

    Confirmer l'ajout du dépôt en appuyant sur "Enter".

4. **Installer Python 3.8**

    Mettre à jour la liste des paquets et installer Python 3.8 avec la commande suivante :

    ``` 
    sudo apt update && sudo apt install -y python3.8
    ```

5. **Vérifier l'installation**

    Vérifier que Python 3.8 est installé en exécutant la commande suivante :

    ``` 
    python3.8 --version
    ```

    Si l'installation a réussi, la version de Python 3.8 sera affichée.

6. **Installer pip pour Python 3.8 (optionnel)**

    Si l'installation de pip pour gérer les paquets Python pour Python 3.8 est souhaitée, exécuter les commandes suivantes :

    ``` 
    sudo apt install -y python3.8-venv python3.8-dev
    wget https://bootstrap.pypa.io/get-pip.py
    python3.8 get-pip.py
    ```

    Ceci installe pip pour Python 3.8, qui pourra être utilisé avec la commande `pip3.8`.