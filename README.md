<h1><p align="center"> PROJET DE MACHINE LEARNING FOR NLP </p></h1>
<h3><p align="center"> (vueillez prendre le temps, svp, de lire le ce readme) </p></h3>

<p align="center">
  <br><br>
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/LOGO-ENSAE.png/480px-LOGO-ENSAE.png", width="300", height="200">
</p>


<p align="center">Réalisé par :</p>

<p align="center">ESSOH Lasme Ephrem Dominique (DSSA)</p>
<p align="center">CHABAUD Mathieu (DSSS)</p>
<p align="center">BERREBI Nathan (DSSA)</p>

<p align="center">Elèves-Ingénieurs 3A (2021 - 2022)</p>
<p align="center">Thème :</p>
<h4><p align="center">Analyses textuelles sur Amazon Product Data : sentiment analysis and texts generation</p></h4>

# Description de ce repos

Ce repos github s'inscrit dans le cadre du projet de Machine Learning for NLP. Il comprend l'ensemble des fichiers sources de notre groupe, principalement des fichiers notebooks écrits en Python. Ce repos peut être cloné et exécuté dans un calpin jupyter, en local, en prenant le soin de reproduire d'abord l'environnement python : <a href  ="https://github.com/lasme-ephrem/nlp_project/blob/main/requirements.txt"> requirements.txt <a/>. Il peut aussi être exécuté directement depuis le lien Google Colab ci-dessous.

### Liens Google Colab 
  Notebook principale : <a href="https://colab.research.google.com/drive/1N1I8gShlDpqSw53JlkRSr7ZSE28TtUsZ?usp=sharing"> MAIN COLAB.<a/>
  Notebook du transfert du LSTM : <a href="https://colab.research.google.com/drive/1i5zehYMtjF6N2Nn3f0aB5XStkQSI_6ne?usp=sharing">TRANSFERT COLAB.<a/>

### Structure du travail
  
  Le fichier principal de ce projet est le notebook suivant <a href ="https://github.com/lasme-ephrem/nlp_project/blob/main/rapport_notebook_nlp_project.ipynb"> notebook_projet_NLP <a/> (<a href="https://colab.research.google.com/drive/1N1I8gShlDpqSw53JlkRSr7ZSE28TtUsZ?usp=sharing"> Lien Colab.<a/>). Ce notebook télécharge automatiquement les données dépuis notre espace de stockage s3, les prétraite puis applique différents modèles sur ceux-ci qui sont exportés dans le dossier <a href ="https://github.com/lasme-ephrem/nlp_project/tree/main/Modeles"> Modeles <a/>. Dans ce dossier, figure en particulier notre modèle LSTM exporté qui est utilisé pour le transfert d'apprentissage sur un sample du jeu de données <a href = "https://github.com/lasme-ephrem/nlp_project/blob/main/Movies_TV_low.csv"> Movie and TV<a/>. Ainsi pour exécuter le notebook <a href = "https://github.com/lasme-ephrem/nlp_project/blob/main/rapport_notebook_nlp_transfert.ipynb"> notebook_transfer_nlp<a/> (<a href="https://colab.research.google.com/drive/1i5zehYMtjF6N2Nn3f0aB5XStkQSI_6ne?usp=sharing">Lien Colab.<a/>), de manière indépendante c'est-à-dire sans passer par l'exécution du notebook principal, il faut s'assurer que le dossier <a href ="https://github.com/lasme-ephrem/nlp_project/tree/main/Modeles"> Modeles <a/> existe bien et contient le fichier <a href ="https://github.com/lasme-ephrem/nlp_project/tree/main/Modeles/best_LSTM_model.pt"> best_LSTM_model.pt<a/>  que ce soit en local ou sur Colab.

 ### Référen ce travail
  
  Pour batir ce travail, nous nous sommes inspirés des références suivantes :
  
  <a href ="https://github.com/Rebecasarai/Amazon-reviews-sentiment-analysis-pytorch">Référence 1 (sentiment analysis)<a/>
    
  <a href ="https://www.kaggle.com/code/rahuldshetty/text-summarization-in-pytorch/notebook">Référence 2 (text summarization)<a/>
