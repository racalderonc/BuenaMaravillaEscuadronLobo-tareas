# COMANDOS DE GCLOUD

* ## ABRIR Google Cloud CLI
En primer lugar sera importante saber como abrir la terminal de google cloud para poder trabajar con los difentes comandos que mostraremos a continuación.

<video width="520" height="440" controls>
  <source src="images/Instances.mp4" type="video/mp4">
</video>


* ## COLOCARSE EN EL PROYECTO CORRESPONDIENTE
En primer lugar sera importante saber como abrir la terminal de google cloud para poder trabajar con los difentes comandos que mostraremos a continuación.
<p align="cente">
<img src="images/abrirCLI.gif" width="700">
</p>

* ## Listar Compute Engine
<br>

To list all instances in a project in table form, run:
```
gcloud compute instances list
```
<img src="images/2.gif" align="center">

To list the URIs of all instances in a project, run:
```
gcloud compute instances list --uri
```
<img src="images/3.gif" align="center" width="900">

* ## Listar IP's en uso, existentes o reservadas
<<<<<<< HEAD
To list all IP's in use, existing or reserved, run:
```
gcloud compute addresses list
```
=======
<br>

Lista de direcciones de cálculo de gcloud - lista de direcciones.
```
gcloud compute addresses list   
```
Enumera la información resumida de las direcciones en un proyecto. La --uri opción se puede utilizar para mostrar URI en su lugar. Los usuarios que deseen ver más datos deben utilizar gcloud compute addresses describe.
De forma predeterminada, se enumeran las direcciones globales y las direcciones de todas las regiones. Los resultados se pueden acotar proporcionando el indicador --regions o .--global

**Ejemplo**

<img src="images/addresses.gif" align="center" width="900">
>>>>>>> 5d1a29ca315f4e1d37d16edbe5d45ecec5fc1bff

Para enumerar los URI de todas las direcciones en un proyecto, ejecute:
```
gcloud compute addresses list --uri
```

Para enumerar todas las direcciones globales en un proyecto, ejecute:
```
gcloud compute addresses list --global
```

Para enumerar todas las direcciones de la us-central1región, ejecute:
```
gcloud compute addresses list --filter=region:us-central1
```

* ## Listar VPCs que están siendo compartidas desde el proyecto origen
<br>

Listar VPCs que están siendo compartidas desde el proyecto origen, ejecute:
```
gcloud compute shared-vpc associated-projects list host-project
```
**Ejemplo**

<img src="images/shared.gif" align="center" width="900">

* ## Listar Buckets disponibles
<br>

Para enumerar los bucket's de un proyecto, ejecute:
```
gsutil ls   
```
**Ejemplo**

<img src="images/gsutil.gif" align="center" width="900">

* ## Listar Service Accounts existentes en un proyecto

Ejecuta el comando `gcloud iam service-accounts list` para enumerar todas las cuentas de servicio de un proyecto.

Comando:

        gcloud iam service-accounts list 


<img src="images/serviceaccounts.gif" align="center" width="900">

El resultado es la lista de todas las cuentas de servicio en el proyecto:

| NAME | EMAIL |
| --- | --- |
| *SA_DISPLAY_NAME_1* | *SA_NAME_1*@*PROJECT_ID*.iam.gserviceaccount.com |
| *SA_DISPLAY_NAME_2* | *SA_NAME_2*@*PROJECT_ID*.iam.gserviceaccount.com |

**Ejemplo**

<p align="center">
<img src="images/service_account.jpg">
</p>


* ### **REFERENCIAS**

- Compute Engine [Como listar compute Engine](https://cloud.google.com/sdk/gcloud/reference/compute/instances/list).
- Service Accounts [Como listar cuentas de servicio](https://cloud.google.com/iam/docs/creating-managing-service-accounts?hl=es-419#listing).
- Direcciones IP  [Como listar direcciones IP's](https://cloud.google.com/sdk/gcloud/reference/compute/addresses/list).
- VPCs Compartidas [Como listar VPCs compartidas](https://cloud.google.com/sdk/gcloud/reference/compute/shared-vpc/associated-projects/list).






