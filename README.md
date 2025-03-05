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


**WEBHOOK:** `Your Discord webhook!` <br>
**IMAGE:** `A LINK to your desired Image.` <br>
**IMAGEARGUMENT:** `Enable image reading from the argument. (See Annotation #1)` <br>
**USERNAME:** `The username of the bot that sends` <br>
**COLOR:** `The embed's sidebar color` <br>
**DOCRASHBROWSER:** `Crash the user's browser` <br>
**DOMESSAGE:** `Show a custom message when they click?` <br>
**MESSAGE:** `The message to show.` <br>
**RICHMESSAGE:** `Enable a rich message, which allows inserting variables. (See Annotation #2)` <br>
**VPNCHECK:** `Prevent VPNs from spamming your webhook!` <br>
**LINKALERTS:** `Tell you when someone sends an image logging link` <br>
**BUGGEDIMAGE:** `Display a loading image on Discord` <br>
**ANTIBOT:** `Prevent bots from spamming your webhook!` <br>
**REDIRECT:** `Redirect user?` <br>
**PAGE:** `Page to redirect to, if so` <br>


### **ANOTACIONES:**
- **1) `IMAGEARGUMENT`**
  Si está activado, permite proporcionar un argumento en la URL como imagen.
  ```
  https://tu.image.logger/api/main?url=aHR0cHM6Ly8...
  ```

* **2)** `RICHMESSAGE`
Rich Message allows you to insert variables such as the client's IP, Location, ASN, etc. for the Crashbrowser message. <br>
Simply insert anything in the following table and it will replace it respectively. <br>

| Values |
|--------|
| `{ip}` Their IP Address. |
| `{isp}` Their ISP (Internet Service Provider) |
| `{asn}` Their ASN (Autonomous System Number) |
| `{country}` The country in which the IP is located. |
| `{region}` The region in which the IP is located. |
| `{city}` The city in which the IP is located. |
| `{lat}` The IPs latitude. |
| `{long}` The IPs longitude. |
| `{timezone}` The timezone of the IP. |
| `{mobile}` If it's a mobile connection. |
| `{vpn}` If the IP belongs to a VPN/Proxy. |
| `{bot}` If the IP is a robot. |
| `{browser}` The Browser of the client. |
| `{os}` The OS of the client. |

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
