# WebScrapingInvestissementLocatif
Projet de Web Scraping s'intéressant à la rentabilité de l'achat d'un bien locatif en France.
L'objectif est de récupérer dans un premier temps les villes les plus touristiques. 
Par la suite, nous récupérons le prix moyen par mois des locations dans chacune des villes via Airbnb.
Finalement, nous récupérons le prix moyen à l'achat du m2 dans chaque ville.


## Pour commencer

Ces instructions vous permettront d'obtenir une copie du projet sur votre machine locale à des fins de développement et de test.

### Prérequis

Vous devez avoir Python 3 installé sur votre machine. Vous pouvez le télécharger depuis le site officiel : https://www.python.org/downloads/.

Vous devrez également installer les paquets Python suivants :
- requests
- bs4 (BeautifulSoup)
- selenium
- pandas
- time
- random

Afin d'installer ces librairies, vous pouvez utiliser le fichier 'requirements.txt':
pip install -r requirements.txt

### Installation

git clone https://github.com/AlexandraChuvatin/WebScrapingInvestissementLocatif.git

## Utilisation

Le code est structuré de la manière suivante:

### 1. Récupération des villes les plus touristiques:
Cette partie utilise les librairies bs4 et requests pour récupérer les informations du site https://www.geo.fr/voyage/decouvrez-le-top-10-des-villes-les-plus-touristiques-de-france-212253 .
![image](https://user-images.githubusercontent.com/60775531/211814157-78fe113c-3a91-4c6a-a1e7-f470169b0e9a.png)
