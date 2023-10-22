#0x00. Clone AirBnB – La console

## 0x00.Table des matières

* [0x01 Introduction](#0x01-Introduction)
* [Environnement 0x02](#0x02-Environnement)
* [Installation 0x03](#0x03-Installation)
* [Test 0x04](#0x04-Test)
* [Utilisation 0x05](#0x05-Utilisation)
* [0x06 Auteurs](#0x06-Auteurs)

## 0x01 Introduction

Projet d'équipe pour créer un clone de [AirBnB](https://www.airbnb.com/).

La console est un interpréteur de commandes pour gérer l'abstraction des objets entre les objets et la façon dont ils sont stockés.

Pour voir le contexte fondamental du projet, visitez le [Wiki](https://github.com/ralexrivero/AirBnB_clone/wiki).

La console effectuera les tâches suivantes :

* créer un nouvel objet
* récupérer un objet à partir d'un fichier
* faire des opérations sur des objets
* détruire un objet

### Stockage

Toutes les classes sont gérées par le moteur `Storage` dans la classe `FileStorage`.

## 0x02 Environnement

<!-- ubuntu -->
<a href="https://ubuntu.com/" target="_blank"> <img height="" src="https://img.shields.io/static/v1?label=&message=Ubuntu&color=E95420&logo =Ubuntu&logoColor=E95420&labelColor=2F333A" alt="Suite CRM"></a> <!-- bash --> <a href="https://www.gnu.org/software/bash/" target="_blank "> <img height="" src="https://img.shields.io/static/v1?label=&message=GNU%20Bash&color=4EAA25&logo=GNU%20Bash&logoColor=4EAA25&labelColor=2F333A" alt="terminal">< /a> <!-- python--> <a href="https://www.python.org" target="_blank"> <img height="" src="https://img.shields.io /static/v1?label=&message=Python&color=FFD43B&logo=python&logoColor=3776AB&labelColor=2F333A" alt="python"></a> </a> <!-- vim --> <a href="https:// www.vim.org/" target="_blank"> <img height="" src="https://img.shields.io/static/v1?label=&message=Vim&color=019733&logo=Vim&logoColor=019733&labelColor=2F333A" alt="Suite CRM"></a> <!-- vs code --> <a href="https://code.visualstudio.com/" target="_blank"> <img height="" src= "https://img.shields.io/static/v1?label=&message=Visual%20Studio%20Code&color=5C2D91&logo=Visual%20Studio%20Code&logoColor=5C2D91&labelColor=2F333A" alt="Suite CRM"></a> </ a><!-- git --> <a href="https://git-scm.com/" target="_blank"> <img height="" src="https://img.shields.io /static/v1?label=&message=Git&color=F05032&logo=Git&logoColor=F05032&labelColor=2F333A" alt="système de contrôle de version distribué git"></a> <!-- github --> <a href="https:// github.com" target="_blank"> <img height="" src="https://img.shields.io/static/v1?label=&message=GitHub&color=181717&logo=GitHub&logoColor=f2f2f2&labelColor=2F333A" alt=" GitHub"></a>
 <!-- Directives de style -->
* Directives de style :
  * [pycodestyle (version 2.7.*)](https://pypi.org/project/pycodestyle/)
  * [PEP8](https://pep8.org/)

Tous les développements et tests ont été exécutés sur un système d'exploitation Ubuntu 20.04 LTS utilisant le langage de programmation Python 3.8.3. Les éditeurs utilisés étaient VIM 8.1.2269, VSCode 1.6.1 et Atom 1.58.0 . Version de contrôle utilisant Git 2.25.1.

## 0x03Installation

```bash
git clone https://github.com/aysuarex/AirBnB_clone.git
```

accédez au répertoire `AirBnb` et exécutez la commande :

```bash
 ./console.py
```

### Exécution

En mode interactif

```bash
$ ./console.py
(hbnb) aide

Commandes documentées (tapez help <topic>) :
========================================
EOF aide à arrêter

(hbnb)
(hbnb)
(hbnb) quitter
$
```

en mode non interactif

```bash
$ echo "aide" | ./console.py
(hbnb)

Commandes documentées (tapez help <topic>) :
========================================
EOF aide à arrêter
(hbnb)
$
$ chat test_help
aide
$
$ chat test_help | ./console.py
(hbnb)

Commandes documentées (tapez help <topic>) :
========================================
EOF aide à arrêter
(hbnb)
$
```

## 0x04 Test

Tous les tests sont définis dans le dossier `tests`.

### Documentation

* Modules:

```python
python3 -c 'print(__import__("mon_module").__doc__)'
```

* Des classes:

```python
python3 -c 'print(__import__("mon_module").MaClasse.__doc__)'
```

* Fonctions (à l'intérieur et à l'extérieur d'une classe) :

```python
python3 -c 'print(__import__("mon_module").ma_fonction.__doc__)'
```

et

```python
python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'
```

### Tests unitaires Python

* module de test unitaire
* Extension de fichier ``` .py ```
* Les fichiers et dossiers sont suivis de ```test_```
* Organisation : pour ```models/base.py```, tests unitaires dans : ```tests/test_models/test_base.py```
* Commande d'exécution : ```python3 -m unittest discover tests```
* ou : ```python3 -m unittest tests/test_models/test_base.py```

### exécuter le test en mode interactif

```bash
echo "python3 -m unittest découvrir les tests" | frapper
```

### exécuter le test en mode non interactif

Pour exécuter les tests en mode non interactif, et découvrir l'intégralité du test, vous pouvez utiliser la commande :

```bash
python3 -m unittest découvrir les tests
```


## 0x05 Utilisation

* Démarrez la console en mode interactif :

```bash
$ ./console.py
(hbnb)
```

* Utilisez l'aide pour voir les commandes disponibles :

```bash
(hbnb) aide

Commandes documentées (tapez help <topic>) :
========================================
EOF tous les comptes créer détruire aider à quitter afficher la mise à jour

(hbnb)
```

* Quittez la console :

```bash
(hbnb) quitter
$
```

### Commandes

> Les commandes sont affichées au format suivant *Commande / utilisation / exemple avec sortie*

* Créer

> *Crée une nouvelle instance d'une classe donnée. L'ID de la classe est imprimé et l'instance est enregistrée dans le fichier file.json.*

```bash
créer <classe>

```

```bash
(hbnb) créer un modèle de base
6cfb47c4-a434-4da7-ac03-2122624c3762
(hbnb)
```

* Montrer

```bash
afficher <classe> <id>
```

```bash
(hbnb) afficher le modèle de base 6cfb47c4-a434-4da7-ac03-2122624c3762
[BaseModel] (a) [BaseModel] (6cfb47c4-a434-4da7-ac03-2122624c3762) {'id' : '6cfb47c4-a434-4da7-ac03-2122624c3762', 'created_at' : datetime.datetime(2021, 11, 14 , 3, 28, 45, 571360), 'updated_at' : datetime.datetime(2021, 11, 14, 3, 28, 45, 571389)}
(hbnb)
```

* Détruire

> *Supprime une instance d'une classe donnée avec un ID donné.*
> *Mettre à jour le fichier.json*

```bash
(hbnb) créer un utilisateur
0c98d2b8-7ffa-42b7-8009-d9d54b69a472
(hbnb) détruire l'utilisateur 0c98d2b8-7ffa-42b7-8009-d9d54b69a472
(hbnb) afficher l'utilisateur 0c98d2b8-7ffa-42b7-8009-d9d54b69a472
** aucune instance trouvée **
(hbnb)
```

* tous

> *Imprime toutes les représentations sous forme de chaîne de toutes les instances d'une classe donnée.*
> *Si aucun cours n'est réussi, tous les cours sont imprimés.*

```bash
(hbnb) créer un modèle de base
e45ddda9-eb80-4858-99a9-226d4f08a629
(hbnb) tous les modèles de base
["[BaseModel] (4c8f7ebc-257f-4ed1-b26b-e7aace459897) [BaseModel] (4c8f7ebc-257f-4ed1-b26b-e7aace459897) {'id' : '4c8f7ebc-257f-4ed1-b26b-e7aace459897', 'créé_à' : datetime.datetime(2021, 11, 13, 22, 19, 19, 447155), 'updated_at' : datetime.datetime(2021, 11, 13, 22, 19, 19, 447257), 'name' : 'Mon premier Modèle', 'mon_numéro' : 89}"]
["[ModeBase
```

* compter

> *Imprime le nombre d'instances d'une classe donnée.*

```bash
(hbnb) créer une ville
4e01c33e-2564-42c2-b61c-17e512898bad
(hbnb) créer une ville
e952b772-80a5-41e9-b728-6bc4dc5c21b4
(hbnb) compter Ville
2
(hbnb)
```

* mise à jour

> *Mise à jour une instance en fonction du nom de classe, de l'identifiant et des kwargs transmis.*
> *Mettre à jour le fichier.json*

```bash
(hbnb) créer un utilisateur
1afa163d-486e-467a-8d38-3040afeaa1a1
(hbnb) mise à jour de l'utilisateur 1afa163d-486e-467a-8d38-3040afeaa1a1 email "aysuarex@gmail.com"
(hbnb) afficher l'utilisateur 1afa163d-486e-467a-8d38-3040afeaa1a1
[Utilisateur] (s) [Utilisateur] (1afa163d-486e-467a-8d38-3040afeaa1a1) {'id' : '1afa163d-486e-467a-8d38-3040afeaa1a1', 'created_at' : datetime.datetime(2021, 11, 14 , 23, 42, 10, 502157), 'updated_at' : datetime.datetime(2021, 11, 14, 23, 42, 10, 502186), 'email' : 'aysuarex@gmail.com'}
(hbnb)

```
## Auteurs
<détails>
    <summary>Ayomide Suara</summary>
    <ul>
    <li><a href="https://www.github.com/aysuarex">Github</a></li>
    <li><a href="https://www.twitter.com/Aysuarex">Twitter</a></li>
    <li><a href="mailto:aysuarex@gmail.com">e-mail</a></li>
    </ul>
</détails>
<détails>
    <summary>Bamidele Adefolaju</summary>
    <ul>
    <li><a href="https://www.github.com/lexxyla">Github</a></li>
    <li><a href="https://www.twitter.com/lexxyla">Twitter</a></li>
    <li><a href="mailto:bamideleadefolaju@gmail.com">e-mail</a></li>
    </ul>
</détails>

