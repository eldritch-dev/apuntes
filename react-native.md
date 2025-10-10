# React Native Cheat Sheet
## Expo: Framework para desarrollo movil

<table>
  <h2>🪄 Inicialización React Native con Expo</h2>
  <tr>
    <td><span style="color: #f8d910ff">npx</span> <span style="color: #00eeffff">create</span>-<span style="color: #00eeffff">expo</span>-<span style="color: #00eeffff">app@latest</span></td>
    <td><span style="color: #79c928ff">#</span> Crea un nuevo projecto Expo</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">npx</span> <span style="color: #00eeffff">expo</span> <span style="color: #FF0077">start</span></td>
    <td><span style="color: #79c928ff">#</span> Inicia el servidor de desarrollo</td>
  </tr>
  <tr>
    <td></td>
    <td><span style="color: #79c928ff">#</span> Luego de iniciar el servidor, verás un QR en la terminal. Escanéalo para abrir la app en tu dispositivo móvil</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">npm</span> <span style="color: #00eeffff">run</span> <span style="color: #FF0077">reset</span>-<span style="color: #FF0077">project</span></td>
    <td><span style="color: #79c928ff">#</span> Resetea el proyecto. Elimina el código prediseñado (boilerplate) para comenzar de cero</td>
  </tr>
</table>

<table>
  <h2>🪄 Comandos de uso típico</h2>
  <tr>
    <td><span style="color: #f8d910ff">npx</span> <span style="color: #00eeffff">expo</span> <span style="color: #FF0077">prebuild</span></td>
    <td><span style="color: #79c928ff">#</span> Genera directorios Android e iOS nativos usando Prebuild</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">npx</span> <span style="color: #00eeffff">expo</span> <span style="color: #FF0077">run</span>:android</td>
    <td><span style="color: #79c928ff">#</span> Compila una app nativa de Android localmente</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">npx</span> <span style="color: #00eeffff">expo</span> <span style="color: #FF0077">run</span>:ios</td>
    <td><span style="color: #79c928ff">#</span> Compila una app nativa de iOS localmente</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">npx</span> <span style="color: #00eeffff">expo</span> <span style="color: #FF0077">install</span> nombre-del-paquete</td> --[<span style="color: #FF0077">fix</span>]
    <td><span style="color: #79c928ff">#</span> Instala una nueva librería o valida y actualiza librerías específicas en el proyecto añadiendo la opción fix</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">npx</span> <span style="color: #00eeffff">expo</span> <span style="color: #FF0077">lint</span></td>
    <td><span style="color: #79c928ff">#</span> Configura ESlint. Si ya está configurado, linteará tu proyecto (revisará el proyecto para encontrar errores de sintaxis, inconsistencias o malas prácticas de estilo</td>
  </tr>
</table>
