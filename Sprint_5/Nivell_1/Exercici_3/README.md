# Nivell 1 - Exercici 3

## Mostra'm tots els documents de pel·lícules estatunidenques que tinguin entre 5 i 9 premis que van ser produïdes entre 2012 i 2014.

---

## Descripció

En aquest exercici s’ha realitzat una consulta sobre la col·lecció `movies` utilitzant MongoDB Compass.  
L’objectiu és obtenir les pel·lícules dels Estats Units que tenen entre 5 i 9 premis i que han estat produïdes entre els anys 2012 i 2014.

---

## Codi (MongoDB Compass)

```
Filter: {
  countries: "USA",
  "awards.wins": { $gte: 5, $lte: 9 },
  year: { $gte: 2012, $lte: 2014 }
}
```
