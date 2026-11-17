# Actualizaciones de Automata

Descarga e instala el APK de la [última versión estable](https://github.com/delucaiago-bot/automata-actualizaciones/releases/latest).
Android puede pedirte permiso para instalar aplicaciones desde el navegador. Las futuras versiones se ofrecen desde Automata y conservan tus macros.

Este repositorio contiene los APK y el flujo de avisos de Firebase Cloud Messaging. El código de la app, los datos de los usuarios y las claves privadas no se publican aquí.

Cada versión incluye un archivo `automata-<versión>-<código>.apk` y sus novedades. Automata comprueba las actualizaciones al abrirse, desde Ajustes y periódicamente en segundo plano.

La acción **Avisar versión nueva** envía el aviso cuando se publica una release estable. Necesita el secreto `FIREBASE_SERVICE_ACCOUNT` del proyecto `automata-actualizaciones` y la variable `FIREBASE_PUSH_ENABLED=true`. La variable permanece desactivada hasta autorizar y verificar la credencial de publicación. El lanzamiento manual permite validar el aviso sin enviarlo.
