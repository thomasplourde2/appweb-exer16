---
outline: deep
---
# Revue de code

## Le code

- Les noms des **composants** sont trop vague et n'en disent pas assez sur leur utilités
- Pas de **commentaire** pour expliquer ou donner la source qui a aidé pour le code
- La gestion des **erreurs** n'est pas couvert à 100%
- Le nommage des **fonctions** n'est pas très significatif
- L'**Indentation** du code qui n'est pas conforme partout

  ````md
  ```const vinyls = ref
  {id:1, name:"In Utero", bandName:"Nirvana", releaseYear:1993, price:"39,99", quantity:6},
  {id:2, name:"Sister", bandName:"Sonic Youth", releaseYear:1987, price:"34,99", quantity:2},
  {id:3, name:"Where You Been", bandName:"Dinosaur Jr.", releaseYear:1993, price:"59,99", quantity:3},
  {id:4, name:"Superfuzz Bigmuff", bandName:"Mudhoney", releaseYear:1988, price:"31,99", quantity:1},
  {id:5, name:"Ten", bandName:"Pearl Jam", releaseYear:1991, price:"36,99", quantity:5},
  {id:6, name:"Amnesiac", bandName:"Radiohead", releaseYear:2001, price:"47,99", quantity:2},
  {id:7, name:"Mellon Collie And The Infinite Sadness", bandName:"The Smashing Pumpkins", releaseYear:1995, price:"74,99", quantity:1},
  {id:8, name:"Sweet Oblivion", bandName:"Screaming Trees", releaseYear:1992, price:"27,99", quantity:2},
  {id:9, name:"Live Through This", bandName:"Hole", releaseYear:1993, price:"42,99", quantity:4},
  {id:10, name:"Loveless", bandName:"My Bloody Valentine", releaseYear:1991, price:"41,99", quantity:3}
  ])
  const actionClickAdd = (vinylName:string, bandName:string, releaseYear:number, price:string) => {
  const newVinyl: Vinyl = {
  id: vinyls.value.length + 1,
  name: vinylName,
  bandName: bandName,
  releaseYear: releaseYear,
  price: price,
  quantity: + 1
  }
  vinyls.value.push(newVinyl);
  showVinylAddForm.value = false
  }
  ```
  ````

## Autres

- La validation des formulaires n'est pas optimale et a quelques brèches
- Des fonctionnalités sont manquantes
- Le manager contient beaucoup de code est peu être réduit

Voici la source pour voir comment faire une revue de code [Bonnes pratiques de revue de code](https://appweb.progwmj.ca/documentations/bonnes-pratiques/revue-code)
