# Angular Cheat Sheet

<table>
    <h2>🪄 Comandos Básicos de Angular</h2>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">new</span> nombre-proyecto --[<span style="color: #FF0077">style=scss</span>] [<span style="color: #FF0077">routing</span>] [<span style="color: #FF0077">strict</span>]
    </td>
    <td><span style="color: #79c928ff">#</span> Crea un proyecto Angular nuevo. Routing agrega rutas, style indica el preprocesador CSS, strict define chequeo TS estricto</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">s</span> --[<span style="color: #FF0077">open</span>] [<span style="color: #FF0077">port {número}</span>] [<span style="color: #FF0077">watch</span>]</td>
    <td><span style="color: #79c928ff">#</span> Levanta servidor local. Open abre navegador, port cambia el puerto y watch recompila al guardar</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">s</span> --<span style="color: #FF0077">ssl</span> true --<span style="color: #FF0077">ssl</span>-cert [url del certificado] --<span style="color: #FF0077">ssl</span>-key [url de la llave]</td>
    <td><span style="color: #79c928ff">#</span> Levanta servidor local con cifrado SSL/TLS (https). Hay que indicar la url del certificado. Si no se le indica, usará uno autofirmado por Angular lo que generará alerta en el navegador de sitio no seguro y no es necesario usar --ssl-key.</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">s</span> --[<span style="color: #FF0077">host</span> 0.0.0.0] --[<span style="color: #FF0077">port</span> 4200]
    --<span style="color: #FF0077">ssl</span> false</td>
    <td><span style="color: #79c928ff">#</span> Levanta servidor local en http en vez de https</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">g</span> <span style="color: #FF0077">c</span> nombre-componente --[<span style="color: #FF0077">inline-style</span>] [<span style="color: #FF0077">inline-template</span>] [<span style="color: #FF0077">skip-tests</span>]</td>
    <td><span style="color: #79c928ff">#</span> Crea un componente</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">g</span> <span style="color: #FF0077">m</span> nombre-modulo --[<span style="color: #FF0077">routing</span>] [<span style="color: #FF0077">flat</span>]</td>
    <td><span style="color: #79c928ff">#</span> Crea un módulo. Flat lo hace sin carpeta extra</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">g</span> <span style="color: #FF0077">s</span> nombre-servicio --[<span style="color: #FF0077">skip-tests</span>]</td>
    <td><span style="color: #79c928ff">#</span> Crea un servicio</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">g</span> <span style="color: #FF0077">d</span> nombre-directiva</td>
    <td><span style="color: #79c928ff">#</span> Crea una directiva</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">g</span> <span style="color: #FF0077">p</span> nombre-pipe</td>
    <td><span style="color: #79c928ff">#</span> Crea un pipe (canalización)</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">build</span> --[<span style="color: #FF0077">prod</span>] [<span style="color: #FF0077">output-path=dist/carpeta</span>]</td>
    <td><span style="color: #79c928ff">#</span> Construye la app. Prod optimiza el resultado para producción</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">test</span> --[<span style="color: #FF0077">watch</span>]
    </td>
    <td><span style="color: #79c928ff">#</span> Ejecuta pruebas unitarias. Watch recompila al guardar</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">e2e</span></td>
    <td><span style="color: #79c928ff">#</span> Ejecuta pruebas end-to-end</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">lint</span> --[<span style="color: #FF0077">fix</span>]</td>
    <td><span style="color: #79c928ff">#</span> Revisa errores de código / estilo. Fix arregla automáticamente los problemas detectados</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">update</span> @[<span style="color: #FF0077">angular/cli</span>] @[<span style="color: #FF0077">angular/core</span>] --[<span style="color: #FF0077">next</span>]</td>
    <td><span style="color: #79c928ff">#</span> Actualiza Angular y su CLI. Next es para instalar la próxima versión disponible aunque no sea estable (beta o release candidate)</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">v</span></td>
    <td><span style="color: #79c928ff">#</span> Muestra versión de Angular, Node, CLI</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">ng</span> <span style="color: #00eeffff">help</span></td>
    <td><span style="color: #79c928ff">#</span> Muestra comandos del CLI</td>
  </tr>
</table>