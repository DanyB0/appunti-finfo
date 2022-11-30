# allocazione dinamica della memoria

- ### libreria:
```c
#include <stdlib.h>
```
- ### comandi:
  - allocazione memoria
  ```c
  void * malloc(size_t);
  ```
  - deallocazione memoria
  ```c
  free(malloc(size_t));
  ```
- ### parametri:
  - **syze_t** --> quanto spazio serve
  ```c
  sizeof(int, char, float...)
  ```
- ### schema base:
```c
var = malloc(size_t)

if (var){
    /* codice */
    free(var);
}
else
    printf("errore di allocazione\n");
```
- ### note:
  - se la memoria non viene allocata perchè non c'è spazio ` malloc(size_t)` restituisce `NULL`, quindi come prima cosa si deve controllare che `malloc` non abbia restituito `NULL`, altrimenti poi il programma andrà in crash
  - se restituisco qualcosa contentuto nella memoria allocata non devo fare `free`, alrimenti andrà perso

- ### esempio:
  - [click here](https://pastebin.com/raw/kQ2cHmGs)
