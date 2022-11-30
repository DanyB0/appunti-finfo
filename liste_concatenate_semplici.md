# liste concatenate semplici

## scopo:
  - permette di allocare memeoria dinamicamente (array dinamici)
  
## dichiarazione:
```c
ilist_t * h = NULL;
```
  - `* h = NULL` è l'indirizzo in memeoria della variabile `h` a cui è stato assegnato il valore `NULL`

## comandi:
- **append** --> aggiunge in coda alla lista
  - ```c
    ilist_t * append(ilist_t *, int);
    ```
- **push** --> aggiunge in testa alla lista
  - ```c
    ilist_t * push(ilist_t *, int);
    ```
- **freelist** --> libera la memoria contenente la lista
   - ```c
   	 freelist(h);
     ```
- **...**
- ### parametri:
  - `ilist_t *` = indirizzo della lista da aggiornare
  - `int` = dato da aggiungere alla lista
  - `h` = la testa della lista la liberare

## note:
  - l'ultimo elemento dell'array deve avere il riferimento al nuovo elemento dell'array
  - si deve creare una `sruct` per definirla
   
## esempio:
  - [clicca qui](https://pastebin.com/raw/9QGwhAdU)
