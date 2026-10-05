# 📱 App Móvil — Simulador de celular con EasyFit

Aplicación **Android** desarrollada con **Kotlin** y **Jetpack Compose** que simula la interfaz de un smartphone (pantalla de bloqueo, pantalla de inicio y apps) e incluye **EasyFit**, una app de entrenamiento personal con rutinas, progreso y pago de membresía.

> Proyecto académico — Universidad Tecnológica de Puebla, Desarrollo de Software Multiplataforma.

---

## ✨ Funcionalidades

### Sistema del celular
| Módulo | Descripción |
|---|---|
| 🔒 Pantalla de bloqueo | Hora y fecha en tiempo real, desbloqueo al tocar |
| 🏠 Pantalla de inicio | Cuadrícula de apps con navegación entre pantallas |
| 📷 Cámara | Vista previa con **CameraX** y solicitud de permiso en tiempo de ejecución |
| 🧮 Calculadora | Operaciones aritméticas con evaluación de expresiones |
| 📞 Teléfono | Teclado de marcado |
| 🖼️ Galería | Cuadrícula de imágenes cargadas con **Coil** |
| 📝 Notas | Bloc de notas para añadir y ver notas |
| ⛅ Clima | Pantalla de pronóstico con datos de ejemplo |
| 🌐 Accesos directos | Play Store, Classroom, YouTube, WhatsApp, Instagram y Facebook abren su sitio web en el navegador |

### 💪 EasyFit — tu entrenador personal
- **Bienvenida y onboarding:** elige tu objetivo (ganar músculo, bajar peso, resistencia, etc.) y tu nivel.
- **Inicio:** racha de entrenamiento, meta diaria, selector de energía y parte del cuerpo a entrenar, **generador de rutina** y cronómetro.
- **Rutinas:** lista de ejercicios con series, repeticiones y calorías.
- **Progreso:** pasos de la semana, racha y logros desbloqueados.
- **Membresía:** planes Mensual / Trimestral / Anual, pago con **tarjeta, transferencia u OXXO**, historial de pagos y aviso de vencimiento.

> Los datos (clima, pasos, historial de pagos, referencias bancarias) son de ejemplo y el pago es una simulación; la app no procesa cobros reales.

## 🛠️ Stack

- **Lenguaje:** Kotlin 2.2
- **UI:** Jetpack Compose + Material 3
- **Navegación:** Navigation Compose
- **Cámara:** CameraX 1.3
- **Imágenes:** Coil
- **Build:** Gradle 9.4.1, Android Gradle Plugin 9.2.1
- **SDK:** `minSdk 31` · `targetSdk / compileSdk 36` · JDK 11

## 📁 Estructura

```
AppMovil/
├── app/
│   └── src/main/
│       ├── AndroidManifest.xml
│       ├── java/com/example/p1_navegacion/
│       │   ├── MainActivity.kt      # navegación y todas las pantallas
│       │   └── ui/theme/            # colores, tipografía y tema
│       └── res/                     # íconos, logos y recursos
├── gradle/libs.versions.toml        # catálogo de versiones
└── README.md
```

## 🚀 Cómo ejecutarlo

### Requisitos
- [Android Studio](https://developer.android.com/studio) reciente (con soporte para AGP 9.x)
- Un emulador o dispositivo con **Android 12 (API 31) o superior**
- Conexión a internet (la galería carga imágenes en línea)

### Pasos

```bash
git clone https://github.com/<tu-usuario>/AppMovil.git
```

1. Abre la carpeta en Android Studio y espera la sincronización de Gradle.
2. Selecciona un emulador o conecta tu teléfono.
3. Presiona **Run ▶**.
4. En el emulador, otorga el permiso de cámara cuando lo solicite.

## 🔐 Permisos

- `CAMERA` — para la app de cámara
- `INTERNET` — para la galería y los accesos directos web

## 👤 Autor

**Angel Ramos Salazar**
Universidad Tecnológica de Puebla — Desarrollo de Software Multiplataforma
