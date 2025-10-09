# Git Cheat Sheet

<table>
    <h2>🪄 Inicialización y Configuración</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> --<span style="color: #00eeffff">version</span></td>
    <td><span style="color: #79c928ff">#</span> Verificar si Git está instalado solicitando su versión</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">init</span></td>
    <td><span style="color: #79c928ff;">#</span> Inicializa un nuevo repositorio Git</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">clone</span> [repo-url]</td>
    <td><span style="color: #79c928ff;">#</span> Clona un repositorio desde una URL</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">config</span> --<span style="color: #FF0077">global</span> user.name "NombreDeUsuario"</td>
    <td><span style="color: #79c928ff;">#</span> Configura tu nombre de usuario</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">config</span> --<span style="color: #FF0077">global</span> user.email "email@dominio.com"</td>
    <td><span style="color: #79c928ff;">#</span> Configura tu email</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">config</span> --<span style="color: #FF0077">global</span> --<span style="color: #FF0077">list</span>"</td>
    <td><span style="color: #79c928ff;">#</span> Revisa configuraciones globales</td>
  </tr>
</table>

<table>
    <h2>🛠️ Desarrollo Diario</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">status</span></td>
    <td><span style="color: #79c928ff">#</span> Muestra el estado de los cambios</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">add</span> [archivo]</td>
    <td><span style="color: #79c928ff;">#</span> Añade cambios de un archivo específico al área de preparación</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">add</span> .</td>
    <td><span style="color: #79c928ff;">#</span> Añade todos los cambios al área de preparación</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">diff</span> [archivo]</td>
    <td><span style="color: #79c928ff;">#</span> Muestra los cambios entre el archivo local y el área de preparación</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">diff</span> --<span style="color: #FF0077">staged</span></td>
    <td><span style="color: #79c928ff;">#</span> Muestra los cambios añadidos al área de preparación</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">checkout</span> -- [archivo]</td>
    <td><span style="color: #79c928ff;">#</span> Descarta los cambios en el archivo local. Irrecuperable</td>
  </tr>
  <tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">commit</span> -<span style="color: #FF0077">m</span> "Mensaje"</td>
    <td><span style="color: #79c928ff;">#</span> Confirma los cambios con un mensaje</td>
  </tr>
</table>

<table>
    <h2>🛠️ Gestión de Ramas</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">branch</span> [-<span style="color: #FF0077">a</span>]</td>
    <td><span style="color: #79c928ff">#</span> Lista las ramas del proyecto local. Con -a muestra también las ramas remotas</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">branch</span> [nombre-rama]</td>
    <td><span style="color: #79c928ff;">#</span> Crea una nueva rama</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">switch</span> [nombre-rama]</td>
    <td><span style="color: #79c928ff;">#</span> Cambia a una rama diferente</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">branch</span> [-<span style="color: #FF0077">d</span>] | [-<span style="color: #FF0077">D</span>] [nombre-rama]</td>
    <td><span style="color: #79c928ff;">#</span> Elimina la rama. Con -D fuerza la eliminación</td>
  </tr>
</table>

<table>
    <h2>🛠️ Integración y Colaboración</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">merge</span> [rama-objetivo]</td>
    <td><span style="color: #79c928ff">#</span> Fusiona los cambios desde la rama objetivo hacia la rama actual</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">rebase</span> [rama-objetivo]</td>
    <td><span style="color: #79c928ff;">#</span> Aplica el último estado de la rama objetivo a la rama actual REVISAR</td>
  </tr>
</table>

<table>
    <h2>🛠️ Recuperación, Sincronización y Limpieza</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">fetch</span></td>
    <td><span style="color: #79c928ff">#</span> Indica si hay cambios en rama remota</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">fetch </span>-<span style="color: #FF0077">p</span> [remote]</td>
    <td><span style="color: #79c928ff">#</span> Elimina las referencias remotas que han sido eliminadas del repositorio remoto (-p / --prune)</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">pull</span> [remote]</td>
    <td><span style="color: #79c928ff">#</span> Descarga los cambios de la rama remota, que no están en la rama local actual</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">push</span> -<span style="color: #FF0077">u</span> [remote] [branch]</td>
    <td><span style="color: #79c928ff">#</span> Sube la rama local al repositorio remoto</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">remote</span> -<span style="color: #FF0077">v</span></td>
    <td><span style="color: #79c928ff">#</span> Muestra repositorios remotos</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">remote</span> <span style="color: #FF0077">add</span> origin [url]</td>
    <td><span style="color: #79c928ff;">#</span> Añade un repositorio/proyecto remoto</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">branch</span> --<span style="color: #FF0077">unset-upstream</span></td>
    <td><span style="color: #79c928ff">#</span> Elimina la conexión de seguimiento existente con de la rama remota REVISAR</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">branch</span> -<span style="color: #FF0077">u</span> origin/nombre-de-la-rama</td>
    <td><span style="color: #79c928ff">#</span> Crea una nueva conexión de seguimiento con la rama especificada</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">reset</span> --<span style="color: #FF0077">hard</span> HEAD</td>
    <td><span style="color: #79c928ff;">#</span> Desecha todos los cambios locales</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">revert</span> [hash-commit]</td>
    <td><span style="color: #79c928ff;">#</span> Crea un commit nuevo, revertiendo los cambios del commit especificado. Genera una inversión de los cambios</td>
  </tr>
</table>

<table>
    <h2>🛠️ Reservas</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">stash</span> <span style="color: #FF0077">list</span></td>
    <td><span style="color: #79c928ff">#</span> Lista las reservas guardadas </td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">stash</span></td>
    <td><span style="color: #79c928ff;">#</span> Crea una reserva</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">stash</span> <span style="color: #FF0077">pop</span></td>
    <td><span style="color: #79c928ff;">#</span> Elimina última reserva y la aplica al código en el que se está trabajando</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">stash</span> <span style="color: #FF0077">drop</span></td>
    <td><span style="color: #79c928ff;">#</span> Elimina una reserva específica</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">apply</span> 'stash@{n}'</td>
    <td><span style="color: #79c928ff;">#</span> Aplica una reserva específica al código en el que se está trabajando</td>
  </tr>
</table>

<table>
    <h2>🛠️ Inspeccionar Historia</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">log</span> [-<span style="color: #FF0077">n</span> count]</td>
    <td><span style="color: #79c928ff">#</span> Lista la historia de commits de la rama actual. <b>-n count</b> limita la lista a los últimos <b>n</b> commits</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">log</span> --<span style="color: #FF0077">oneline</span> --<span style="color: #FF0077">graph</span></td>
    <td><span style="color: #79c928ff">#</span> Lista la historia de commits de manera compacta y gráfica</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">show</span> [<span style="color: #FF0077">commit</span> ]</td>
    <td><span style="color: #79c928ff">#</span>Muestra los detalles de un commit</td>
  </tr>
</table>

<table>
    <h2>🛠️ Commits de Tag</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">tag</span></td>
    <td><span style="color: #79c928ff">#</span> Lista todos los tags</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">tag</span> [nombre] [commit sha]</td>
    <td><span style="color: #79c928ff">#</span> Crea un tag de referencia para el commit actual. <b>commit sha</b> permite crear el tag sobre un commit específico en vez del actual</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">tag</span> -<span style="color: #FF0077">d</span> [nombre]</td>
    <td><span style="color: #79c928ff">#</span> Elimina un tag del repositorio local</td>
  </tr>
</table>

## Definiciones
- git: sistema de control de versiones de código abierto
- commit: un objeto Git, una instantánea de tu repositorio
- branch: un puntero movible y ligero hacia un commit. Una rama
- clone: una versión local de un repositorio, incluyendo todos sus commits y ramas
- remote: un repositorio común en GitHub que todos los miembros del equipo usan para intercambiar sus cambios
- pull request: solicitud para comparar y discutir las diferencias introducidas a una rama, con revisiones, comentarios, tests integrados y más
- tag: un estandar o un objeto anotado
- HEAD: representa tu directorio de trabajo actual. Es un puntero que puede moverse a ramas diferentes, tags o commits usando git checkout.

## Buenas Prácticas para un Commit
- Limita el asunto a 50 caracteres
- Solo la primera letra del asunto debe tener mayúscula
- No termines la linea del asunto con un punto
- Separa el asunto del cuerpo con una linea en blanco
- El cuerpo debe tener 72 caracteres como máximo
- En el asunto, usa el modo imperativo: "(This commit will) Add nationality column to AddDataToUser table"
- Usa el cuerpo para explicar el "qué" y el "por qué" en vez de explicar el "cómo"



