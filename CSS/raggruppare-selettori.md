I selettori CSS si possono raggruppare in 3 modi diversi:
## Lista separata da virgola
In questo modo si può risparmiare spazio sul file CSS raggruppando due o più selettori distinti che però condividono le stesse dichiarazioni di stile.

Esempio, da così:
```
.read {
  color: white;
  background-color: black;
  /* several unique declarations */
}

.unread {
  color: white;
  background-color: black;
  /* several unique declarations */
}
```

A così:
```
.read,
.unread {
  color: white;
  background-color: black;
}

.read {
  /* several unique declarations */
}

.unread {
  /* several unique declarations */
}
```

Entrambi i modi hanno lo stesso risultato, ma il secondo rende pià ordinato il file CSS e più facile apportare modifiche.

## Incatenare i selettori
In questo modo si può dire al file CSS di selezionare solamente gli elementi che hanno una classe E un'altra classe. Una specie di AND. Si possono incantenare anche classi e id, l'importante è che facciano parte dello stesso tag HTML (non si possono incatenare due classi che per es. una appartiene a un <div> e l'altra a un <p>). Per farlo si scrivono i selettori non separati da niente.

## 