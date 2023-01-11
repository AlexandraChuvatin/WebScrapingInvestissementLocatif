# Web Scraping - Investissement Locatif
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


### 2. Récupération des codes postaux de ces villes
Le code postal des villes nous sera utile ultérieurement. Ces derniers ont été récupérés en utilisant la librairie selenium sur le site https://www.code-postal.com/ .

![image](https://user-images.githubusercontent.com/60775531/211818252-52c72a99-a121-48bd-9acd-9beea65d73bc.png)


### 3. Récupération des tarifs locatifs
Ici, nous utilisons à nouveau la librairie selenium en passant par le site https://www.airbnb.fr/ .
Nous récupérons pour chaque mois, une moyenne des prix pratiqués pour un appartement 1 chambre, 1 sdb, en logement complet.

![image](https://user-images.githubusercontent.com/60775531/211819113-06bae429-c63a-4345-aa0e-f76928d950da.png)


### 4. Récupération des prix moyen par m2
Finalement, nous utilisons selenium pour scraper le site https://www.efficity.com/prix-immobilier-m2/ .

![image](https://user-images.githubusercontent.com/60775531/211819705-6367612c-9ced-4b38-a929-28867e250ba5.png)


## Conclusion

Economisez, investissez, louez !
