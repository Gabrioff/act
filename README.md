# 🚀 DegenTerminal

**Trading, Casino & Social Gaming Platform**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![MQTT](https://img.shields.io/badge/MQTT-Protocol-660066?logo=mqtt&logoColor=white)](https://mqtt.org/)
[![PeerJS](https://img.shields.io/badge/WebRTC-PeerJS-blue)](https://peerjs.com/)

---

## 📖 Descripción

**DegenTerminal** es una plataforma web descentralizada y serverless que combina:

- 📊 **Trading Simulado**: Gráficos en tiempo real, órdenes de compra/venta y portafolio
- 🎰 **Casino Games**: Juegos de azar con mecánicas tipo "degen" trading
- 💬 **Social Hub**: Chat en tiempo real, salas privadas y avatares personalizables
- 🎮 **Mini Games**: Carreras y otros juegos multijugador P2P

Todo esto sin necesidad de backend tradicional, utilizando **MQTT** para mensajería en tiempo real y **WebRTC/PeerJS** para conexiones peer-to-peer.

---

## ✨ Características Principales

### 🔐 Autenticación Serverless
- Sistema de perfiles con almacenamiento local
- Avatares personalizables (👽 🦍 🐸 🐶 🤖 💀 🤡 etc.)
- Códigos de sala únicos para sesiones privadas

### 📈 Trading Terminal
- Gráficos de velas en tiempo real
- Órdenes Long/Short con apalancamiento
- Sistema de PnL (Profit & Loss)
- Historial de trades
- Gestión de portafolio con balance virtual

### 🎰 Casino & Games
- **Crash Game**: Apuesta antes del crash
- **Roulette**: Ruleta con múltiples opciones
- **Car Racing**: Carreras multijugador en tiempo real
- **Slots**: Máquina tragamonedas temática crypto

### 💬 Social Features
- Chat global y por salas
- Mensajes encriptados P2P
- Sistema de notificaciones toast
- Emojis y avatares dinámicos

---

## 🛠️ Tecnologías

| Tecnología | Propósito |
|------------|-----------|
| **HTML5** | Estructura semántica |
| **TailwindCSS** | Estilizado utility-first |
| **Vanilla JavaScript** | Lógica del cliente |
| **MQTT.js** | Mensajería publish/subscribe |
| **PeerJS** | Conexiones WebRTC P2P |
| **LocalStorage** | Persistencia de datos |
| **Google Fonts** | Tipografías Inter & JetBrains Mono |

---

## 🚀 Instalación y Uso

### Opción 1: Abrir directamente
```bash
# Simplemente abre el archivo en tu navegador
open index.html
```

### Opción 2: Servidor local recomendado
```bash
# Usando Python
python -m http.server 8000

# Usando Node.js (npx)
npx serve .

# Luego abre http://localhost:8000
```

### Opción 3: Deploy gratuito
Puedes desplegar este proyecto en:
- [GitHub Pages](https://pages.github.com/)
- [Netlify Drop](https://app.netlify.com/drop)
- [Vercel](https://vercel.com/)
- [Cloudflare Pages](https://pages.cloudflare.com/)

---

## 📁 Estructura del Proyecto

```
DegenTerminal/
├── index.html          # Pantalla de inicio y gestión de salas
├── game.html           # Juego principal (trading, casino, chat)
├── video1.mp4.mp4      # Assets de video
├── video2.mp4.mp4      # Assets de video
├── video3.mp4          # Assets de video
└── README.md           # Este archivo
```

---

## 🎮 Cómo Jugar

### 1. Crear Perfil
- Abre `index.html`
- Ingresa tu nombre y selecciona un avatar
- Guarda tu perfil

### 2. Unirse o Crear Sala
- **Crear Sala**: Genera un código único y comparte con amigos
- **Unirse a Sala**: Ingresa el código de 5 dígitos

### 3. Explorar Funcionalidades
Una vez en la sala (`game.html`):
- 📊 **Trading**: Navega a la pestaña de trading
- 🎰 **Casino**: Prueba tu suerte en los juegos
- 💬 **Chat**: Conecta con otros jugadores
- ⚙️ **Settings**: Configura tu experiencia

---

## 🌐 Arquitectura Serverless

```
┌─────────────┐     MQTT      ┌──────────────┐
│   Cliente   │ ◄──────────►  │   Broker     │
│  (Browser)  │               │    MQTT      │
└─────────────┘               └──────────────┘
       │                              │
       │         WebRTC/P2P           │
       └──────────◄──────►────────────┘
                    │
             ┌─────────────┐
             │   Otros     │
             │  Clientes   │
             └─────────────┘
```

- **MQTT Broker Público**: Para descubrimiento de salas y mensajería global
- **PeerJS/WebRTC**: Para comunicación directa entre usuarios (chat, juegos)
- **LocalStorage**: Para persistencia de perfil y configuración

---

## 🔒 Seguridad y Privacidad

- ✅ No se recopilan datos personales
- ✅ Todo el almacenamiento es local (localStorage)
- ✅ Comunicaciones P2P encriptadas por WebRTC
- ✅ Sin cookies de terceros
- ✅ Código 100% client-side

---

## 🤝 Contribuir

Las contribuciones son bienvenidas! Si quieres mejorar DegenTerminal:

1. Fork el repositorio
2. Crea una rama (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

---

## 📄 Licencia

Este proyecto está bajo la licencia **MIT** - ver el archivo [LICENSE](LICENSE) para detalles.

---

## 🙏 Agradecimientos

- [TailwindCSS](https://tailwindcss.com/) por el framework CSS
- [MQTT.js](https://github.com/mqttjs/MQTT.js) por la librería de mensajería
- [PeerJS](https://peerjs.com/) por WebRTC simplificado
- La comunidad crypto/degen por la inspiración 🚀💎

---

## 📞 Contacto

¿Tienes preguntas o sugerencias? 

- 🐦 Twitter: [@tuusuario]
- 💬 Discord: [Servidor de la comunidad]
- 📧 Email: tu@email.com

---

<div align="center">

**Hecho con ❤️ y ☕ para la comunidad degen**

[⬆️ Volver arriba](#-degenterminal)

</div>
