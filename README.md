# Actualizaciones de Automata

Descarga e instala el APK de la [última versión estable](https://github.com/delucaiago-bot/automata-actualizaciones/releases/latest).
Android puede pedirte permiso para instalar aplicaciones desde el navegador. Las futuras versiones se ofrecen desde Automata y conservan tus macros.

Este repositorio contiene los APK y el flujo de avisos de Firebase Cloud Messaging. El código de la app, los datos de los usuarios y las claves privadas no se publican aquí.

Cada versión incluye un archivo `automata-<versión>-<código>.apk` y sus novedades. Automata comprueba las actualizaciones al abrirse, desde Ajustes y periódicamente en segundo plano.

La acción **Avisar versión nueva** envía el aviso cuando se publica una release estable. El envío automático está activado mediante el secreto `FIREBASE_SERVICE_ACCOUNT` y la variable `FIREBASE_PUSH_ENABLED=true`.

La cuenta de envío es exclusiva de Automata y tiene únicamente el rol de Firebase Cloud Messaging en el proyecto `automata-actualizaciones`. Su clave privada se guarda como secreto de GitHub Actions. El lanzamiento manual con `dry_run=true` permite validar el aviso sin enviarlo; la validación inicial se completó correctamente.
