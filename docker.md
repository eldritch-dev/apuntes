# Docker Cheat Sheet

<table>
    <h2>🪄 Trabajo Diario</h2>
  <tr>
    <td><span style="color: #f8d910ff">docker-compose</span> <span style="color: #00eeffff">up</span> -<span style="color: #FF0077">d</span></td>
    <td><span style="color: #79c928ff">#</span> Crea y ejecuta el contenedor configurado en el archivo docker-compose</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">docker</span> <span style="color: #00eeffff">ps</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Verifica todos los contenedores que están ejecutándose</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">docker-compose</span> <span style="color: #00eeffff">down</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Detiene y elimina el contenedor configurado en el archivo docker-compose que está ejecutándose</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">docker</span> <span style="color: #00eeffff">stop</span> [nombre-del-contenedor]
    </td>
    <td><span style="color: #79c928ff">#</span> Detiene el contenedor indicado sin eliminarlo</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">docker</span> <span style="color: #00eeffff">start</span> [nombre-del-contenedor]
    </td>
    <td><span style="color: #79c928ff">#</span> Inicia el contenedor iniciado</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">docker-compose</span> <span style="color: #00eeffff">down</span> -<span style="color: #FF0077">v</span></td>
    <td><span style="color: #79c928ff">#</span> Elimina el volumen asociado al contenedor configurado en el archivo docker-compose</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">docker</span> <span style="color: #00eeffff">logs</span> -<span style="color: #FF0077">f</span> [nombre-del-contenedor]</td>
    <td><span style="color: #79c928ff">#</span> Muestra los logs del contenedor indicado en vivo</td>
  </tr>
</table>

## Definiciones
- Imagen: archivo inmutable que tiene todo lo necesario para ejecutar una app (OS, binarios, dependencias, etc).
- Contenedor: instancia en ejecución de una imagen. Es un proceso en ejecución basado en una imagen. Tiene sus propios puertos y sistema de archivos. Se puede iniciar, detener, reiniciar y eliminar. Por defecto sus datos son volátiles.
- Volúmen: espacio de almacenamiento persistente gestionado por docker que existe fuera del contenedor. Se puede conectar un volumen a uno o más contenedores.
