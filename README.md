# JARVIS para iPhone — versión 1.0

PWA inicial diseñada para Safari en iPhone. No necesita cuenta ni API key. Incluye interfaz futurista, historial local, respuestas básicas, síntesis de voz y reconocimiento de voz cuando Safari lo admite.

## Qué hace esta versión
- Se puede instalar desde Safari en la pantalla de inicio después de publicarla con HTTPS.
- Responde a comandos básicos (hora, fecha, organización del día).
- Puede leer respuestas en voz alta.
- Intenta usar reconocimiento de voz de Safari con `webkitSpeechRecognition`.
- Guarda el historial en el almacenamiento local del navegador.
- Tiene una caché de PWA para abrir la interfaz cuando no haya conexión.

## Qué NO hace todavía
- No es todavía un chatbot de IA general: no hay un modelo de IA conectado.
- No escucha continuamente en segundo plano ni tiene una palabra de activación permanente.
- No puede controlar libremente otras apps de iOS.
- El reconocimiento de voz depende de la compatibilidad de Safari, permisos y conexión.

## Publicar gratis con GitHub Pages
Necesitas usar una computadora solo para subir los archivos una vez, o un servicio de edición de repositorios desde el propio iPhone. No necesitas ejecutar un servidor en tu PC.

1. Inicia sesión o crea una cuenta en GitHub.
2. Crea un repositorio nuevo llamado `jarvis-iphone` (puede ser público).
3. Sube todos los archivos y carpetas de este ZIP a la raíz del repositorio. Debe quedar `index.html` en la raíz.
4. En el repositorio, abre **Settings → Pages**.
5. En **Build and deployment**, selecciona **Deploy from a branch**, rama `main`, carpeta `/(root)`, y guarda.
6. Espera a que GitHub Pages publique el sitio. La dirección tendrá un formato parecido a `https://TU-USUARIO.github.io/jarvis-iphone/` (usa la URL exacta que GitHub muestre).
7. En tu iPhone 16 Pro, abre esa URL en **Safari**.
8. Pulsa **Compartir** → **Añadir a pantalla de inicio**. Si aparece, activa **Abrir como app web** y pulsa **Añadir**.
9. Abre JARVIS desde el icono nuevo. Toca el botón de voz y concede acceso al micrófono si Safari lo solicita.

## Uso desde iPhone sin computadora
Puedes intentar crear el repositorio y subir archivos desde Safari en el iPhone, pero cargar muchos archivos puede ser incómodo. Otra opción es pedir ayuda a alguien para el paso de publicación inicial. Una vez publicado, el uso diario es desde el iPhone.

## Privacidad
El historial se guarda en `localStorage` de ese navegador/dispositivo. No escribas contraseñas ni información sensible. Si borras los datos del sitio, se borrará el historial. No hay telemetría ni servicios externos integrados en esta versión.

## Personalización
Edita `index.html` para cambiar textos, colores y comandos. Si actualizas los archivos después de publicar, puede que la caché tarde en actualizarse; cierra y vuelve a abrir la PWA o actualiza el nombre de caché en `sw.js`.
