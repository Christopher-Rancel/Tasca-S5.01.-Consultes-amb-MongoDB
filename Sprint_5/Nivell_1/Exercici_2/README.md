# Nivell 1 - Exercici 2

## Mostra'm tots els documents de les pel·lícules produïdes en 1932, però que el gènere sigui drama o estiguin en francès.

---

## Descripció

En aquest exercici s’ha realitzat una consulta sobre la col·lecció `movies` utilitzant MongoDB Compass.  
L’objectiu és obtenir les pel·lícules produïdes l’any 1932 que siguin del gènere drama o que estiguin en llengua francesa.

---

## Codi

```
Filter: {
  year: 1932,
  $or: [
    { genres: "Drama" },
    { languages: "French" }
  ]
}
```
