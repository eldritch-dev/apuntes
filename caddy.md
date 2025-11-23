Desde CMD - Windows:
Cargar archivo de configuración: curl -X POST localhost:2019/load -H "Content-Type: application/json" -d "@caddy.json"

ESTO FUNCIONÓ CORRECTAMENTE CON CADDYFILE. JSON NO FUNCIONÓ NUNCA

Archivo de configuración *.json nunca me funcionó.
Lo que sí me funcionó fue usar un Caddyfile (sin extensión).

Desde Símbolo del Sistema (CMD), porque desde otra terminal no me ha logrado funcionar:

"caddy start" usa ese archivo y arranca caddy.
"caddy stop" detiene caddy.

"tasklist | find "caddy" sirve para revisar que caddy no siga corriendo a pesar de caddy stop.
"taskkill /IM caddy.exe /F" mata el proceso caddy si no pudimos detenerlo con caddy stop.
