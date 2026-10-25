# Estimador ClO₂ para Android

Este proyecto envuelve la calculadora HTML en una aplicación Android sencilla (WebView). La calculadora funciona sin conexión y no solicita permisos de Internet.

## Obtener el APK con GitHub Actions

1. Crea un repositorio nuevo en GitHub y sube **todo el contenido de esta carpeta**.
2. En GitHub, entra en la pestaña **Actions** y habilita los workflows si te lo pide.
3. Ejecuta el workflow **Construir APK Android** desde Actions (`Run workflow`), o haz un `push` a la rama `main`.
4. Al terminar, abre la ejecución y descarga el artefacto **EstimadorClO2-debug-apk**.
5. Dentro del ZIP descargado estará `app-debug.apk`. Descárgalo en el móvil Android y ábrelo para instalarlo. Puede que Android solicite permitir la instalación desde esa fuente.

## Nota técnica importante

La app muestra una estimación estequiométrica teórica basada en los factores configurados para Fe(II) y Mn(II). No es una dosis operativa garantizada ni sustituye ensayos de tratabilidad, validación del responsable técnico o control de residual y subproductos. Comprueba siempre los requisitos de seguridad y normativa de la ETAP.

El APK que genera este flujo es de depuración (`debug`) y sirve para uso/pruebas personales. Para distribuirlo públicamente conviene generar una versión de lanzamiento firmada.
