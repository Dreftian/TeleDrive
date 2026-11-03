<div align="center">

<img src="android/src/main/res/mipmap-xxxhdpi/ic_launcher.webp" width="120" alt="TeleDrive icon">

# TeleDrive (Español Latinoamérica)

Respalda y explora tus archivos usando un canal privado de Telegram como tu almacenamiento ilimitado en la nube.

[![Android](https://img.shields.io/badge/Android-8.0%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white)](#requisitos)
[![Windows](https://img.shields.io/badge/Windows-10%2B-0078D4?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0id2hpdGUiPjxwYXRoIGQ9Ik0wIDMuNDQ5IDkuNzUgMi4xdjkuNDUxSDB6bTEwLjk0OS0xLjUwMUwyNCAwdjExLjRIMTAuOTQ5ek0wIDEyLjZoOS43NXY5LjQ1MUwwIDIwLjY5OXptMTAuOTQ5IDBIMjRWMjRsLTEzLjA1MS0xLjgwMXoiLz48L3N2Zz4%3D)](#requisitos)
[![Linux](https://img.shields.io/badge/Linux-x86__64-FCC624?style=for-the-badge&logo=linux&logoColor=black)](#requisitos)
[![macOS](https://img.shields.io/badge/macOS-Apple%20Silicon-111111?style=for-the-badge&logo=apple&logoColor=white)](#requisitos)
[![Kotlin](https://img.shields.io/badge/Kotlin-2.4-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Compose](https://img.shields.io/badge/Compose%20Multiplatform-Material%203-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)](https://www.jetbrains.com/compose-multiplatform/)
[![Release](https://img.shields.io/github/v/release/Dreftian/TeleDrive?style=for-the-badge&logo=github&logoColor=white&color=1F883D)](https://github.com/Dreftian/TeleDrive/releases)
[![License](https://img.shields.io/badge/license-Apache%202.0-6750A4?style=for-the-badge&logo=apache&logoColor=white)](LICENSE)
</div>

---

## Contenido

- [Acerca de](#acerca-de) · [Funciones principales](#funciones-principales) · [Capturas de pantalla](#capturas-de-pantalla)
- **Instalación**: [Android](#android) · [Windows](#windows) · [Linux (x86_64)](#linux-x86_64) · [macOS (Apple Silicon)](#macos-apple-silicon)
- [Requisitos](#requisitos) · [Primeros pasos](#primeros-pasos)
- [Traer archivos existentes](#traer-archivos-existentes) · [Consejos y detalles técnicos](#consejos-y-detalles-técnicos)
- [Arquitectura](#arquitectura) · [Modelo de seguridad](#modelo-de-seguridad) · [Licencia](#licencia)

---

## Acerca de

**TeleDrive** guarda tus archivos directamente en un canal privado de Telegram de tu propia cuenta. No existen servidores externos ni intermediarios: tú tienes el control total de tus datos. La aplicación mantiene una indexación local ultrarrápida que permite explorar, buscar y organizar archivos incluso sin conexión a internet.

Una sola base de código con **Compose Multiplatform** compila las aplicaciones para Android, Windows, Linux x86_64 y macOS. Todas comparten el mismo motor de almacenamiento, cifrado local, gestor de transferencias y explorador de archivos.

## Funciones principales

- **Respaldo automático:** Tus fotos y carpetas seleccionadas se suben solas en Android con horarios, reglas de Wi-Fi, nivel de batería y patrones de exclusión.
- **Sin límite de almacenamiento total:** Tu cuenta de Telegram es tu disco duro virtual.
- **Soporte completo en Español (Latinoamérica):** Interfaz adaptada con detección automática de tu idioma regional.
- **Cifrado de extremo a extremo (E2E):** Cifrado AES-256-GCM opcional para proteger el contenido de los archivos, nombres, pies de foto y carpetas.
- **Gestión completa de archivos:** Carpetas, favoritos, archivos ocultos, archivados, papelera y acciones por lote.
- **Streaming integrado:** Reproduce música y videos directamente desde la nube de Telegram al instante con soporte para archivos cifrados.
- **Vistas previas integradas:** Visualiza imágenes, documentos PDF, textos y contenidos de archivos ZIP sin salir de la app.
- **Múltiples unidades:** Organiza canales separados para temas personales, trabajo o fotos dentro de tu misma cuenta.
- **Cola de transferencias inteligente:** Sube y descarga en paralelo con pausa y reanudación automática tras reinicios.
- **Seguridad en tu dispositivo:** Bloqueo biométrico (huella/rostro), bloqueo de capturas de pantalla y caché local protegida.

## Capturas de pantalla

<div align="center">
<img src=".github/screenshots/1.png" width="24%" alt="Inicio"> <img src=".github/screenshots/2.png" width="24%" alt="Archivos"> <img src=".github/screenshots/3.png" width="24%" alt="Galería"> <img src=".github/screenshots/4.png" width="24%" alt="Ajustes">
</div>

---

## Instalación

### Android
Descarga el archivo APK directamente desde la [sección de Releases](https://github.com/Dreftian/TeleDrive/releases):
* `TeleDrive-Android-v1.5.0-universal.apk` (Compatible con todos los celulares modernos).

Instálalo en tu celular activando la opción de permitir orígenes desconocidos si tu navegador te lo solicita.

### Windows
Descarga el instalador `.msi` desde la [sección de Releases](https://github.com/Dreftian/TeleDrive/releases):
* `TeleDrive-Windows-v1.5.0.msi`

Ejecuta el instalador. No requiere permisos de administrador, añade accesos directos al menú Inicio y a tu escritorio. Tu sesión y configuraciones se guardan de forma segura en `%APPDATA%\TeleDrive`.

### Linux (x86_64)
Disponible en paquetes AppImage y `.deb` desde Releases.

### macOS (Apple Silicon)
Descarga el archivo `.dmg` desde Releases y arrastra TeleDrive a tu carpeta de Aplicaciones.

---

## Requisitos

- **Android 8.0+**, **Windows 10+ (64 bits)**, **Linux x86_64** o **macOS (Apple Silicon)**.
- Una cuenta activa de Telegram.
- Tus credenciales de la API de Telegram (gratuitas en [my.telegram.org](https://my.telegram.org) bajo *API development tools*).

### Cómo obtener tus credenciales:
1. Inicia sesión con tu número de teléfono en [my.telegram.org](https://my.telegram.org).
2. Haz clic en **API development tools**.
3. Ingresa un nombre para tu app (ejemplo: `TeleDrivePersonal`) y un nombre corto.
4. Obtendrás tu **`api_id`** y tu **`api_hash`**. Estos datos se introducen una única vez al abrir la aplicación y se guardan cifrados en tu dispositivo.

---

## Primeros pasos (Desarrollo local)

Si deseas clonar y compilar el proyecto por tu cuenta:

```bash
git clone https://github.com/Dreftian/TeleDrive.git
cd TeleDrive

# Compilar para Android
./gradlew :android:installDebug

# Compilar y ejecutar en Windows / Linux Escritorio
./gradlew :desktop:run
```

---

## Traer archivos existentes a tu unidad

¿Ya tienes archivos guardados en chats o en Mensajes guardados de Telegram? Reenvíalos al canal privado creado por TeleDrive y aparecerán en tu explorador de archivos en la siguiente sincronización, sin tener que gastar datos volviéndolos a subir.

---

## Modelo de seguridad

| Capa | Qué protege |
| --- | --- |
| **En el dispositivo** | Bases de datos de Room y TDLib protegidas con clave maestra de la plataforma (Android Keystore, Windows DPAPI). Caché y miniaturas cifradas con AES-GCM. |
| **En Telegram** | Si activas el cifrado, el canal solo almacena bytes cifrados ininteligibles, nombres en código y carpetas protegidas. |
| **Respaldo de clave** | La clave de cifrado se respalda en tu canal sellada mediante tu frase de contraseña personal (PBKDF2, 310k iteraciones). |

---

## Licencia

Este proyecto está bajo la licencia [Apache License 2.0](LICENSE).

---

<div align="center">
<sub>TeleDrive es un proyecto independiente, sin afiliación oficial con Telegram ni respaldo de Telegram.</sub>
</div>
