# ML-FinalProjet
Projet final de Machine Learning, école 2600

## 1. Quels modèles avez-vous testés ? Expliquer.

Nous avons testé RandomForestClassifier, qui est un choix courant pour les problèmes de classification en raison de sa robustesse et de sa capacité à gérer des ensembles de données complexes. 

## 2. Quel modèle avez-vous utilisé dans votre soumission finale ? Pourquoi ?

Nous avons sélectionner le modèle par rapport à ce qu'il nous semblé le plus pertinent pour notre ensemble de données.

RandomForestClassifier à pour capacité à gérer efficacement les données hétérogènes
RandomForestClassifier peu résoudre des problèmes de régression (variable cible numérique) et de classification (variable cible catégorique). 
RandomForestClassifier utilise une méthode d'ensemble, ce qui signifie qu'elles combinent les prédictions d'autres modèles.

## 3. Quels hyperparamètres associés au modèle final avez vous utilisé ?

Nous avons essayer utilisé ces hyperparamètres :

- `n_estimators=100`: Le nombre d'arbres dans la forêt. Nous avons choisi une valeur raisonnable pour équilibrer la performance et le coût de calcul.
- `random_state=42`: Pour assurer la reproductibilité des résultats, en fixant la graine aléatoire.

Ces valeurs ont été choisies après des expérimentations et des ajustements pour garantir une bonne performance sans surajustement excessif.

Etant sur des Toaster le temps de traitement ne sais jamais fini / (ou sinon on à fais quelque chose de mal mais on sais pas quoi)

## 4. Quelles variables ont le plus d'influence dans votre prédiction ?

Pour identifier les variables les plus influentes dans la prédiction, nous avons utilisé des techniques d'importance des fonctionnalités fournies par le RandomForestClassifier. Ces techniques attribuent des scores à chaque variable en fonction de leur contribution à la réduction de l'impureté des arbres de décision. Les variables avec des scores plus élevés sont considérées comme plus influentes dans la prédiction.

## 5. Comment avez-vous géré la liste des imports et des exports ?

Nous avons fait le choix de ne pas utiliser les listes d'imports et d'exports car trop complexes à utiliser (encodage correct, etc).

## 6. L'utilisation de l'accuracy pour évaluer votre modèle fait-elle sens ? Pourquoi ?

L'utilisation de l'accuracy comme métrique d'évaluation a du sens dans notre cas, car notre problème est de l'ordre de la classification et semble être équilibré. Nous cherchons à maximiser le nombre de prédictions correctes globales. Cependant, nous devons également être conscients des limites de l'accuracy, en particulier si notre ensemble de données présente un déséquilibre entre les classes. Dans de tels cas, d'autres métriques d'évaluation peuvent être nécessaires pour une compréhension plus approfondie de la performance du modèle.

##    Quelle autre métrique d'évaluation auriez-vous pu utiliser ? Expliquer.

Une métrique alternative que nous aurions pu utiliser est l'AUC-ROC. Cette métrique est particulièrement pertinente lorsque l'équilibre entre les classes est crucial. Elle évalue la capacité du modèle à discriminer entre les classes, même en tenant compte du déséquilibre. Cela aurait fourni une perspective plus complète de la performance du modèle, en particulier dans des scénarios où la sensibilité et la spécificité sont cruciales.
L’aire sous la courbe ROC est donc un indicateur de la performance globale du modèle.

## 7. Afficher la matrice de confusion et expliquer vos résultats.

Afficher la matrice de confusion nous permet de visualiser les performances du modèle en termes de vrais positifs, vrais négatifs, faux positifs et faux négatifs. En interprétant cette matrice, nous pouvons évaluer la précision, le rappel et d'autres métriques de performance. Les résultats de la matrice de confusion nous aident à comprendre les erreurs spécifiques que le modèle commet, ce qui peut orienter d'éventuelles améliorations ou ajustements du modèle.
