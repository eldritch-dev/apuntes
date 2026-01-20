# Flask Cheat Sheet

<table>
  <h2>🪄 Comandos Básicos de Flask</h2>
  <tr>
    <td><span style="color: #f8d910ff">flask</span> run --<span style="color: #00eeffff">debug</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Levanta la aplicación en modo hot reload</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">flask</span> db <span style="color: #00eeffff">init</span></td>
    <td><span style="color: #79c928ff">#</span> Crea directorio migrations</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">flask</span> db <span style="color: #00eeffff">migrate</span>
      <span style="color: #FF0077">-m</span> "create users table (nombre migración)"
    </td>
    <td><span style="color: #79c928ff">#</span> Crea migración</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">flask</span> db <span style="color: #00eeffff">upgrade</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Actualiza base de datos</td>
  </tr>
</table>

## Consideraciones
- Para que Migrate detecte los modelos, deben ser importados en app.py.

## Buenas prácticas reales
- Crear un entorno virtual por cada proyecto, incluso si es chico.
- Usar 'requirements.txt' en los repositorios para que otros puedan ejecutarlo.
- Versionar los archivos de entorno (pero no los archivos internos de venv)
- Activar siempre el entorno virtual antes de ejecutar el script.

## Errores comunes
- Instalar todo globalmente y después perder control de versiones.
- No saber qué versión de librería se está usando realmente.
- Romper un proyecto al actualizar algo para otro. Por eso todas las dependencias van aisladas en el entorno virtual.