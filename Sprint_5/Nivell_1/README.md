# Nivell 1 - Exercici 1

## Mostra els 2 primers comentaris que hi ha en la base de dades.  
## Quants usuaris tenim registrats?  
## Quants cinemes hi ha en l'estat de Califòrnia?  
## Quin va ser el primer usuari/ària en registrar-se?  
## Quantes pel·lícules de comèdia hi ha en la nostra base de dades?

---

## Descripció

En aquest exercici s’han realitzat diverses consultes bàsiques utilitzant MongoDB Compass.  
L’objectiu és consultar dades, aplicar filtres simples i obtenir informació rellevant de les diferents col·leccions.

---

## Consultes realitzades

### 1. Primers 2 comentaris

S’ha accedit a la col·lecció `comments` i s’han mostrat els dos primers documents utilitzant el límit de resultats.

---

### 2. Nombre total d’usuaris

S’ha accedit a la col·lecció `users` i s’ha obtingut el nombre total de documents mostrats a la part superior de MongoDB Compass.

---

### 3. Cinemes a Califòrnia

S’ha filtrat la col·lecció `theaters` per obtenir els cinemes situats a l’estat de Califòrnia (`CA`).

---

### 4. Primer usuari registrat

S’ha ordenat la col·lecció `users` pel camp `_id` en ordre ascendent i s’ha limitat el resultat a un únic document per obtenir el primer usuari registrat.

---

### 5. Pel·lícules de comèdia

S’ha filtrat la col·lecció `movies` per mostrar les pel·lícules que contenen el gènere `Comedy`.

---

## Codi (MongoDB Compass)

```json
// 1. Primers 2 comentaris (Filter)
{}

// Limit: 2

// 2. Nombre total d’usuaris
// Es consulta la col·lecció `users` i es mostra el total a la part superior (Documents)

// 3. Cinemes a Califòrnia
{
  "location.address.state": "CA"
}

// 4. Ordenació i límit
Sort: { _id: 1 }
Limit: 1

// 5. Pel·lícules de comèdia
{ genres: "Comedy" }
