# Projet_Personnel_Fraude_Carte_Credit
### Transactions par carte de crédit anonymisées étiquetées comme frauduleuses ou authentiques.

## Contexte
Il est important que les sociétés émettrices de cartes de crédit soient en mesure de reconnaître les transactions frauduleuses par carte de crédit afin que les clients ne soient pas facturés pour des articles qu'ils n'ont pas achetés.

## Contenu
L'ensemble de données contient les transactions effectuées par carte de crédit en septembre 2013 par des titulaires de cartes européens.
Cet ensemble de données présente les transactions survenues en deux jours, où nous avons 492 fraudes sur 284 807 transactions. L'ensemble de données est très déséquilibré, la classe positive (fraudes) représentant 0,172% de toutes les transactions.

Il contient uniquement des variables d'entrée numériques qui sont le résultat d'une transformation PCA. Malheureusement, en raison de problèmes de confidentialité, nous ne pouvons pas fournir les caractéristiques originales ni davantage d'informations générales sur les données. Les fonctionnalités V1, V2, … V28 sont les principales composantes obtenues avec PCA, les seules fonctionnalités qui n'ont pas été transformées avec PCA sont 'Time' et 'Amount'. La fonctionnalité « Temps » contient les secondes écoulées entre chaque transaction et la première transaction de l'ensemble de données. La fonctionnalité « Montant » correspond au montant de la transaction. Cette fonctionnalité peut être utilisée pour un apprentissage sensible aux coûts, en fonction d'un exemple. La fonctionnalité 'Class' est la variable de réponse et elle prend la valeur 1 en cas de fraude et 0 sinon.

Compte tenu du rapport de déséquilibre de classe, nous recommandons de mesurer la précision à l’aide de l’aire sous la courbe de précision-rappel (AUPRC). La précision de la matrice de confusion n’est pas significative pour une classification déséquilibrée.
## Livrables:
* Votre code en Python contenant : 
  * l’ensemble des traitements effectués sur les données;
  * Modélisation;
  * Sauvegarde et déploiement du modèle final;
  * Application du modèle final puis prédiction.
## Compétences évaluées:
- [x] Tester différents modèles d'apprentissage supervisé automatique pour la détection de fraude par carte de crédit (sur des données déséquilibrées).
- [x] Évaluer les performances d’un modèle d'apprentissage (sur des données déséquilibrées) avec une métrique adapté au problème métier.
- [x] Passer au technique de rééchantillonnage des données (classe cible)
- [x] Réévaluer les performances d’un modèle d'apprentissage (sur des données équilibrées après rééchantillonnage)
