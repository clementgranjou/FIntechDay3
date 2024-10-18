# FIntechDay3

> Les rendus finaux se trouvent dans le dossier course2.

##### 1. Accuracy du modèle Multinomial Naive Bayes
L'accuracy de 0.8558 indique que 85,58 % des prédictions faites par le modèle sont correctes. Cela signifie que dans 85,58 % des cas, le modèle a correctement classé les critiques comme positives ou négatives.

L'accuracy, bien qu'importante, n'est pas toujours suffisante pour évaluer un modèle, surtout si le jeu de données est déséquilibré (si une classe est représentée de manière significativement plus importante que l'autre). Toutefois, dans ce cas précis, le dataset des critiques de films IMDB est équilibré (50 % de critiques positives et 50 % de critiques négatives), ce qui signifie que l'accuracy donne une bonne idée de la performance globale du modèle.


##### 2. Rapport de Classification :
Ce rapport affiche la précision, le rappel, et le F1-score pour chaque classe (négatif et positif).

Classe Négative (Negative) :

Précision (0.86) : Sur toutes les critiques prédites comme négatives, 86 % étaient réellement négatives.
Rappel (0.85) : Sur toutes les critiques réellement négatives, 85 % ont été correctement identifiées par le modèle.
F1-score (0.85) : La moyenne harmonique entre la précision et le rappel, donc un bon équilibre entre les deux métriques pour la classe négative.
Classe Positive (Positive) :

Précision (0.85) : Sur toutes les critiques prédites comme positives, 85 % étaient réellement positives.
Rappel (0.86) : Sur toutes les critiques réellement positives, 86 % ont été correctement identifiées par le modèle.
F1-score (0.86) : Ce qui montre également un bon équilibre entre précision et rappel pour la classe positive.
Accuracy (0.86) : Le modèle a correctement classé 86 % des critiques, un score globalement solide pour une classification binaire.

Macro avg et Weighted avg (0.86) : Ces moyennes montrent que le modèle traite bien les deux classes de manière équilibrée.

##### 3. Matrice de Confusion :
La matrice de confusion donne des informations plus détaillées sur les erreurs de classification :

True Negatives (TN) = 2106 : Le modèle a correctement prédit 2106 critiques comme négatives.
False Positives (FP) = 375 : Le modèle a prédit à tort 375 critiques comme positives alors qu'elles étaient négatives.
False Negatives (FN) = 346 : Le modèle a prédit à tort 346 critiques comme négatives alors qu'elles étaient positives.
True Positives (TP) = 2173 : Le modèle a correctement prédit 2173 critiques comme positives.
Interprétation :
Le modèle a de bonnes performances avec une précision et un rappel similaires pour les classes négative et positive.
Erreur la plus courante : Le modèle a tendance à confondre certaines critiques négatives avec des positives (375 faux positifs), mais aussi des critiques positives avec des négatives (346 faux négatifs). Cela montre que le modèle est équilibré dans les deux types d'erreurs.
