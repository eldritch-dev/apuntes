# RxJs Cheat Sheet

<table>
  <tr>
    <td><span style="color: #f8d910ff">Observable</span>()
    </td>
    <td><span style="color: #79c928ff">#</span> Fuente de datos que emite valores con el tiempo</td>
    <td><span style="color: #79c928ff">#</span> Para recibirlos es necesario suscribirse al Observable</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">pipe</span>()
    </td>
    <td><span style="color: #79c928ff">#</span> Función utilitaria de RxJs que recibe operadores y los aplica secuencialmente al flujo de datos</td>
    <td><span style="color: #79c928ff">#</span> Mecanismo de composición de operadores. Organiza cómo estos se aplican</td>
  </tr>
  <tr>
    <td>Operadores</td>
    <td><span style="color: #79c928ff">#</span> Funciones que transforman el flujo de datos. Existen 2 tipos:</td>
    <td><span style="color: #79c928ff">#</span> ...pipe(operator) y ...pipe(operatorFactory()) </td>
  </tr>
</table>

<Table>
<h2>🪄 Algunos Operadores</h2>
  <tr>
    <td><span style="color: #f8d910ff">debounceTime</span>(<span style="color: #FF0077">dueTime</span>, scheduler)</td>
    <td><span style="color: #79c928ff">#</span> Retrasa la emisión que el Observable hace hasta que hayan pasado <span style="color: #FF0077">x</span> ms sin que llegue un nuevo valor</td>
    <td><span style="color: #79c928ff">#</span> Sólo emite el último valor del período de silencio. dueTime es tiempo en ms y scheduler por defecto si omitido es asyncScheduler</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">switchMap(project => 0, resultSelector? => R)</span></td>
    <td><span style="color: #79c928ff">#</span> Proyecta cada valor emitido por el Observable fuente a un Observable interno, reemitiendo en el Observable resultante únicamente los valores provenientes del último Observable interno creado, cancelando cualquier suscripción interna previa.</td>
    <td><span style="color: #79c928ff">#</span> Sólo emite el último valor del período de silencio. dueTime es tiempo en ms y scheduler por defecto si omitido es asyncScheduler</td>
  </tr>
</table>

## RxJs
- RxJs es una librería para trabajar con Observables y flujos de datos asíncronos.

## Ejemplos
### DebounceTime con SwitchMap
this.searchControl.valueChanges
  .pipe(
    debounceTime(300),
    switchMap((query: string) => query.length > 0
      ? this.service.getSuggestions(query).pipe(catchError(() => of([]))) : of([])
    )
  )
  .subscribe((res: CharacterSuggestionDto[]) => {
    this.suggestions.set(res)
  }
);

valueChanges observa un control de input y emite sus valores.
debounceTime(300) espera 300ms de silencio y emite únicamente el último valor (el estado actual del Input).
switchMap() proyecta ese valor (query) a getSuggestions(query).
Si query está vacío, como si ocurre un error con el resultado de getSuggestions(query), se retorna un arreglo vacío of([]). En caso contrario el resultante es un Observable con datos válidos, los que son asignados a this.suggestions mediante una suscripción.