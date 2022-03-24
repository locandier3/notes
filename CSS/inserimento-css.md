## CSS esterno
Bisogna creare separatamente un file CSS da linkare nella pagina HTML, all'interno di `<head>` in un elemento chiamato `<link>`

```
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```
L'elemento `href` è la posizione del file CSS relativo alla pagina HTML, l'elemento `rel` è richiesto e specifica la relazione tra file HTML e CSS.

## CSS interno
Basta inserire tutte le regole all'interno del file HTML, tra due tag `<style>` (apertura e chiusura), a sua volta all'interno di `<head>`
Sintassi uguale al metodo esterno, può essere utile per modificare singolarmente lo stile di alcune pagine di un sito web.

## CSS inline
All'interno dei tag HTML si inserisce l'elemento `<style>`

Es.
```
<body>
  <div style="color: white; background-color: black;">...</div>
</body>
``` 
Gli attributi sono identici. NB CSS inline fa override di tutti gli altri stili.