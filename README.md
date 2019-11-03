## face_recognition_crop
Reconnaissance de visage dans une video et enregistré dans un dossier
# Reconnaître, rogner et enregistrer des visages sous forme d'images à partir d'une vidéo

Pour les détails techniques, !
Si vous souhaitez étudier un 
aspect de la reconnaissance faciale ou de la détection faciale. Une chose que vous allez vouloir est 
une variété de visages que vous pouvez utiliser pour votre système. Vous pouvez créer votre propre base 
de données de détection / reconnaissance de visage par ce programme. [face_recognizer.py] 
(https://github.com/rlamah05/face_recognition_crop/blob/master/face_recognizer.py)
reconnaît les visages de la vidéo, les recadre et les enregistre en tant qu'image dans la hiérarchie appropriée.

Une fois les données de visage acquises, nous devrons les lire dans notre programme. Dans les applications 
de démonstration, j'ai décidé de lire les images à partir d'un fichier CSV très simple. Pourquoi? 
Parce que c’est l’approche la plus simple, indépendante de la plate-forme, à laquelle je peux penser. 
Cependant, si vous connaissez une solution plus simple, veuillez m'envoyer une requête ping à ce sujet. 
Fondamentalement, tout fichier CSV doit contenir des lignes composées d'un nom de fichier suivi d'un;
suivi du libellé (sous forme de nombre entier).

## INSTALLATION
 **1.) Python and pip**

Python est automatiquement installé sur Ubuntu. Prenez un moment pour confirmer (en émettant une commande python -V)
l’une des versions suivantes de Python est déjà installée sur votre système:


- Python 2.7
- Python 3.3+

Le gestionnaire de paquets pip ou pip3 est généralement installé sur Ubuntu. Prenez un moment pour confirmer
(en émettant une commande * pip -V * ou * pip3 -V *) que pip ou pip3 est installé. Nous recommandons fortement
version 8.1 ou supérieure de pip ou pip3. Si la version 8.1 ou ultérieure n'est pas installée, 
lancez la commande suivante qui installera ou mettra à niveau vers la dernière version de pip:

    $ sudo apt-get install python-pip python-dev   # for Python 2.7
    $ sudo apt-get install python3-pip python3-dev # for Python 3.n
    
**2.) dlib**

Install dlib prerequisites

La bibliothèque dlib n'a que quatre conditions préalables principales:
Boost
Boost.Python
CMake
X11/XQuartx

L'installation de CMake, Boost, Boost.Python et X11 peut être réalisée facilement avec ** apt-get **:

    $ sudo apt-get install build-essential cmake
    $ sudo apt-get install libgtk-3-dev
    $ sudo apt-get install libboost-all-dev
    
    $ wget https://bootstrap.pypa.io/get-pip.py
    $ sudo python get-pip.py
    
Installer dlib avec des liaisons Python

La bibliothèque dlib n’a pas de prérequis Python, mais si vous prévoyez d’utiliser dlib pour tout type
de la vision par ordinateur ou du traitement d’images, je recommanderais l’installation:


- NumPy
- SciPy
- scikit-image

Ces packages peuvent être installés via pip:

    $ pip install numpy
    $ pip install scipy
    $ pip install scikit-image
    
Il y a des années, nous devions compiler dlib manuellement à partir du source (de la même manière que nous installons OpenCV).
Cependant, nous pouvons maintenant utiliser pip pour installer dlib:

    $ pip install dlib
    
**3.) face_recognition 1.2.1**
Dans ce projet, le système de reconnaissance faciale de [Adam Geitgey] (https://github.com/ageitgey/face_recognition)
(* grâce à Adam *) a été utilisé par pypi à l’aide de pip3 ( ou pip2 pour Python 2):
    
     pip3 install face_recognition

## USAGE

Il suffit d'executer *face_recognizer.py*
## CITATION
Si vous utilisez ce code pour vos publications, veuillez le citer comme suit:

     @ONLINE {frc,
         author = "Lamah Richard",
         title = "Créateur de base de données de visages",
         année = "2019",
         url = "https://github.com/rlamah05/face_recognition_crop"
     }

## AUTEUR
Lamah Richard

## LICENCE
Ce système est disponible sous licence MIT. Voir le fichier LICENSE pour plus d'informations.
