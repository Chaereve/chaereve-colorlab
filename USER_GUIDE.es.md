# 🎨 Chaereve ColorLab — Guía de usuario

Una herramienta para ver, mezclar y exportar paletas de color de Photoshop (`.aco`) directamente en tu navegador.
**Sin instalación, sin subir datos** — todo se procesa en tu dispositivo.

---

## Índice
1. [Primeros pasos](#1-primeros-pasos)
2. [Idioma](#2-idioma)
3. [Pestaña "Ver ACO"](#3-pestaña-ver-aco)
4. [Pestaña "Mezclar colores"](#4-pestaña-mezclar-colores)
5. [Pestaña "Colores aleatorios"](#5-pestaña-colores-aleatorios)
6. [Herramientas de diseño — Crear y Analizar](#6-herramientas-de-diseño--crear-y-analizar)
7. [Procesamiento por lotes](#7-procesamiento-por-lotes)
8. [Pestaña "Degradado (.grd)"](#8-pestaña-degradado-grd)
9. [Ajustes](#9-ajustes)
10. [Exportar imagen y datos](#10-exportar-imagen-y-datos)
11. [Historial de mezclas](#11-historial-de-mezclas)
12. [Instalar como aplicación (PWA)](#12-instalar-como-aplicación-pwa)
13. [Preguntas frecuentes](#13-preguntas-frecuentes)

---

## 1. Primeros pasos

- Abre `index.html` en cualquier navegador (Chrome, Edge, Firefox, Safari…).
- Hay **7 pestañas** en la parte superior:
  - **📁 Ver ACO** — ver, editar y exportar colores de un archivo `.aco`.
  - **🎨 Mezclar colores** — mezclar varios colores en uno nuevo.
  - **🎲 Colores aleatorios** — generar colores aleatorios por miembro.
  - **🧩 Crear** — generador de paletas, degradado, extraer de imagen, preajustes.
  - **🔍 Analizar** — contraste, daltonismo, auditoría de accesibilidad, estadísticas.
  - **📦 Lotes** — combinar varios archivos `.aco`.
  - **📐 Degradado** — abrir y editar degradados `.grd` de Photoshop.
- El botón **⚙️ Ajustes** (arriba a la derecha, junto al botón de tema) abre el panel de ajustes — tema, color de acento, idioma, tamaño de fuente, sonido, efectos, borrar datos y Acerca de.

---

## 2. Idioma

- Abre **⚙️ Ajustes** (arriba a la derecha) y elige un idioma en el menú **Idioma**: Vietnamita, Inglés, 中文 (简体), 한국어, 日本語, Español.
- Toda la interfaz cambia al instante y tu elección se recuerda la próxima vez.

---

## 3. Pestaña "Ver ACO"

### Abrir un archivo
- **Arrastra y suelta** un archivo `.aco` en el área central, **o** haz clic para elegir un archivo.
- Compatible con ACO **v1 y v2**, lee **nombres de color** y los espacios RGB / HSB / CMYK / Lab / Escala de grises.

### Ver colores
- Cada color se muestra como tarjeta: **número de índice** (1, 2, 3…), muestra, nombre, HEX, RGB y su espacio de color original.
- El índice sigue el **orden del archivo ACO** para facilitar la comparación.

### Copiar códigos de color
- **Haz clic en una muestra** para copiar su código (elige el formato — HEX / RGB / HSL — en el menú de formato de la barra).
- **📋 Copiar todo** copia todo como lista HEX, variables CSS, SCSS, JSON o RGB.

### Seleccionar varios colores
- Haz clic en la **✓** de la esquina de una tarjeta para seleccionar/deseleccionar.
- **☑ Seleccionar** → Seleccionar todo / Deseleccionar / Invertir.

### Buscar y ordenar
- **🔍** busca por nombre, HEX o RGB.
- Ordena por orden original, tono, luminosidad, saturación o nombre.

### Búsqueda avanzada
Escribe tokens especiales en el cuadro de búsqueda para filtrar con precisión:
- `hue:0-60` — colores con tono en ese rango (p. ej. rojos/amarillos).
- `hue:>200` / `hue:<40` / `hue:120` — mayor, menor o tono exacto.
- `sat:>50` — saturación superior a 50; `light:40-80` — luminosidad entre 40 y 80.
- `similar:#FF0000` — colores cercanos a ese color (distancia RGB ≤ 80).
- Las palabras normales siguen funcionando; puedes combinar varios tokens.

### Editar la paleta
- **✏️ Renombrar** un color, **🗑 eliminar** uno, o **➕ añadir** un color nuevo.
- Usa **↩ Deshacer / ↪ Rehacer** (hasta 60 pasos).
- **Clic derecho** en una muestra para un menú rápido: copiar, detalles, renombrar, exportar un color como `.aco` o eliminar.
- **💾 Guardar .aco** escribe tus cambios en un nuevo archivo `.aco`.

### Compartir paleta
- Haz clic en **🔗 Compartir** (en la barra) para copiar un enlace como `…?palette=…`.
- Abrir ese enlace carga la misma paleta — sin servidor ni cuenta.

---

## 4. Pestaña "Mezclar colores"

Esta pestaña funciona **de forma independiente** — no hace falta abrir un ACO primero.

### Añadir colores a la mezcla
Dos formas:
1. **Selector de color** + **➕ Añadir este color** — elige cualquier color.
2. **📁 Abrir archivo ACO** — elige un `.aco` y aparecerá una **cuadrícula de selección**:
   - Todos los colores están seleccionados (✓) por defecto.
   - **Haz clic en una muestra** para excluir los colores que **no quieras mezclar**.
   - Botones **Seleccionar todo / Deseleccionar / Invertir**.
   - Haz clic en **➕ Añadir N colores a la mezcla** para añadir los colores elegidos.

### Reajustar colores sin volver a subir
- Haz clic en **🔁 Reajustar colores** para **reabrir la cuadrícula del ACO cargado** (sin re-subir).
- Marca/desmarca y luego "Añadir colores a la mezcla" — la app **añade los nuevos y quita los desmarcados**.

### Proporción de color
- La proporción se **iguala automáticamente** según el número de colores (p. ej. 4 colores → 25% cada uno).
- **⚖️ Igualar proporción** la restablece en cualquier momento.
- **Arrastra un control** para subir/bajar un color — el resto se recalcula hasta el 100%.

### Resultado de la mezcla
- La caja de resultado muestra el color mezclado con **HEX / RGB / HSL**, actualizado al instante.
- **📋 Copiar HEX / RGB / HSL** para copiar rápido.
- **💾 Guardar en historial** para conservar el color mezclado.

---

## 5. Pestaña "Colores aleatorios"

Genera colores aleatorios, uno por "miembro".

- **Modo:** 🌈 Totalmente aleatorio, o 🎯 Por familia de color (rojo / naranja / amarillo / verde / cian / azul / morado / rosa).
- **Número de colores** = número de miembros.
- **Sin colores duplicados** — márcalo para evitar repeticiones.
- Haz clic en **🎲 Aleatorizar** y luego **en una tarjeta** para copiarla (el número = miembro).
- **📋 Copiar todo** copia líneas `Miembro #1: #XXXXXX`.

---

## 6. Herramientas de diseño — Crear y Analizar

Las herramientas se dividen en dos pestañas: **🧩 Crear** y **🔍 Analizar**.

### Pestaña 🧩 Crear
| Herramienta | Qué hace |
|-------------|----------|
| 🧩 **Generador de paletas** | Crea una paleta armónica (complementarias, análogas, triádicas, divididas, tetrádicas) desde un color base. |
| 🌈 **Generador de degradados** | Construye un degradado CSS lineal / radial / **cónico** y copia el CSS. |
| 🖼 **Imagen → Paleta / Cuentagotas** | Haz clic en una imagen para elegir un color, extrae colores dominantes y expórtalos a `.aco`. |
| 📦 **Preajustes y plantillas** | Paletas integradas con un clic (Material, Tailwind, Colores de marca, Pastel, Tonos tierra). |

### Pestaña 🔍 Analizar
| Herramienta | Qué hace |
|-------------|----------|
| 🔳 **Comprobador de contraste** | Muestra el ratio WCAG entre texto y fondo con distintivos AA/AAA. |
| 👁 **Vista de daltonismo** | Muestra la paleta con protanopía / deuteranopía / tritanopía / escala de grises. |
| ♿ **Auditoría de accesibilidad** | Porcentaje de la paleta que aprueba AA frente a texto blanco/negro. |
| 📊 **Estadísticas de paleta** | Saturación/luminosidad media y un gráfico de distribución de tonos. |

Además, al hacer clic en **ℹ️** en cualquier tarjeta se abre un **panel de detalle** con HEX / RGB / HSL / HSV / CMYK / Lab, luminancia y contraste (clic en una fila para copiar).

---

## 7. Procesamiento por lotes

En la pestaña **📦 Lotes**:

- Haz clic en **Abrir archivos** y elige **varios archivos `.aco`** a la vez (o arrastra y suelta).
- La lista muestra cada archivo con su número de colores; quita archivos con ✕.
- **Combinar en el Visor** los fusiona en la pestaña Ver ACO (opcionalmente eliminando duplicados con la casilla "deduplicar").
- **Exportar .aco combinado** descarga un único `merged-palette.aco`.

---

## 8. Pestaña "Degradado (.grd)"

En la pestaña **📐 Degradado** puedes abrir, editar y exportar archivos de degradado de Photoshop (`.grd`, v3 y v5).

### Abrir un archivo
- Haz clic en **📁 Abrir archivo .grd** (o arrastra un `.grd` a la pestaña) para cargar sus degradados.
- Cada degradado aparece en la lista con una **vista previa en vivo** y una insignia Sólido/Ruido; haz clic en uno para editarlo.

### Editar un degradado sólido
- **Renómbralo** en el campo superior; **🗑** elimina el degradado.
- **➕ Añadir degradado** crea uno nuevo negro→blanco.
- **Paradas de color:** haz clic en una muestra para cambiar su color, arrastra **Ubicación** (0–100%) y **Punto medio** para dar forma a la transición, **✕** quita una parada, **➕ Añadir parada de color** inserta una en medio.
- **Paradas de transparencia:** lo mismo — Opacidad y Ubicación por parada.
- **Suavidad** controla la interpolación general.

### Editar un degradado de ruido
- **Semilla / 🎲 Regenerar**, **Rugosidad**, **Espacio de color**, **Añadir transparencia**, **Restringir colores**, y los valores **mínimo / máximo** por canal.
- Los degradados de ruido se recrean de forma **aproximada** (Photoshop usa su propio algoritmo interno).

### Exportar
- **📋 Copiar CSS** → una cadena `linear-gradient(…)`.
- **📐 Exportar SVG** → un degradado vectorial independiente.
- **🎨 Extraer colores → .aco** → guarda las paradas como paleta.
- **📁 Cargar en el Visor** → envía los colores a la pestaña Ver ACO.
- **💾 Guardar .grd** → escribe todos los degradados en un `.grd`.

> **Nota:** las paradas de primer plano/fondo se resuelven a colores concretos al abrir, y las paradas guardadas se escriben siempre como paradas de usuario con colores RGB.

---

## 9. Ajustes

La pestaña **⚙️ Ajustes** te permite personalizar la app. Cada elección se guarda en tu dispositivo.

| Ajuste | Qué hace |
|--------|----------|
| **Apariencia** | **Claro**, **Oscuro** o **Automático** (sigue tu sistema). El botón 🌙/☀️ de arriba a la derecha sigue alternando al instante. |
| **Color de acento** | Elige un color de resalte — recolorea el logo, la pestaña activa, los botones y los brillos. |
| **Idioma** | Elige entre 6 idiomas: Vietnamita, Inglés, 中文 (简体), 한국어, 日本語, Español. |
| **Tamaño de fuente** | Pequeño / Mediano / Grande. |
| **Efectos de sonido** | Reproduce sonidos sutiles en clics, copias y notificaciones (activar/desactivar). |
| **Efectos de movimiento** | Activa o desactiva las animaciones. |
| **Borrar datos guardados** | Elimina el historial de mezclas, idioma, tema y todas las preferencias, y recarga. |
| **Acerca de** | Una breve descripción de la app. |

---

## 10. Exportar imagen y datos

En la pestaña **Ver ACO**, selecciona los colores y haz clic en **⬇ Exportar imagen y datos**. Un diálogo te permite elegir:

- **Diseño:** franja horizontal / franja vertical / cuadrícula (con número de columnas).
- **Tamaño de celda** y **espaciado**.
- **Etiqueta:** HEX / HEX + Nombre / ninguna.
- **Fondo:** blanco o transparente.
- **Vista previa en vivo** antes de descargar.

Formatos de exportación:

| Formato | Descripción |
|---------|-------------|
| 🖼 PNG | Imagen de paleta en alta resolución |
| 📐 SVG | Vectorial, editable |
| 🎨 CSS | Variables `--color-1: #…;` |
| { } JSON | Datos de color estructurados |
| 📄 TXT | Lista HEX, uno por línea |

También puedes exportar los colores seleccionados de vuelta a **`.aco`** con el botón **💾 Exportar .aco**.

---

## 11. Historial de mezclas

- Se encuentra al final de la pestaña **Mezclar colores**.
- Cada vez que **copias** o **guardas** un color mezclado, se añade al historial automáticamente.
- **Haz clic en una muestra del historial** para copiarla de nuevo.
- **✕** quita un color; **🗑 Borrar historial** elimina todos.
- El historial se **guarda en tu navegador** (persiste al reabrir la página).

---

## 12. Instalar como aplicación (PWA)

Puedes instalar la app en escritorio y móvil:

| Plataforma | Cómo |
|------------|------|
| **Escritorio** (Chrome/Edge) | Abre la URL → botón **📲** o icono de instalación de la barra de direcciones → **Instalar** |
| **Android** (Chrome) | Abre la URL → menú **⋮** → **Añadir a pantalla de inicio** |
| **iPhone/iPad** (Safari) | Abre la URL → **Compartir** → **Añadir a pantalla de inicio** |

Una vez instalada: tiene su propio icono, se abre en una **ventana independiente** (sin barra de direcciones) y funciona **sin conexión**.

> **Requisito:** la app debe servirse por **HTTPS** (GitHub Pages / Netlify / Vercel). No se puede instalar desde un `file://` local.

---

## 13. Preguntas frecuentes

**P:** Abrí un archivo pero no veo colores?
**R:** Comprueba que sea un `.aco` válido. Algunos programas exportan ACO con otra estructura.

**P:** ¿Se suben mis datos a algún sitio?
**R:** No. La app funciona por completo en tu navegador — nada se envía por la red.

**P:** ¿Cómo funciona la mezcla?
**R:** Los colores se mezclan por proporción (media ponderada) — como mezclar pintura. Arrastra un control para "pesar" más un color.

**P:** ¿Cómo mezclo solo parte de un archivo ACO?
**R:** Haz clic en **📁 Abrir archivo ACO**, desmarca los colores que no quieras y pulsa **Añadir colores a la mezcla**.
