#FROM nginx:latest
FROM ubuntu:24.04
RUN apt update && apt install nginx -y
WORKDIR /var/www/html
RUN apt update && apt install git -y
RUN git clone https://github.com/josejuansanchez/2048 && \ 
    mv /var/www/html/2048/* /var/www/html
CMD ["nginx", "-g", "daemon off;"]
    #docker run -d -p 80:80 2048 para verlo en la web con el puerto80 de mi maquina
#docker tag nombre actual nombre nuevo: hace una copia renombrada 

#docker push nombre imagen para subir la imagen
#https://github.com/josejuansanchez/2048-github-actions/tree/main/.github/workflows para la actividad nueva
#https://github.com/josejuansanchez/2048-github-actions.git