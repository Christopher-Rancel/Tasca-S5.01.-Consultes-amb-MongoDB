# Nivell 2 - Exercici 2

## Quants cinemes hi ha en cada codi postal situats dins de l'estat Washington D. C. (DC)?

---

## Descripció

En aquest exercici s’ha utilitzat MongoDB Compass per analitzar la col·lecció `theaters`.  
L’objectiu és obtenir el nombre de cinemes agrupats per codi postal dins de l’estat Washington D.C. (`DC`).

Per fer-ho, s’ha utilitzat una agregació amb dues etapes: filtratge i agrupació.

---

## Codi (Aggregation)

```
Stage 1 ($match):
{ "location.address.state": "DC" }

Stage 2 ($group):
{
  _id: "$location.address.zipcode",
  total: { $sum: 1 }
}
```

---

## Resultat

S’obté una llista de codis postals amb el nombre de cinemes corresponent a cada un d’ells.
