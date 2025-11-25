# Nginx con Docker

## Estructura de carpetas
![Imagen de estructura de carpetas](./img/001.png)

### Clonación del repositorio en "html"
![Imagen de clonación de repositorio](./img/002.png)

## Configuración de Nginx
![Imagen de archivo de configuración de Nginx](./img/003.png)

### Creación y ejecución del contenedor
¡NOTA: Al estar en Windows, al ejecutar el contenedor necesita una ruta absoluta o no funcionará, se necesita cambiar "~" por "C:/Users/[usuario]"!
<br>
<br>
Comando: docker run -d --name nginx-dani -p 80:80 -v ~/nginx/dani.test/html:/usr/share/nginx/html -v ~/nginx/dani.test/conf/nginx.conf:/etc/nginx/conf.d/default.conf nginx:latest

![Imagen de contenedor en ejecución](./img/004.png)

## Comprobación de funcionamiento
![Imagen de comprobación de funcionamiento](./img/005.png)

### Logs
![Imagen de logs](./img/006.png)

## Gestión del contenedor
### Detener el contenedor
![Imagen de detener el contenedor](./img/007.png)

### Reiniciar el contenedor
![Imagen de reiniciar el contenedor](./img/008.png)

### Eliminar el contenedor
![Imagen de eliminar el contenedor](./img/009.png)