# L'algo du café : un sujet central pour notre groupe

## Modalités

Travail en petits groupes.

## Mission

La Fabrique du Numérique a fait l'acquisition d'un robot pour faire le café.

Ce robot doit être programmé, voici les opérations qu'il est capable d'exécuter :

- déclencher le démarrage du café
- s'arrêter

Il doit y avoir 2 programmes :

- un programme long qui préparera 12 tasses
- un programme court qui préparera 6 tasses

Votre mission consiste à réaliser la programmation de ce robot avec les règles suivantes :

- on souhaite que le café soit prêt le matin (du lundi au vendredi) à 8h30 (pour l'arrivée des étudiants !)
- en général, le café ne doit pas être lancé après 15h00
- le dosage est le suivant : 
    - pour 12 tasses, 5 doses de café
    - pour 6 tasses, 3 doses de café
- lorsqu'il n'y a plus de café dans la cafetière, le robot doit en lancer un nouveau, de 6 tasses après 15h00, et de 12 tasses par défaut

## Consignes

La simulation doit s'effectuer sur une journée.
Vous pouvez commencer votre programme par le défilement du temps et afficher l'heure courante en console.
Vous pouvez l'initialiser dans une variable (par exemple heure = 8.00) et l'incrémenter dans la boucle du programme avec un setInterval, avec des incrémentations de 15mn).
Les données variables sont l'heure et le niveau du café dans la carafe.
Lorsque le niveau de café est à 0, il faut relancer un café (de 12 tasses par défaut et de 6 tasses après 15h00).

Une action se fera par une fonction réalisant un console.log().
Identifier les variables et les constantes.

Vous aurez également à simuler la consommation du café en décrémentant une variable représentant la quantité restante dans la carafe.

A la fin de la journée, affichez le nombre de cafés préparés, et le nombre de doses consommées.
