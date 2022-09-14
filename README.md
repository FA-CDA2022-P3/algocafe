# L'algo du café

La Fabrique du Numérique a fait l'acquisition d'un robot pour faire le café.

Ce robot doit être programmé, voici les opérations qu'il est capable d'exécuter :

- verser l'eau dans le réservoir
- verser les doses de café dans le filtre
- déclencher le démarrage du café

Votre mission consiste à réaliser la programmation de ce robot avec les règles suivantes :

- on souhaite que le café soit prêt le matin (du lundi au vendredi) à 8h15 (pour l'arrivée des étudiants !)
- en général, le café ne doit pas être lancé après 15h00
- le dosage est le suivant : 
    - pour 12 tasses, 5 doses de café
    - pour 6 tasses, 3 doses de café
- lorsqu'il n'y a plus de café dans la cafetière, le robot doit en lancer un nouveau, de 6 tasses après 15h00, et de 12 tasses par défaut
- lorsqu'il n'y a plus de café moulu (idéalement, on doit connaître le stock de café moulu en nombre de paquets), le robot ne pourra pas lancer le café et enverra une alerte

# Le robot apprend

Avant chaque nouveau lancement, le robot reccueille les avis des consommateurs selon 3 notes possibles :

- -1 si le café est jugé pas assez fort
- 0 si le café est jugé suffisamment fort
- 1 si le café est jugé trop fort

Le robot effectuera ensuite une moyenne des avis arrondie à l'entier le plus proche.
Si le résultat est différent de 0, le robot corrigera les doses de café moulu en augmentant ou en diminuant d'une demi-dose.
