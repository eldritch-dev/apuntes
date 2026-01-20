# Python Cheat Sheet

## Consideraciones BD en Docker
<table>
  <h2>🪄 Backup desde el Contenedor</h2>
  <tr>
    <td><span style="color: #f8d910ff">docker</span> <span style="color: #00eeffff">exec</span>
      [nombre_del_contenedor>]/opt/mssql-tools/bin/sqlcmd \ <span style="color: #00eeffff">-S localhost
       -U SA -P</span> "[mi_password]"\ <span style="color: #00eeffff">-Q</span> 
       "BACKUP DATABASE [nombre_bd] TO DISK = N'/var/opt/mssql/backup/backup.bak' WITH INIT"
    </td>
    <td><span style="color: #79c928ff">#</span> Ejecuta un backup desde el contenedor</td>
  </tr>
  <tr>
    <td><span style="color: #f8d910ff">docker</span> cp<span style="color: #00eeffff"> [nombre_del_contenedor]:</span>/var/opt/mssql/backup/backup.bak ./backup.bak
    </td>
    <td><span style="color: #79c928ff">#</span> Copia backup a mi máquina</td>
  </tr>
</table>


- Guarda el backup en una carpeta fuera del contenedor.
- Verifica el backup (abre el archivo, revisa tamaño, etc).
- Hacer backup de la DB antes de cada migración importante.