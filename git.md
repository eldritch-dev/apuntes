# Git Cheat Sheet

<table>
    <h2>🪄 Inicialización y Configuración</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> --version</td>
    <td><span style="color: #79c928ff">#</span> Verificar si Git está instalado solicitando su versión</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> init</td>
    <td><span style="color: #79c928ff;">#</span> Inicializa un nuevo repositorio Git</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> clone &lt;repo-url&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Clona un repositorio desde una URL</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> config --global user.name "NombreDeUsuario"</td>
    <td><span style="color: #79c928ff;">#</span> Configura tu nombre de usuario</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> config --global user.email "email@dominio.com"</td>
    <td><span style="color: #79c928ff;">#</span> Configura tu email</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> config --global --list"</td>
    <td><span style="color: #79c928ff;">#</span> Revisa configuraciones globales</td>
  </tr>
</table>

<table>
    <h2>🛠️ Desarrollo Diario</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> status</td>
    <td><span style="color: #79c928ff">#</span> Muestra el estado de los cambios</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> add &lt;archivo&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Añade cambios de un archivo específico al área de preparación</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> add .</td>
    <td><span style="color: #79c928ff;">#</span> Añade todos los cambios al área de preparación</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> commit -m "Mensaje"</td>
    <td><span style="color: #79c928ff;">#</span> Confirma los cambios con un mensaje</td>
  </tr>
</table>

<table>
    <h2>🛠️ Gestión de Ramas</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> branch</td>
    <td><span style="color: #79c928ff">#</span> Lista las ramas del proyecto local</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> branch &lt;nombre-rama&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Crea una nueva rama</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> switch &lt;nombre-rama&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Cambia a una rama diferente</td>
  </tr>
</table>

<table>
    <h2>🛠️ Integración y Colaboración</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> merge &lt;rama-objetivo&gt;</td>
    <td><span style="color: #79c928ff">#</span> Fusiona los cambios desde la rama objetivo hacia la rama actual</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> remote add &lt;nombre&gt; &lt;url&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Añade un repositorio/proyecto remoto</td>
  </tr>
</table>

<table>
    <h2>🛠️ Recuperación y Limpieza</h2>
  <tr>
    <td><span style="color: #f8d910ff">git</span> fetch</td>
    <td><span style="color: #79c928ff">#</span> Indica si hay cambios en rama remota</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> reset --hard HEAD</td>
    <td><span style="color: #79c928ff;">#</span> Desecha todos los cambios locales</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">git</span> revert &lt;hash-commit&gt;</td>
    <td><span style="color: #79c928ff;">#</span> Revierte los cambios de un commit</td>
  </tr>
</table>



