# Uso de HELM para desplegar una pagina web
> **NOTA:** El contenido de la pagina esta mediante un **ConfigMap**, sin embargo, se puede customizar una imagen, subirla a quay/dockerhub y usar esa misma imagen para lanzar la app.

1) helm create **pagina_demo**
> Esto crea un chart de ejemplo. Luego puedes modificar values.yaml y los archivos en templates/ para adaptarlo a tu aplicación.
2) Editar y/o crear los archivos dentro de **Templates**
 
