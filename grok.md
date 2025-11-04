Hay que setear el token de autenticación de mi usuario en ngrok.

setx NGROK_CONFIG "C:\Users\Javier\AppData\Local\ngrok.yml" - setea el archivo de configuración, que debe haber sido creado en la ruta entregada.

<table>
  <h2>🪄 Comandos Esenciales</h2>
  <tr>
    <td><span style="color: #f8d910ff">ngrok</span> http <span style="color: #00eeffff">8080</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Expone públicamente https://localhost:8080 a través de un endpoint de ngrok correspondiente a mi usuario en ngrok. Lo que hace es leer la configuración del Caddyfile. En el caso con el que inicié mi uso de ngrok, hace 2 reverse proxies de 2 URLs definidas allí. Redirige a esas 2 URLs con los path definidos a quienes entren a localhost:8080 a través del endpoint de ngrok.</td>
  </tr>
</table>