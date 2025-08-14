<p align="center">
   <img width="180" src="https://helm.sh/img/helm.svg">
   </p>

# Uso de HELM para desplegar una pagina web 

**Helm_http_demo_noAuth** es una aplicacion para entender un poco la estructura de HELM.

---
## Instalación
Sigue los pasos a continuación para configurar y ejecutar la aplicación:

1. Crear tu HELM
   ```
   helm create <name_helm>
   ```
2) Modificar los archivos que estan en el directorio **`templates`** para adaptarlos a tu aplicación.
   
3) Verifica que el chart se renderiza correctamente.
   ```
   helm template <name-helm-release> ./<path-chart>
   ```
4) Haz loggin a openshift y situate en el project donde desplegaras el Helm.
   ```
   oc project <name_project>
   ```
   ```
   kubectl project <name_project>
   ```
5) Despliega el HELM
   ```
   helm install <name-helm-release> ./<path-chart>
   ```
6) Si realizaste el cambio es necesario que hagas Upgrade al HELM
   ```
   helm upgrade <name-helm-release> ./<path-chart>
   ```

**Si deseas eliminar el Helm solo ejecuta**
```
helm uninstall <name-helm-release>
```

> **NOTA:** El contenido de la pagina esta almacenado en un configmap, sin embargo, se puede crear una image personalizada y desplegar la app basandose en esa imagen.
>
>⚠️ Este ejemplo está pensado para un repositorio público, por lo que no se requiere un archivo de autenticación.

