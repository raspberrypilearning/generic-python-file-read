Pour lire un fichier texte en Python, tu dois ouvrir (`open`) le fichier avant de lire (`read`) son contenu.

Pour l'ouverture du fichier, utilise `with` et `as`.  Cela permet de t'assurer que le fichier se fermera automatiquement lorsque ton code indenté aura été exécuté. La fermeture des fichiers dont tu n'as pas besoin économise de la mémoire sur ton ordinateur.

```python
with open(nom_fichier) as f:
```

Où `nom_fichier` est le nom du fichier que tu es en train d'ouvrir, par exemple `'info.txt'`.

Une fois que tu as chargé ton fichier, tu peux transformer le fichier entier en une chaîne de texte. Ou tu peux utiliser une boucle `for` pour parcourir le fichier ligne par ligne.

### Transformer le fichier entier en chaîne de texte
Le fichier est chargé dans la variable `f` , mais pas sous forme de chaîne de texte avec laquelle Python peut travailler. Pour transformer le fichier en texte, tu dois utiliser `read()`.

```python
with open(nom_fichier) as f:
  texte_fichier = f.read()
  # Fais quelque chose avec le texte
```

### Utiliser une boucle pour parcourir le fichier ligne par ligne
Le fichier est chargé dans la variable `f` . Tu peux utiliser une boucle `for` pour exécuter le même code sur chaque ligne du fichier.

```python
with open(nom_fichier) as f:
  for ligne_fichier in f:
    # Fais quelque chose avec la ligne
```