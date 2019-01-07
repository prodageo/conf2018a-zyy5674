# Titre

## Cartouche d'identification

 - Manifestation : CodeursEnSeine 2017
 - Lieu : Université de Rouen - site du Madrillet
 - Conférence : Personnalisation et Système de Recommandation chez vente-privée
 - Horaire de la conférence : 12h
 - Durée de la conférence : 15 minutes
 - Conférencier(s) :
   - Betty Moreschini (Twitter: @bettymoreschini)
 - Audience : 50 à 100 personnes
 - Auteur du billet : Zhenghui Zhu
 - Mots-clés : Recommandation, User portrait, classement
 - URL de l'illustration : ![Mettre votre image, Photo by Oscar Keys on Unsplash](oscar-keys-58399-unsplash.jpg)
   

## Support
 - Lien vers le support (diapos) présenté en conférence
 - Nombre de diapos du support : Non dispo
 - Plan du support :
   -L'entreprise 
   -Le site web avec recommandation
   -Le système de recommandation 
   -Les modifications à apporter

## Résumé
Vente-privée est un site d'achat spécialisé en 'Déstockage'. Son modèle commerçant est de proposer aux utilisateurs inscrits les produits à des prix réduits pendant une durée limitée. L'inscription est obligatoire pour consulter les produits et les marques disponibles. Chaque jour, Vente-Privée organise les événement de déstockage pour au moins 150 marques différentes.

La page d'accueil du site a été présentée. L'élément essentiel de la page est ses recommandations proposées en fonction de l'utilisateur connecté. Le but est de mettre en avant les marques les plus intéressantes pour le client car plus celui-ci fait défiler la page, moins il a des chances d'acheter. Le A/B test de ce système a présenté des résultats prometteurs: +4% d'entrée en vente et +2.3% de vente conclue pour les clients concernés, comparé avec l'ancien système de recommandation statique.

Le système fonctionne via Real-Time Activity Tracking With Kafka. Pour chaque paire de produit/ utilisatuer, le système propose un 'Product aggeregator score' qui represente la possiblité que l'utilisatuer acheter ce produit. Ce noté est estimée avec machine learning en fonction d'un enregistrement des opérations utilisateurs effectuées. Le système de recommandation applique un filtrage d'estimation collaboratif qui s'appelle 'Démographie affinité popularité'. Après, le système calcule un classement final en fonction du final score et diversification. Chaque 15 minutes, les recommandations sont mis à jour.

Le système se heurte pour le moment à certaines difficultés. En effet, l'électroménager est de loin la catégorie de produits la plus vendue et a tendance à trop influencer la prédiction des autres catégories. De plus, la répartition des articles en genre est parfois mauvaise dans certains cas.

## Architecture et facteur qualité
...
