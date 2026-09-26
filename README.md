# 🎸 Reparto Banda

Aplicación web offline para gestionar el **reparto de dinero** entre los integrantes de una banda de rock después de cada evento.

![Estado](https://img.shields.io/badge/estado-activo-6C5CE7)
![Plataforma](https://img.shields.io/badge/plataforma-Android-19C7D8)
![Offline](https://img.shields.io/badge/modo-offline-22C55E)

---

## 📱 ¿Qué hace la app?

**Reparto Banda** permite registrar eventos, calcular el reparto entre los músicos y generar comprobantes imprimibles. Funciona **100% offline**, sin servidor, sin internet, sin Firebase.

---

## ✨ Características principales

- 🎤 **Gestión de integrantes** — Agregar, editar rol, activar/desactivar y eliminar.
- 🎸 **Reparto automático** — Dos modalidades de cálculo:
  - **Modalidad A:** Total directo → reparto automático entre integrantes activos.
  - **Modalidad B:** Valores por integrante → exactos, sin redistribuir.
- 🎚️ **Sonido** — Descuento automático antes del reparto (Sin sonido, Pequeño, Mediano, Grande).
- 📸 **Foto del evento** — Desde cámara o galería, con lectura de fecha EXIF.
- 📜 **Historial** — Todos los eventos guardados, con detalle completo.
- 🧾 **Comprobantes** — Uno por integrante + uno independiente para sonido, con marca de agua personalizada.
- 🖨️ **Impresión / PDF** — Guarda los comprobantes como PDF desde el navegador.
- 🎨 **Personalización** — Nombre de banda y colores configurables.
- 💾 **Guardado local** — Los datos se conservan aunque cierres la app.

---

## 🎨 Estética

- Estilo **oscuro, rockero, musical e intenso**.
- Paleta de colores por defecto:
  - **Primario:** `#6C5CE7` (morado)
  - **Secundario:** `#19C7D8` (cian)
  - **Fondo:** `#070B14`
  - **Superficie:** `#0E1726`
- Todos los colores son **personalizables** desde la pantalla de Configuración.

---

## 🧭 Navegación

| Sección | Descripción |
|---|---|
| 🏠 **Inicio** | Muestra los últimos 3 eventos y acceso al historial completo. |
| ➕ **Nuevo evento** | Registra un reparto con nombre, fecha, total, sonido y foto. |
| 👥 **Integrantes** | Gestiona los músicos de la banda. |
| 📜 **Historial** | Todos los eventos guardados con su detalle. |
| ⚙️ **Configuración** | Nombre de banda, colores y reinicio de la app. |

---

## 👥 Integrantes iniciales

| Nombre | Rol |
|---|---|
| Alex | Baterista |
| Cristian | Vocalista |
| Esteban | Guitarrista |
| John | Músico |
| Leandro | Guitarrista |
| Leonardo | Bajista |

> Todos los roles son **editables** y los integrantes se pueden **activar o desactivar** en cualquier momento.

---

## 💰 Modalidades de reparto

### Modalidad A — Total directo
1. Ingresas el **total recibido** del evento.
2. Se descuenta primero el **sonido** (si aplica).
3. El disponible se reparte automáticamente entre los integrantes activos.
4. Se ajustan diferencias de redondeo para que los pagos coincidan exactamente con el dinero disponible.

### Modalidad B — Definir total por integrantes
1. Aparecen los integrantes activos.
2. Ingresas **manualmente** cuánto le corresponde a cada uno.
3. Los valores se mantienen **exactamente** como los escribiste.
4. **No se redistribuye** ni se recalcula nada.
5. El total del evento es la suma de los valores asignados + el sonido (si aplica).

---

## 🎚️ Opciones de sonido

| Opción | Valor |
|---|---|
| Sin sonido | $0 |
| Sonido Pequeño | $400.000 COP |
| Sonido Mediano | $650.000 COP |
| Sonido Grande | $800.000 COP |

- En **Modalidad A**, el sonido se descuenta del total antes del reparto.
- En **Modalidad B**, el sonido va aparte y no altera los valores individuales.
- Siempre genera su **propio comprobante**.

---

## 💾 Almacenamiento

- **localStorage** → integrantes, eventos, configuración, colores y nombre de banda.
- **IndexedDB** → fotos de los eventos sin comprimir (máxima capacidad).
- **Sin servidor, sin internet, sin Firebase.**

> 📌 Los eventos conservan la información del momento en que fueron creados. Si luego cambias un rol o desactivas a alguien, los eventos pasados **no se alteran**.

---

## 🧾 Comprobantes

- Un comprobante por cada integrante con pago.
- Un comprobante independiente para el sonido (si aplica).
- Muestra: **Reparto Banda**, nombre de la banda, evento, fecha, integrante, rol y valor.
- **Marca de agua** con el nombre de la banda.
- La **foto del evento** puede usarse como fondo visual.
- Se pueden **imprimir** o **guardar como PDF**.

---

## 🛠️ Tecnología

- HTML5 + CSS3 + JavaScript vanilla.
- Sin frameworks, sin dependencias externas.
- Un **solo archivo `.html`** autosuficiente.
- Preparada para conversión a **APK** con PakePlus.

---

## 🚀 Cómo usarla

### Opción 1 — Navegador
1. Abre el archivo `reparto-banda.html` en Chrome (Android).
2. Menú (⋮) → **Agregar a pantalla de inicio**.
3. Listo, queda como acceso directo.

### Opción 2 — APK
1. Sigue la guía de conversión con **PakePlus**.
2. Instala el APK generado en tu dispositivo.
3. Listo, funciona como app nativa.

---

## 📋 Reglas de desarrollo

- El diseño base aprobado **no se rediseña** sin autorización.
- Cada cambio se limita a la característica solicitada.
- No se agregan funciones no pedidas.
- No se eliminan funciones existentes.
- Si se modifica una cosa, **todo lo demás permanece igual**.

---

## 👤 Autor

**John Gallego**
© Impulsado por IA

---

## 📄 Licencia

Uso personal. Todos los derechos reservados.
