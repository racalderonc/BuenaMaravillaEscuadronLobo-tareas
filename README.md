# Comandos básicos de gcloud

## Compute Engine

### Describe Proyectos

Ejecuta el siguiente comando para consultar información sobre tu proyecto de Compute Engine, como metadatos del proyecto, claves SSH y métricas de cuotas:

            gcloud compute project-info describe

### Trabaja con VM

Con los siguientes comandos se muestran tareas comunes cuando se trabaja con instancias de máquina virtual (VM).

- **Crea VM**

            gcloud compute instances create *VM_NAME* \ 
                [--image *IMAGE* | --image-family *IMAGE_FAMILY*] \
                --image-project *IMAGE_PROJECT*

donde

*VN_NAME*: El nombre de la VM

*IMAGE* o *IMAGE_FAMILY*: Especifica alguna de las siguientes opciones:

    - *IMAGE*: Es la versión requerida de una imagen pública. Por ejemplo: `--image debian-10-buster-v20200309`
    
    - *IMAGE_FAMILY*: Es una familia de imágenes. Esto crea la VM a apartir de la imagen de SO no obsoleta más reciente. Por ejemplo, si especificas `--image-family debian-10`, Compute Engine crea una VM a partir de la última versión de la imagen de  SO en la familia de imágenes Debian 10.

*IMAGE_PROJECT*: El proyecto que tiene la imagen.

<span style="color: green"> Some green text </span>

- **Ennumera las VM**






