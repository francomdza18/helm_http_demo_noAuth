# Uso de HELM para desplegar una pagina web
> **NOTA:** El contenido de la pagina esta almacenado en un configmap, sin embargo, se puede crear una image personalizada y desplegar la app basandose en esa imagen.

1) Crear tu HELM
   ```helm create <name_helm>```

2) Modificar values.yaml y los archivos en templates/ para adaptarlo a tu aplicación.
3) Verifica que el chart se renderiza correctamente.
```helm template <name-helm-release> ./<name_helm>```
4) 
5) 
