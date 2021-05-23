# Pokemons

Projet de programmation mobile réalisé avec kotlin l'application POKEMON affiche la liste de 100 Pokemons avec une RecyclerView et renvoit les informations suivantes : le nom du pokemon son image,sa taille et son poids grace à une API Rest.

### L'api rest :
l'api rest utilisée se trouve à cet endroit [API] (https://pokeapi.co/api/v2)

### archtecture

l'application est composé deux activtés:
- PokeListActivity (l'activté principale): elle se compose d'une RecyclerView qui affiche 100 pokemon récupérés au travers de l'api via la librarie retrofit. Chaque élément chargé de l'api est affiché dans un encart (clickable)

- au click dans l'encart une information contenant l'id du pokemon correpondant à l'encart est envoyée via (intent) pour l'activité info et un deuxième appel http est fait pour récupérer le détail du pokemon (son poids, taille, une url vers une image)


### permssion requise

- Uniquement internet pour pouvoir faire des appel http (rest) vers l'api

### Librairies utilisées

- Glide (pour le chargement des images)
- Retrofit pour faire les appel http Rest
- Gson pour la déserialization du résultat des appel rest en objet 
 
#screenshot
![alt text](https://github.com/Dehbia20/pokemon-app/blob/master/screenshot%20PokemonApp/pokems.PNG?raw=true)
