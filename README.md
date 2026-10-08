🌐 WebServer

WebServer es una aplicación Android creada para convertir el dispositivo en un servidor web local. 🚀📱

La aplicación permite alojar archivos web directamente desde el dispositivo y acceder a ellos desde un navegador utilizando la red local.

«🔥 Proyecto creado por Eituprocoder.»

---

🚀 ¿Qué hace?

WebServer crea un servidor HTTP local que puede servir archivos directamente desde una carpeta del dispositivo.

Esto permite utilizar el teléfono como un pequeño servidor para proyectos como:

- 🌐 Páginas web
- 🎮 Juegos HTML
- ⚙️ Aplicaciones web
- 📱 PWAs
- 🎨 Proyectos HTML/CSS/JS
- 📄 Documentos
- 🎵 Audio
- 🎬 Vídeos
- 🧪 Prototipos y pruebas locales

---

✨ Características

🌐 Servidor HTTP local

El servidor utiliza HTTP y escucha por defecto en el puerto 8080.

http://IP-DEL-DISPOSITIVO:8080

El servidor puede aceptar conexiones desde la red local.

---

📂 Explorador de archivos web

Cuando se accede a una carpeta, WebServer puede mostrar una interfaz web para explorar los archivos disponibles.

También detecta automáticamente:

index.html
index.htm

como páginas principales de una carpeta.

---

📦 Compatibilidad con archivos

WebServer reconoce diferentes tipos de contenido, incluyendo:

Tipo| Extensiones
🌐 HTML| ".html", ".htm"
⚙️ JavaScript| ".js"
🎨 CSS| ".css"
🖼️ Imágenes| ".png", ".jpg", ".jpeg", ".gif", ".svg", ".webp"
🎵 Audio| ".mp3", ".ogg", ".wav"
🎬 Vídeo| ".mp4", ".webm"
📄 Texto| ".txt"
📑 PDF| ".pdf"
📦 Datos| ".json"
🧩 WebAssembly| ".wasm"

---

⚡ Streaming y archivos grandes

El servidor implementa soporte para solicitudes HTTP "Range".

Esto permite realizar transferencias parciales de archivos y facilita el funcionamiento con contenido multimedia y archivos grandes.

También utiliza bloques de transferencia de hasta 128 KB.

---

🔒 Seguridad

WebServer incorpora varias medidas para evitar accesos incorrectos a archivos:

- Bloqueo de rutas ".."
- Protección contra rutas fuera de la carpeta raíz
- Rechazo de determinadas rutas inválidas
- Protección contra enlaces simbólicos en el explorador
- "X-Content-Type-Options: nosniff"
- Control de solicitudes "Range"
- Tiempo de espera de conexiones

El servidor está pensado principalmente para uso local y desarrollo.

---

📊 Registro de solicitudes

La aplicación mantiene estadísticas del servidor, incluyendo:

- Número de solicitudes recibidas
- Registro de las últimas solicitudes
- Dirección del cliente
- Información básica de cada petición

El historial mantiene hasta 60 registros recientes.

---

🧠 Tecnología

El proyecto combina Android con Python.

Android

La APK utiliza:

- Android
- Java/Kotlin runtime de Android
- Servicio de hosting
- Interfaz nativa

Python

El servidor está implementado utilizando módulos estándar de Python como:

http.server
threading
mimetypes
urllib.parse
os
json
re

La aplicación utiliza Chaquopy para ejecutar Python dentro de Android.

---

🎮 ¿Para qué puede servir?

WebServer puede ser especialmente útil para desarrolladores que quieran probar sus proyectos directamente desde un teléfono.

Por ejemplo:

📱 Android
   ↓
🌐 WebServer
   ↓
📂 MiJuego/
   ├── index.html
   ├── style.css
   ├── game.js
   ├── textures/
   └── audio/

Después, otro dispositivo conectado a la misma red puede acceder al proyecto mediante el navegador.

---

🛠️ Ejemplo

Si el servidor está ejecutándose en el puerto "8080" y el dispositivo tiene una IP local como:

192.168.1.25

otro dispositivo de la misma red podría acceder a:

http://192.168.1.25:8080

---

📱 Ideal para proyectos

WebServer puede utilizarse para probar proyectos como:

- 🎮 Juegos de navegador
- 🕹️ Fangames
- 🤖 Prototipos de IA web
- 🌐 Sitios HTML
- 📱 PWAs
- 🧪 Experimentos JavaScript
- 🎨 Experimentos Three.js
- 🔧 Herramientas web locales

---

🔥 Filosofía del proyecto

La idea de WebServer es sencilla:

«Convertir un dispositivo Android en una pequeña plataforma de hosting local.»

Sin necesidad de subir el proyecto a Internet para realizar pruebas dentro de una red local.

---

📜 Estado del proyecto

Estado: 🟢 Funcional

Plataforma: Android

Servidor: HTTP

Puerto predeterminado: "8080"

Backend: Python

Runtime Python: Chaquopy

Dependencias externas del servidor: Ninguna

---

👨‍💻 Autor

Eituprocoder

🎮 Game Developer
💻 Web Developer
🤖 AI & Programming Projects

---

⭐ Créditos

Proyecto desarrollado por Eituprocoder.

Si este proyecto te resulta útil, ¡puedes darle una ⭐ al repositorio!

---

🚀 WebServer

Your Android device. Your files. Your local web server.

😎📱🌐🔥
