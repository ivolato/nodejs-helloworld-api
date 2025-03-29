# NodeJs, helloworld API for test propouses.

This is a simple API that returns a welcome message.

## Objetivo

Este desafío tiene como objetivo realizar la configuración de un webhook en un repositorio de Github y también crear un simple pipeline para ejecutar un build y testear un proyecto nodejs.

## Descripción.
En este trabajo implementamos una solucion de CICD para automatizar el despliegue de la aplicacion. El repositorio es de una API de NodeJs.
Mediante la implementacion de Jenkins, a travez de un pipeline, el cual esta configurado para poder acceder a este repositorio, y la configuracion del Webhook automatizamos el proceso. 
El proceso comienza cuando (en este caso se configuro para este comando en particular) hacemos - git push - para subir los cambios al repositorio remoto, esto dispara una alerta a travez del Webhook hacia el Jenkins, esta ultima al recibirlo ejecuta el Job y comienza el proceso para descargar el contenido del repositio remoto y ejecutar los pasos declarados en el Jenkisfile.
La utilizacion de ngrok es necesario para poder dar acceso publico (ip Publica, acceso desde la red externa) del Webhook a Jenkisn.

## Requisitos.

Crear el Pipeline en Jenkins.
Activar ngrok para poder acceder publicamente.
Comfigurar el Webhub del repositorio.
