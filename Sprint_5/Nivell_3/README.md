# Nivell 3 - Exercici 1

## Troba totes les pel·lícules dirigides per John Landis amb una puntuació IMDb (Internet Movie Database) d'entre 7,5 i 8.

---

## Descripció

En aquest exercici s’ha realitzat una consulta sobre la col·lecció `movies` utilitzant MongoDB Compass.  
L’objectiu és obtenir les pel·lícules dirigides per John Landis que tinguin una puntuació IMDb compresa entre 7,5 i 8.

---

## Codi

```
Filter: {
  directors: "John Landis",
  "imdb.rating": { $gte: 7.5, $lte: 8 }
}
```

---

## Resultat

S’obtenen totes les pel·lícules que compleixen les condicions indicades.
