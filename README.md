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




