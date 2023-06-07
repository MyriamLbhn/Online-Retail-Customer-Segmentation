# Online_Retail-Customer_segmentation

Dans le cadre de la mission pour UK Retail, en tant que Data scientist, on utilisera des techniques de segmentation client pour améliorer l'efficacité des campagnes marketing en identifiant des groupes de clients similaires et en adaptant les stratégies en conséquence.  
Vous pouvez accéder à la présentation Google slide [ici](https://docs.google.com/presentation/d/1tXZAzQ3QNI2SOmmIZfHz5AXhh-NkBpFlGZV-PqoIUaU/edit?usp=sharing)

## Objectifs

En tant que data scientist, notre mission consiste à :

- analyser et nettoyer le dataset fourni
- faire une seglentation client
- proposer un contrat de maintenance (stabilité de la segmentation dans le temps)
- proposer des actions marketing

## Arborescence des fichiers

Ce projet est organisé en plusieurs fichiers et dossiers :

*nettoyage.ipynb* : Opération de nettoyage des données brutes  

*Update_features_cluster.ipynb* : Fonction pour calculer directement les 6 features (RFM + 3 extras)  

*Analyse 2009-2010* : Contient les notebook pour effectuer la segmentation client sur l'année 2009/2010
- *groupby _customer_rfm_2009-2010.ipynb*: création du dataset groupé par client, création de 6 features pour la segmentation (RFM + 3 extras)
- *clustering_2009-2010.ipynb*: Algorithme de segmentation client (k-means)

*Analyse 2009-2011*: Contient les notebook pour effectuer la segmentatio client sur l'ensemble du dataset

*ARI maintenance*: Contient les notebook et données relatives au calcul du score ARI (pour proposer un contrat de maintenance)
- *ARI_maintenance.ipynb*
- *data ARI*: Contient les fichiers csv des données clients à J+1, J+15, M+1, ..., M+12

*dataset*: Contient les dataset crée lors des différentes analyses:
- *clean_online_retail.csv*: Données clients 2009/2011 après nettoyage
- *rfm_2009-2010*: Dataset des données RFM + extra features sur les données 2009/2010
- *rfm.csv*: Dataset des données RFM + extra features sur les données 2009/2011
- *rfm_filtered_2009-2010.csv*: Dataset des données RFM + extra features sur les données 2009/2010, filtrée (suppression des 2% de clients qui font le plus d'achat = grossistes)
- *rfm_filtered.csv*: Dataset des données RFM + extra features sur les données 2009/2011, filtrée (suppression des 2% de clients qui font le plus d'achat = grossistes)

*img*: Contient les graphiques de performance de l'entreprise
