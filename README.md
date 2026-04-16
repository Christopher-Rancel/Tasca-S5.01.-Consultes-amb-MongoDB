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
Crea una base de dades amb MongoDB utilitzant com a col·leccions els arxius adjunts.

### Exercici 1
Mostra els 2 primers comentaris que hi ha en la base de dades.  
Quants usuaris tenim registrats?  
Quants cinemes hi ha en l'estat de Califòrnia?  
Quin va ser el primer usuari/ària en registrar-se?  
Quantes pel·lícules de comèdia hi ha en la nostra base de dades?

### Exercici 2
Mostra'm tots els documents de les pel·lícules produïdes en 1932, però que el gènere sigui drama o estiguin en francès.

### Exercici 3
Mostra'm tots els documents de pel·lícules estatunidenques que tinguin entre 5 i 9 premis que van ser produïdes entre 2012 i 2014.

---

## Nivell 2

### Exercici 1
Compte quants comentaris escriu un usuari/ària que utilitza "GAMEOFTHRON.ES" com a domini de correu electrònic.

### Exercici 2
Quants cinemes hi ha en cada codi postal situats dins de l'estat Washington D. C. (DC)?

---

## Nivell 3

### Exercici 1
Troba totes les pel·lícules dirigides per John Landis amb una puntuació IMDb (Internet Movie Database) d'entre 7,5 i 8.

### Exercici 2
Mostra en un mapa la ubicació de tots els teatres de la base de dades.

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
