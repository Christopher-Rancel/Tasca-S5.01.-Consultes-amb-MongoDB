# Nivell 3 - Exercici 2

## Mostra en un mapa la ubicació de tots els teatres de la base de dades.

---

## Descripció

En aquest exercici s’ha utilitzat MongoDB Compass per visualitzar la ubicació dels teatres de la base de dades.  
L’objectiu és representar les dades geogràfiques mitjançant un mapa utilitzant el camp de coordenades.

---

## Procés realitzat

S’ha accedit a la col·lecció `theaters` i s’ha utilitzat l’opció **Schema → Analyze Schema** de MongoDB Compass.

Posteriorment, s’ha seleccionat el camp `location.geo`, que conté les coordenades geogràfiques dels teatres.

MongoDB Compass ha detectat automàticament aquestes coordenades i ha mostrat la seva ubicació en un mapa.

---

## Resultat

Els teatres es mostren correctament en un mapa, on cada punt representa la ubicació d’un cinema segons les seves coordenades geogràfiques.
