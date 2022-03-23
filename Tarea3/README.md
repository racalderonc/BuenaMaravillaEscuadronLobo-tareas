# COMANDOS DE GCLOUD

* ## Listar Compute Engine
<br>

To list all instances in a project in table form, run:
```
gcloud compute instances list
```
<img src="images/list-compute-engine.png" align="center" width="900">

To list the URIs of all instances in a project, run:
```
gcloud compute instances list --uri
```
<img src="images/list-compute-engine-uri.png" align="center" width="900">

* ## Listar IP's en uso, existentes o reservadas

* ## Listar Buckets disponibles
<br>

Para enumerar los bucket's de un proyecto, ejecute:
```
gsutil ls   
```
**Ejemplo**

<img src="images/BucketGCP.PNG" align="center" width="900">

* ## Listar Service Accounts existentes en un proyecto

Ejecuta el comando `gcloud iam service-accounts list` para enumerar todas las cuentas de servicio de un proyecto.

Comando:

        gcloud iam service-accounts list 


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








