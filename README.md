
<h1 align="center">PROYECTO ASIR KUBERNETES</h1>

Este repositorio contiene los archivos YAML utilizados para desplegar varias aplicaciones en un clúster de Kubernetes. El proyecto está orientado a la demostración de conceptos fundamentales de Kubernetes, incluyendo el uso de **Deployments**, **Services**, **Persistent Volumes (PV)** y **Persistent Volume Claims (PVC)**. Los recursos están organizados en carpetas para facilitar su comprensión y aplicación.

## Estructura del repositorio

Los archivos YAML están organizados en las siguientes carpetas:

- **`hello-world/`**  
  Contiene los archivos necesarios para desplegar una aplicación simple de "Hello World". Incluye un Deployment y un Service para exponer la aplicación.

- **`wordpress-mysql/`**  
  Incluye los archivos para desplegar una aplicación de WordPress junto con MySQL, con sus respectivos Deployment y Service para ambos.

- **`pv-pvc/`**  
  Contiene el archivo YAML para configurar un **PersistentVolume (PV)** y un **PersistentVolumeClaim (PVC)**, necesarios para gestionar almacenamiento persistente dentro del clúster.

## ¿Cómo usar estos archivos?

### Pre-requisitos:
1. Tener un clúster de Kubernetes en funcionamiento.
2. Tener acceso a `kubectl` para aplicar los archivos YAML.

### Desplegar las aplicaciones:
1. Clona este repositorio y navega hasta la carpeta de los manifiestos que desees aplicar.
2. Usa el siguiente comando para aplicar los archivos de configuración:

   ```bash
   kubectl apply -f <archivo>.yaml
   ```

### Archivos incluidos:
Los manifiestos contienen configuraciones para crear **Pods**, **Services**, y persistencia de datos utilizando **PV** y **PVC**.

## Descripción de las aplicaciones

- **Hello World**  
  Una aplicación básica para probar el funcionamiento de Kubernetes. Desplegada con un Deployment y expuesta mediante un Service.

- **WordPress y MySQL**  
  Un despliegue de una aplicación web de WordPress con su base de datos MySQL, donde ambos servicios están configurados con sus respectivos Deployments y Services.

- **Persistent Storage**  
  Configuración de almacenamiento persistente utilizando un PersistentVolume y un PersistentVolumeClaim que aseguran que los datos de las aplicaciones (como los de MySQL) no se pierdan si los Pods se reinician.

## Contribuciones

Si tienes mejoras o sugerencias, ¡siéntete libre de hacer un pull request! Este repositorio es para demostrar el proceso de despliegue de aplicaciones en Kubernetes, pero siempre estamos abiertos a mejoras. 
Alberto Vázquez 😊
