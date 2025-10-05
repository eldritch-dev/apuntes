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
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">clone</span> &lt;repo-url&gt;</td>
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
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">add</span> &lt;archivo&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Añade cambios de un archivo específico al área de preparación</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">add</span> .</td>
    <td><span style="color: #79c928ff;">#</span> Añade todos los cambios al área de preparación</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">commit</span> -<span style="color: #FF0077">m</span> "Mensaje"</td>
    <td><span style="color: #79c928ff;">#</span> Confirma los cambios con un mensaje</td>
  </tr>
</table>

<table>
    <h2>🛠️ Gestión de Ramas</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">branch</span></td>
    <td><span style="color: #79c928ff">#</span> Lista las ramas del proyecto local</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">branch</span> &lt;nombre-rama&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Crea una nueva rama</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">switch</span> &lt;nombre-rama&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Cambia a una rama diferente</td>
  </tr>
</table>

<table>
    <h2>🛠️ Integración y Colaboración</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">merge</span> &lt;rama-objetivo&gt;</td>
    <td><span style="color: #79c928ff">#</span> Fusiona los cambios desde la rama objetivo hacia la rama actual</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">remote</span> <span style="color: #FF0077">add</span> &lt;nombre&gt; &lt;url&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Añade un repositorio/proyecto remoto</td>
  </tr>
</table>

<table>
    <h2>🛠️ Recuperación y Limpieza</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">fetch</span></td>
    <td><span style="color: #79c928ff">#</span> Indica si hay cambios en rama remota</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">reset</span> --<span style="color: #FF0077">hard</span> HEAD</td>
    <td><span style="color: #79c928ff;">#</span> Desecha todos los cambios locales</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">revert</span> &lt;hash-commit&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Revierte los cambios de un commit</td>
  </tr>
</table>

<table>
    <h2>🛠️ Reservar Cambios para Más Tarde</h2>
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
    <td><span style="color: #f8d910ff">git</span> <span style="color: #00eeffff">apply</span> 'stash@{n}'</td>
    <td><span style="color: #79c928ff;">#</span> Aplica una reserva específica al código en el que se está trabajando</td>
  </tr>
</table>



