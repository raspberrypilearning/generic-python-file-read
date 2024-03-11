Om een tekstbestand in Python te lezen, moet je het bestand `openen` en dan de inhoud ervan `lezen`.

Gebruik bij het openen van het bestand `with` en `as`.  Dit zorgt ervoor dat, wanneer je ingesprongen code is uitgevoerd, het bestand automatisch wordt gesloten. Als je bestanden sluit die je niet nodig hebt, bespaar je geheugen op je computer.

```python
with open(bestandsnaam) as f:
```

Waarbij `bestandsnaam` de naam is van het bestand dat je opent, bijvoorbeeld `'info.txt'`.

Nadat je je bestand hebt geladen, kun je het hele bestand in een tekststring veranderen. Of je kunt een `for` lus gebruiken om regel voor regel door het bestand te gaan.

### Verander het hele bestand in een tekststring
Het bestand wordt geladen in de variabele `f`, maar niet als een tekststring waarmee Python kan werken. Om het bestand als tekst te krijgen, moet je `read()`gebruiken.

```python
with open(bestandsnaam) as f:
  bestand_tekst = f.read()
  # Doe iets met de tekst
```

### Loop door het bestand, regel voor regel
Het bestand wordt geladen in de variabele `f`. Je kunt een `for` lus gebruiken om dezelfde code op elke regel van het bestand uit te voeren.

```python
with open(bestandsnaam) as f:
  for bestand_regel in f:
    # Doe iets met de regel
```