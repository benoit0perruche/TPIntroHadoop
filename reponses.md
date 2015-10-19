# Question 1.1 :

1. **À quoi correspondent les compteurs**
	* **`Map input records`** : cette valeur représente le nombre d'objets que map a traité. Cela correspond ici le nombre de lignes du fichier texte en input.
	
	* **`Map output records`** : cette valeur représente le nombre d'objets que `map` va envoyer à la fonction `reduce` ici le nombre d'éléments (séparés par un espace) du texte.

2. **Quel est le lien entre `Map output records` et `Reduce input records`?**

`Map output records` compte le nombre de valeurs envoyéès à `reduce`, `Reduce input records` correspond donc aux nombre de valeurs reçues par `reduce`. 
Nous n'avons pas utilisé de Combiners, nous voyons donc que `reduce` a bien traité toutes les valeurs qui ont été générées par le `map`.

3. **À quoi correspond `Reduce input groups` ?**

Le compteur `Reduce input groups` correspond aux nombre de clés uniques transmises à `reduce`.