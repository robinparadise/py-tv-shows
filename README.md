# Examen 2º DAM

API de TV Shows
Endpoint: [https://tv-show-dam-default-rtdb.europe-west1.firebasedatabase.app/shows.json](https://tv-show-dam-default-rtdb.europe-west1.firebasedatabase.app/shows.json)

### Ejemplo de uso de la API

```python
import requests

url = "https://tv-show-dam-default-rtdb.europe-west1.firebasedatabase.app/shows.json"
response = requests.get(url)
data = response.json()
print(data)
```

```python
class TVShows:
    def __init__(self):
        self.url = "https://tv-show-dam-default-rtdb.europe-west1.firebasedatabase.app/shows.json"
        ...

    def tvShows(self):
        pass

    def endedShows(self):
        pass

    ...

tvshows = TVShows()
print(tvshows.tvShows())
...

```

1. **(3pts) Crea una función en la clase `TVShows` que muestre una lista de shows de TV. La lista debe consistir solo con los nombres de los shows. La función debe de llamarse `tvShows()`.**

Ejemplo:

```python
Output: ["Under the Dome", "Person of Interest", "Bitten", ...]
```

2. **(2pts) Crea un método dentro de la clase `TVShows` que muestre todos los shows que están en idioma `English`. La función debe de llamarse `showsByLanguage(language)`**

Ejemplo:
```python
Output: ["Under the Dome", "Person of Interest", "Bitten", ...]
```

3. **(3pts) Crea un método dentro de la clase `TVShows` que muestre todos los géneros de los shows. La función debe de llamarse `allGenres()` y no debe de retornar géneros repetidos.**

Ejemplo:
```python
Output: ["Drama", "Science-Fiction", "Thriller", "Action", "Crime", "Horror", "Romance", "Fantasy"]
```

4. **(2pts) Crea un método dentro de la clase `TVShows` que muestre los shows que tienen una duración mayor a 60 minutos. La función debe de llamarse `showsByDuration(duration)`**

Ejemplo:
```python
Output: ["Under the Dome", "Person of Interest", "Bitten", ...]
```

__

## Entrega:

- Duración del exámen 1h
- Sube tu código a un repositorio de GitHub [opcional].
- Envía el enlace de tu repositorio a `robinchogiles@gmail.com`
- Renombra la carpeta y comprímela en un archivo .zip con tu nombre y apellido.
