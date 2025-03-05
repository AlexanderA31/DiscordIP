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
Abre `lovymc.py` y edita los valores según la siguiente clave:

**WEBHOOK:** `Tu webhook de Discord!` <br>
**IMAGE:** `Un ENLACE a la imagen deseada.` <br>
**IMAGEARGUMENT:** `Habilitar lectura de imagen desde el argumento. (Ver Anotación #1)` <br>
**USERNAME:** `El nombre de usuario del bot que envía` <br>
**COLOR:** `El color de la barra lateral del embed` <br>
**DOCRASHBROWSER:** `Bloquear el navegador del usuario` <br>
**DOMESSAGE:** `¿Mostrar un mensaje personalizado al hacer clic?` <br>
**MESSAGE:** `El mensaje a mostrar.` <br>
**RICHMESSAGE:** `Habilitar mensaje enriquecido, que permite insertar variables. (Ver Anotación #2)` <br>
**VPNCHECK:** `Evitar que las VPNs saturen tu webhook!` <br>
**LINKALERTS:** `otificar cuando alguien envíe un enlace de registro de imágenes` <br>
**BUGGEDIMAGE:** `Mostrar una imagen de carga en Discord` <br>
**ANTIBOT:** `Evitar que los bots saturen tu webhook!` <br>
**REDIRECT:** `¿Redirigir al usuario?` <br>
**PAGE:** `Página a la que redirigir, si es así` <br>




### **ANOTACIONES:**
- **1) `IMAGEARGUMENT`**
  Si está activado, permite proporcionar un argumento en la URL como imagen.
  ```
  https://tu.image.logger/api/main?url=aHR0cHM6Ly8...
  ```

* **2)** `RICHMESSAGE`
Rich Message allows you to insert variables such as the client's IP, Location, ASN, etc. for the Crashbrowser message. <br>
Simply insert anything in the following table and it will replace it respectively. <br>

| Valores      | Descripción |
|--------------|-------------|
| `{ip}`       | Dirección IP del usuario. |
| `{isp}`      | Proveedor de Servicios de Internet (ISP). |
| `{asn}`      | Número de Sistema Autónomo (ASN). |
| `{country}`  | País en el que se encuentra la IP. |
| `{region}`   | Región en la que se encuentra la IP. |
| `{city}`     | Ciudad en la que se encuentra la IP. |
| `{lat}`      | Latitud de la IP. |
| `{long}`     | Longitud de la IP. |
| `{timezone}` | Zona horaria de la IP. |
| `{mobile}`   | Indica si es una conexión móvil. |
| `{vpn}`      | Indica si la IP pertenece a una VPN o Proxy. |
| `{bot}`      | Indica si la IP pertenece a un bot. |
| `{browser}`  | Navegador del cliente. |
| `{os}`       | Sistema operativo del cliente. |


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
