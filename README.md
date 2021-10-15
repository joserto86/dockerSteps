# Docker

## Dockerfile directives

- `FROM`: Establece la imagen base a partir de la que se creará el nuevo contenedor
- `MAINTAINER`: Establece el autor de la imagen generada
- `RUN`: Ejecuta comandos dentro de la nueva imagen que se está construyendo.
- `CMD`: Define un comando por defecto cuando el contenedor se arranca.
- `EXPOSE`: Informa a Docker que el contenedor escucha en la red específica en el momento de la ejecución
- `ENV`: Estable variables de entorno
- `ADD`: Para copiar ficheros/directorios desde el host hacia el contenedor, este comando permite que la fuente sea una url
- `COPY`: También para copiar ficheros/directorios desde el host hacia el contenedor, salvo que éste no permite que la fuente sea una url
- `ENTRYPOINT`: Similar a CMD, se suele utilizar cuando el contenedor ejecuta un determinado script y nada mas. Combinados ambos, ENTRYPOINT y CMD, el primero establece el comando y el segundo los argumentos. A ENTRYPOINT no se le pueden definir argumentos.
- `VOLUME`: Crea un punto de montaje para compartir ficheros entre el host y el contenedor
- `USER`: Crea un usuario dentro del contenedor.
- `WORKDIR`: Establece el directorio de trabajo dentro del contenedor.
- `ARG`: Define una variable en tiempo de construcción del contenedor.
- `ONBUILD`: Añade una instrucción que se desencadena cuando la imagen se está usando como base de otro 'build'
- `STOPSIGNAL`: Establece la señal de sistema que será enviada al contenedor para salir
- `LABEL`: Aplica una clave de metadatos a la imagen/contenedor/demonio
