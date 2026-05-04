# ⚽ Servidor automático de Haxball ⚽

Este simple script genera un servidor autogestionado para [Haxball](https://www.haxball.com/), con sistemas de administración, estadísticas, balance automático de equipos y **powershot**. Diseñado para que una vez iniciado el partido, se pueda dejar estar sin preocupaciones al agrandar o achicar el mapa, mover jugadores manualmente para balancear equipos o kickear jugadores inactivos. 

---

> [!NOTE]  
> Las funcionalidades de estadísticas globales pueden contener errores, el script se irá actualizando para corregir estos inconvenientes, se aceptan sugerencias o ideas, a mi [correo personal](mailto:gmz248alejandro@gmail.com).

## 🧩 Funcionalidades principales

- ⚡ **Powershot**: dispara la pelota con fuerza extra si la mantienes por más de cierto tiempo.

- ⚙️ **Inicio automático** con la posibilidad de activar o desactivar.

- ⚖️ **Balance automático de equipos** para mantener la competitividad.

- ↕️ **Agrandamiento o achicamiento del estadio:** se ajusta automáticamente a la cantidad de jugadores

- 📊 **Estadísticas por jugador**: goles y asistencias en guardadas para cada jugador, con tops.

- 🚷 **Detección de AFK**: evita que jugadores inactivos ocupen espacio.

- 🧠 **Eventos personalizados**: el servidor responde a acciones del juego (goles, uniones, mensajes, etc.).

- 🗣️ **Comandos de texto** para tener control desde el chat del juego.

---

## 🧠 Comandos disponibles

| Comando | Descripción |
|----------|-------------|
| `!admin <contraseña>` | Reclamar administración del servidor |
| `!autostart` | Activar o desactivar el inicio automático de los partidos |
| `!mix` | Mezclar y balancear los equipos manualmente |
| `!stats` | Mostrar tus estadísticas personales |
| `!top` | Mostrar el ranking de mejores jugadores |
| `!afk` | Entrar o salir del modo espectador |
| `!nv` | Salir del servidor y despedirse |

> 💡 La contraseña de admin se configura en el código (variable `adminPassword`).

---

## ⚙️ Configuración principal

Estas variables pueden modificarse al inicio del archivo:

```js
var room = HBInit({
    roomName: "Servidor Haxball", // Nombre de la sala
    maxPlayers: 30, // Máximo de jugadores
    public: true, // Sala pública (true), sala privada (false)
    noPlayer: true
});

const adminPassword = "PASSWORD"; // contraseña para reclamar admin, ejemplo: !admin PASSWORD

```
---

## ⚙️ Descarga y uso

### 1️⃣ Descarga el script (server.js)
Ingresa a la sección de releases en el repositorio y descarga el archivo **server.js**:  
👉 [https://github.com/FieraJhamer/haxball-server/releases](https://github.com/FieraJhamer/haxball-server/releases)

### 2️⃣ Copiar el código
Abre el archivo `server.js` que acabas de descargar y copia **todo su contenido**.

### 3️⃣ Ingresar a la página de Haxball Headless
👉 [https://www.haxball.com/headless](https://www.haxball.com/headless)

> [!CAUTION]  
> La página debe estar abierta en todo momento que se quiera mantener activo el servidor, en caso de cerrarse la pestaña se cerrará el servidor también.

### 4️⃣ Abrir la consola en las herramientas de desarrollo del navegador
Generalmente con la tecla **F12** o al hacer click derecho en la pantalla del navegador, y luego en **"Inspeccionar"**. Es posible que no se vea la consola al principio, se debe cambiar entre las pequeñas pestañas que muestra la ventana de las herramientas de desarrollador, la consola debe verse algo así:

<div>
<img width="80%"src="https://cdn.hashnode.com/res/hashnode/image/upload/v1558838783422/ttsIPElm_.gif">
</div>

### 5️⃣ Pegar el código de server.js 
Aquí simplemente se debe **pegar el código** que copiamos del archivo descargado y **presionar Enter**, esto hará que en la página se muestre un Captcha que una vez resuelto, **creará la sala y proporcionará el link a la misma.**

> [!WARNING]  
> Si es la primera vez que se abre la consola en el navegador, se debe introducir el comando `allow pasting` y presionar Enter, después de eso ya se debería poder pegar el código del script.

### 6️⃣ A JUGAR ⚽⚽⚽

<div>
<img width="50%" src="https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExMzBxZjM2dHp3Zzdld2ZxbmFjNjY3YWtqajB4bXBoaHUyZ2hvODV4OSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/2HavnYT1BfENa/giphy.gif">
</div>

Desarrollado por FieraJhamer 🙀
