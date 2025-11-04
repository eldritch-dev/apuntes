# Python Cheat Sheet

<table>
  <h2>🪄 Comandos Básicos de Python</h2>
  <tr>
    <td><span style="color: #f8d910ff">python</span> --<span style="color: #00eeffff">version</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Muestra la versión actual de Python instalada</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">python</span> <span style="color: #00eeffff">freeze</span></td>
    <td><span style="color: #79c928ff">#</span> Entra al intérprete interactivo de Python</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">python</span> <span style="color: #00eeffff">script.py</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Ejecuta el archivo script.py</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">python</span> <span style="color: #00eeffff">app.py</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Ejecuta el proyecto</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">python</span> -<span style="color: #00eeffff">m</span> unittest
    </td>
    <td><span style="color: #79c928ff">#</span> Ejecuta los tests definidos con unittest</td>
  </tr>
</table>

<table>
    <h2>🪄 Comandos del Gestor de Dependencias Pip de Python</h2>
  <tr>
    <td><span style="color: #f8d910ff">pip</span> <span style="color: #00eeffff">list</span> | <span style="color: #00eeffff">freeze</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Muestra todas las dependencias del proyecto y sus versiones actuales. List las muestra en formato 'humano' y freeze en formato para exportar y reinstalar</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">pip</span> <span style="color: #00eeffff">freeze</span> > <span style="color: #FF0077">requirements.txt</span></td>
    <td><span style="color: #79c928ff">#</span> Guarda todas las dependencias del proyecto en un archivo requirements.txt</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">pip</span> <span style="color: #00eeffff">install</span> -<span style="color: #FF0077">r</span> requirements.txt
    </td>
    <td><span style="color: #79c928ff">#</span> Instala todas las dependencias de mi proyecto que están listadas en el archivo requirements.txt. Sirve para cuando el proyecto es clonado en un equipo nuevo</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">pip</span> <span style="color: #00eeffff">install</span> paquete
    </td>
    <td><span style="color: #79c928ff">#</span> Instala paquete en el proyecto</td>
  </tr>
    <td><span style="color: #f8d910ff">pip</span> <span style="color: #00eeffff">install</span> paquete==1.2.3
    </td>
    <td><span style="color: #79c928ff">#</span> Instala versión específica del paquete</td>
  </tr>
  </tr>
    <td><span style="color: #f8d910ff">pip</span> <span style="color: #00eeffff">install</span> --<span style="color: #FF0077">upgrade</span> paquete
    </td>
    <td><span style="color: #79c928ff">#</span> Actualiza un paquete en su última versión</td>
  </tr>
  </tr>
    <td><span style="color: #f8d910ff">pip</span> <span style="color: #00eeffff">uninstall</span> paquete
    </td>
    <td><span style="color: #79c928ff">#</span> Desinstala un paquete</td>
  </tr>
  </tr>
    <td><span style="color: #f8d910ff">pip</span> <span style="color: #00eeffff">show</span> paquete
    </td>
    <td><span style="color: #79c928ff">#</span> Entrega información detallada sobre un paquete</td>
  </tr>
  </tr>
    <td><span style="color: #f8d910ff">pip</span> <span style="color: #00eeffff">list</span> --<span style="color: #FF0077">outdated</span>
    </td>
    <td><span style="color: #79c928ff">#</span> Lista los paquetes que tienen una versión nueva disponible</td>
  </tr>
</table>

## Consideraciones
- Para trabajar con Python se usa un entorno virtual. Esto permite aislar las dependencias. Es similar al directorio de node files.
- .venv\Scripts\activate: activa el entorno virtual.
- deactivate: desactiva el entorno virtual. Hay que estar en el directorio del entorno virtual.
- Cada dependencia del proyecto se debe instalar desde el ambiente virtual activo.

## Buenas prácticas reales
- Crear un entorno virtual por cada proyecto, incluso si es chico.
- Usar 'requirements.txt' en los repositorios para que otros puedan ejecutarlo.
- Versionar los archivos de entorno (pero no los archivos internos de venv)
- Activar siempre el entorno virtual antes de ejecutar el script.

## Errores comunes
- Instalar todo globalmente y después perder control de versiones.
- No saber qué versión de librería se está usando realmente.
- Romper un proyecto al actualizar algo para otro. Por eso todas las dependencias van aisladas en el entorno virtual.