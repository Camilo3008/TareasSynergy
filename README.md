# TareasSinergy

Primero tenemos que iniciar los servicios de php y mysql en laragon o cualquier entorno de desarrollo compatible. 
Luego de esto tenemos que crear una carpeta en www si estamos trabajando con laragon, llamamos a esta carpeta
PruebaSynergy, alli bajaremos el repocitorio.
Encontraremos una carpeta llamada BD, alli se encontrara una copia de la base de datos utilizada para el desarrollo del ejercicio. 
Tendremos que importarla y llamarla sinergycrud

Nos ubicamos en la carpeta SinergyCrudClientes y creamos un documento llamado:
.htaccess
y copeamos la siguiente informacion: 

Options All -Indexes
Options -MultiViews
RewriteEngine on
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule ^(.*)$ index.php?url=$1 [QSA,L]


Luego de esto copeamos lo siguiente en el navegador para probar el sistema:
http://localhost/PruebaSynergy/SinergyCrudClientes/Views/tareas.php
