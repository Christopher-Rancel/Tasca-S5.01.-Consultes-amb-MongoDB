# Tasca-S5.01.-Consultes-amb-MongoDB

## Descripció

En aquest sprint es treballa la realització de consultes sobre bases de dades NoSQL utilitzant MongoDB.

L’activitat consisteix en explorar diferents col·leccions, aplicar filtres, utilitzar operadors i realitzar consultes per extreure informació rellevant a partir de les dades.

Es treballa amb una base de dades relacionada amb una aplicació d’entreteniment cinematogràfic.

---

## Estructura de la base de dades

El projecte treballa amb les següents col·leccions:

- `users` → informació d’usuaris (nom, email i contrasenya)  
- `theaters` → informació de cinemes (ubicació i coordenades geogràfiques)  
- `sessions` → sessions d’usuari i autenticació  
- `movies` → informació de pel·lícules (gèneres, any, directors, puntuacions i premis)  
- `comments` → comentaris d’usuaris sobre pel·lícules  

Les col·leccions es relacionen mitjançant identificadors com `user_id` i `movie_id`.

---

## Nivell 1

### Exercici 0
Creació de la base de dades i importació de les col·leccions a partir dels arxius JSON proporcionats.

### Exercici 1
Realització de consultes bàsiques per obtenir informació general de la base de dades:

- Mostra dels primers comentaris  
- Comptatge d’usuaris  
- Filtrat de cinemes per estat  
- Obtenció del primer usuari registrat  
- Filtrat de pel·lícules per gènere  

### Exercici 2
Consulta de pel·lícules produïdes en 1932 amb condicions sobre el gènere i la llengua.

### Exercici 3
Consulta de pel·lícules dels Estats Units amb un rang de premis i produïdes dins d’un interval d’anys.

---

## Nivell 2

### Exercici 1
Comptatge de comentaris realitzats per usuaris amb un domini de correu electrònic específic.

### Exercici 2
Anàlisi dels cinemes agrupats per codi postal dins de l’estat Washington D.C. utilitzant agregacions.

---

## Nivell 3

### Exercici 1
Filtrat de pel·lícules segons director i puntuació IMDb dins d’un rang determinat.

### Exercici 2
Visualització de la ubicació dels teatres en un mapa utilitzant dades geogràfiques.

---

## Objectiu del projecte

L’objectiu d’aquesta activitat és consolidar els coneixements sobre consultes en MongoDB, incloent:

- Consultes bàsiques (`find`)  
- Ús d’operadors (`$gte`, `$lte`, `$or`)  
- Treball amb arrays i camps anidats  
- Comptatge de documents  
- Aggregations (`$match`, `$group`)  
- Ús d’expressions regulars  
- Visualització de dades geogràfiques  

Aquest projecte forma part del procés d’aprenentatge en bases de dades NoSQL i anàlisi de dades.
