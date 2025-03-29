# NodeJs, helloworld API for test propouses.

This is a simple API that returns a welcome message.

## Objetivo

Este desafío tiene como objetivo realizar la configuración de un webhook en un repositorio de Github y también crear un simple pipeline para ejecutar un build y testear un proyecto NodeJs.

## Descripción.
En este trabajo implementamos una solución de CICD para automatizar el despliegue de la aplicación. El repositorio es de una API de NodeJs.
Mediante la implementación de Jenkins, a través de un pipeline, el cual está configurado para poder acceder a este repositorio, y la configuración del Webhook automatizamos el proceso. 
El proceso comienza cuando (en este caso se configuró para este comando en particular) hacemos - git push - para subir los cambios al repositorio remoto, esto dispara una alerta a través del Webhook hacia el Jenkins, esta última al recibirlo ejecuta el Job y comienza el proceso para descargar el contenido del repositorio remoto y ejecutar los pasos declarados en el Jenkisfile.
La utilización de ngrok es necesario para poder dar acceso público (ip Pública, acceso desde la red externa) del Webhook a Jenkins.

## Requisitos.

Crear el Pipeline en Jenkins.
Activar ngrok para poder acceder públicamente.
Configurar el Webhub del repositorio.

