Test de Docker


Se comenzaron con las prácticas de usabilidad de Docker


Pasos para crear un archivo de Docker


Primero se genera una carpeta usando el comando "mkdir mi-primer-dockerfile"

Luego entramos a la carpeta "cd mi-primer-dockerfile"

Luego abrimos el editor de docker: "vim Dockerfile"

Luego usamos los comandos: "FROM nginx" y "COPY static-html-directory /usr/share/nginx/html"
para que se inicie un contendido estático

Luego creamos una nueva carpeta "mkdir static-html-directory"

Luego entramos a la carpeta "cd static-html-directory" y usamos el comando "vim index.html"

Luego escribimos lo que queremos escribir en ese archivo y ejecutamos el 
comando: "docker image build -t some-content-nginx ."


Para crear una imagen y checkearla, se tiene que usar los siguientes comandos:

"docker image build -t some-content-nginx ."
"docker image ls"

Luego vamos a la página de docker, y creamos nuestra cuenta
 y desde el comando iniciamos sesión con el comando " docker login"

Luego creamos un tag con el siguiente comando:
docker tag some-content-nginx xxxxxx/yyyyyy-yyy
Siendo "X" el usuario de Docker y "Y" el tag del repo

mi caso sería: kyokazu/fedesoft-kyokazu
se adjunta Screenshot en la carpeta.

Luego se carga
docker push kyokazu/fedesoft-kyokazu

Y ya se queda generada la imagen, el repo y el tag


