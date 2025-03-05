# 📸 Registrador de Imágenes de Discord [ARCHIVADO]

**¡Este proyecto ha sido archivado!** Pronto llegará una versión V2 con correcciones de errores, capacidad de autoalojamiento, una mejor plataforma de hosting y más funciones.

**Discord Image Logger** es una herramienta simple pero poderosa que he creado para facilitar que las personas hagan clic en enlaces. Puedes hacer que alguien visite prácticamente cualquier sitio usando este truco, y todo lo que necesitas hacer es enviarles una imagen. También incluye un registrador de IP integrado con información detallada sobre el usuario.

Ten en cuenta que esto **NO** es un registrador de imágenes de "un solo clic". Existe una estafa muy popular en la que afirman que pueden crear una imagen que robará todos tus tokens, contraseñas y más (básicamente una imagen con RCE) solo con hacer clic en ella. Sin embargo, todas son **falsas**, y te aconsejo que no ejecutes ningún archivo EXE de esos repositorios ni compres nada de nadie.

**Si vas a hacer un fork de este repositorio, ¡dale una estrella también!**

## 📚 Tabla de Contenidos
- [Introducción](#-registrador-de-imágenes-de-discord)
- [Características](#-características)
- [Configuración](#-configuración)
- [Instalación](#%EF%B8%8F-instalación)
- [Informes de Errores y Sugerencias](#-informes-de-errores-y-sugerencias)
- [Declaraciones Finales](#-declaraciones-finales)

---

## 💎 Características
- ¡Rápido, gratis y fácil!
- ¡100% anónimo y no rastreable!
- Solo requiere hacer clic en "Abrir original".
- Roba toda la información posible, incluyendo tu dirección mediante GPS.
- ~~Bajo desarrollo activo, muchas funciones nuevas serán añadidas.~~ No tanto, pero una nueva versión se desarrollará pronto. ¡Deja tus ideas!

---

## 🔧 Configuración

Antes de instalarlo, modifiquemos el **config.**  
Abre `main.py` y edita los valores según la siguiente clave:

```ini
WEBHOOK: Tu webhook de Discord.
IMAGE: Un ENLACE a la imagen deseada.
IMAGEARGUMENT: Habilitar lectura de imagen desde el argumento. (Ver Anotación #1)
USERNAME: El nombre de usuario del bot que envía.
COLOR: Color de la barra lateral del embed.
DOCRASHBROWSER: ¿Bloquear el navegador del usuario?
DOMESSAGE: ¿Mostrar un mensaje personalizado al hacer clic?
MESSAGE: El mensaje a mostrar.
RICHMESSAGE: Habilitar mensaje enriquecido con variables. (Ver Anotación #2)
VPNCHECK: Evitar que VPNs saturen tu webhook.
LINKALERTS: Avisarte cuando alguien envíe un enlace de registro de imágenes.
BUGGEDIMAGE: Mostrar una imagen de carga en Discord.
ANTIBOT: Evitar que bots saturen tu webhook.
REDIRECT: ¿Redirigir al usuario?
PAGE: Página a la que redirigir, si es así.
```

### **ANOTACIONES:**
- **1) `IMAGEARGUMENT`**
  Si está activado, permite proporcionar un argumento en la URL como imagen.
  ```
  https://tu.image.logger/api/main?url=aHR0cHM6Ly8...
  ```

- **2) `RICHMESSAGE`**
  Permite insertar variables como la IP del cliente, ubicación, ASN, etc.

---

## ⚒️ Instalación

Ahora que está configurado, ¡vamos a instalarlo!

1. Crea un repositorio en GitHub (recomiendo hacerlo privado).
2. Crea una carpeta llamada `api` y coloca dentro `requirements.txt` y `main.py`.
3. *(Opcional)* En el directorio raíz, crea un archivo `index.html` con:
   ```html
   <meta http-equiv="refresh" content="0;url=./api/main.py">
   ```
4. Ve a [Vercel](https://vercel.com) e inicia sesión con GitHub.
5. Importa tu repositorio.
6. Copia el dominio generado y usa `tuprojecto.vercel.app/api/main`.

Puedes agregar un dominio personalizado si tienes uno.

---

## 🐛 Informes de Errores y Sugerencias

**¿Encontraste un error? ¿Tienes una idea?** Háznoslo saber [aquí](../../issues).

**NOTA:** __NO__ ejecutes `main.py` directamente. Sigue las instrucciones.

**Errores conocidos:** Ninguno por el momento.

---

## 📜 Declaraciones Finales

¿Te gustó el proyecto? ¡Déjame una estrella ⭐!  

¡Gracias por usar mis herramientas! 🙏
