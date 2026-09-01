# 🎨 Chaereve ColorLab

<p align="center">
  <a href="README.md"><img alt="English" src="https://img.shields.io/badge/English-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.vi.md"><img alt="Tiếng Việt" src="https://img.shields.io/badge/Ti%E1%BA%BFng%20Vi%E1%BB%87t-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.zh.md"><img alt="中文" src="https://img.shields.io/badge/%E4%B8%AD%E6%96%87-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ko.md"><img alt="한국어" src="https://img.shields.io/badge/%ED%95%9C%EA%B5%AD%EC%96%B4-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ja.md"><img alt="日本語" src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.es.md"><img alt="Español" src="https://img.shields.io/badge/Espa%C3%B1ol-22d3ee?style=for-the-badge"></a>
</p>

Una herramienta para **ver, mezclar y exportar paletas de color de Photoshop (`.aco`)** que funciona **completamente en tu navegador**. Sin instalación, sin registro, sin subir datos.

> Todo se procesa **100% en local** en tu dispositivo.

**🌐 Interfaz multilingüe (6 idiomas):** Vietnamita, Inglés, 中文 (简体), 한국어, 日本語, Español — cámbialo en **⚙️ Ajustes**.

---

## ✨ Funciones

### 📁 Ver ACO
- Arrastra y suelta (o haz clic) un archivo `.aco` para abrirlo.
- Compatible con **ACO v1 y v2**, lee **nombres de color** y los espacios RGB / HSB / CMYK / Lab / Escala de grises.
- Cada color muestra un **número de índice**, nombre, HEX, RGB y su espacio de color original.
- **Busca** por nombre/HEX/RGB y **ordena** por tono, luminosidad, saturación o nombre.
- **Búsqueda avanzada**: filtra por rangos con `hue:0-60`, `sat:>50`, `light:40-80`, o encuentra colores cercanos con `similar:#FF0000`.

### ✏️ Editar paleta (en el sitio)
- **Renombra** colores (✏️), **borra** (🗑) o **añade** colores nuevos — y **guarda de nuevo en .aco**.
- **Deshacer / rehacer** completo (hasta 60 pasos).
- **Clic derecho** en cualquier muestra para un menú rápido (copiar / detalles / renombrar / exportar / eliminar).

### 📋 Copiar
- Haz clic en una muestra para copiar su código (**HEX / RGB / HSL** — seleccionable).
- **Copiar todo** como: lista HEX, variables CSS, SCSS, JSON, RGB, **configuración de Tailwind** o **Styled Components**.

### 🎨 Mezclar colores (independiente — no requiere ACO)
- Añade colores con el **selector de color** o **abre un archivo ACO** directamente en esta pestaña.
- Una cuadrícula de selección te permite **excluir los colores que no quieres mezclar** con un clic.
- **Reajusta tu selección** sin volver a subir el archivo.
- Las proporciones **se igualan automáticamente** según el número de colores; arrastra un control para ajustar cada uno.
- El **historial de mezclas** se guarda automáticamente; haz clic para copiar de nuevo.

### 🎲 Colores aleatorios (por miembro)
- Genera 1–100 colores aleatorios para cada "miembro", ya sea totalmente aleatorios o dentro de una familia de color elegida (rojo / naranja / amarillo / verde / cian / azul / morado / rosa), con modo opcional sin duplicados.

### 🛠 Herramientas de diseño
Divididas en dos pestañas — **🧩 Crear** y **🔍 Analizar**:
- **Generador de paletas** — complementarias / análogas / triádicas / divididas / tetrádicas.
- **Generador de degradados** — degradado CSS lineal / radial / **cónico** con copiado al portapapeles.
- **Imagen → Paleta / Cuentagotas** — haz clic en una imagen para elegir un color, extrae colores dominantes y **expórtalos directo a .aco**.
- **Preajustes y plantillas** — paletas integradas de Material Design, Tailwind, Colores de marca, Pastel y Tonos tierra.
- **Comprobador de contraste** — ratio WCAG con distintivos AA/AAA.
- **Auditoría de accesibilidad** — % de la paleta que aprueba AA frente a texto blanco/negro.
- **Estadísticas de paleta** — saturación/luminosidad media y un gráfico de distribución de tonos.
- **Vista previa de daltonismo** — protanopía / deuteranopía / tritanopía / escala de grises.
- **Panel de detalle de color** — HEX / RGB / HSL / HSV / CMYK / Lab, luminancia, contraste.
- **Detector de duplicados** y **buscador de colores similares**.

### 📦 Procesamiento por lotes
- Abre **varios archivos .aco** a la vez y **combínalos** en una sola paleta (con deduplicación opcional) o **exporta un .aco combinado**.

### 🔗 Compartir paleta
- Genera un **enlace compartible** (`?palette=...`) que codifica la paleta actual — cualquiera que abra el enlace ve los mismos colores, sin servidor.

### 📐 Degradado (.grd)
- Abre **archivos de degradado de Photoshop** (`.grd`, **v3 y v5**) — degradados sólidos y de ruido.
- **Previsualiza** cada degradado y **edita** paradas de color, paradas de transparencia, punto medio, suavidad y parámetros de ruido (semilla, rugosidad, mín/máx).
- **Añade / elimina degradados** y paradas, y **guarda de nuevo en `.grd`**.
- Exporta un degradado como **CSS `linear-gradient`** o **SVG**, y **extrae sus colores a `.aco`** o directamente al Visor.

### ⬇ Exportar
- **PNG / SVG / CSS / JSON / TXT** con opciones de diseño, tamaño, etiqueta y fondo (incluido transparente).
- **Exportar .aco** (v2, con nombres de color) de los colores seleccionados.

### 🌙 Interfaz — glassmorphism
- Diseño **glassmorphism**: paneles de cristal esmerilado, desenfoque suave y luz ambiental — pulido como macOS/iOS.
- Tema **oscuro / claro / automático** (sigue tu sistema por defecto).
- **6 idiomas**: Vietnamita, Inglés, 中文 (简体), 한국어, 日本語, Español — cambiable en **⚙️ Ajustes**.
- Animaciones fluidas y diseño móvil primero (navegación inferior, hojas inferiores, objetivos táctiles grandes).

### ⚙️ Ajustes
- **Apariencia** — tema claro, oscuro o automático.
- **Color de acento** — recolorea toda la interfaz (logo, pestañas, botones, brillo).
- **Idioma** y **tamaño de fuente** (pequeño / mediano / grande).
- **Efectos de sonido** — sonidos sutiles en clics, copias y notificaciones (activar/desactivar).
- **Efectos de movimiento** activar/desactivar, **borrar datos guardados** y una caja **Acerca de**.

### 📲 Instalar como aplicación (PWA)
- Instalable en **escritorio (Windows/macOS/Linux)** y **móvil (Android/iOS)**.
- Tiene su propio icono, se abre en una ventana independiente y funciona **sin conexión**.

### 🖥 Versión de escritorio (Windows / macOS / Linux)
- Empaquetada como **aplicación de escritorio nativa** con Electron — consulta la carpeta `electron-app/`.
- Genera instaladores para cada sistema: **Windows** (`.exe` instalador + portable), **macOS** (`.dmg`) y **Linux** (`.AppImage`).
- El logo de la aplicación es **redondo**, como las apps modernas.

---

## 🚀 Uso

### En escritorio / móvil
Abre `index.html` en cualquier navegador (doble clic) o visita la URL desplegada.

### Flujo rápido
1. Abre la pestaña **📁 Ver ACO** → arrastra y suelta un archivo `.aco`.
2. Haz clic en un color para copiarlo, o marca varios colores para exportarlos.
3. Abre la pestaña **🎨 Mezclar colores** → añade colores → mira el resultado al instante.
4. Haz clic en **⬇ Exportar imagen y datos** para descargar la paleta.
5. Abre la pestaña **📐 Degradado** → suelta un archivo `.grd` para ver y editar degradados de Photoshop.
6. Abre **⚙️ Ajustes** para cambiar tema, color de acento, idioma y tamaño de fuente.

---

## 🌐 Idiomas (6)

Abre **⚙️ Ajustes** (el botón de engranaje, arriba a la derecha) y elige un idioma en el menú **Idioma**: Vietnamita, Inglés, 中文 (简体), 한국어, 日本語, Español. Toda la interfaz cambia al instante y tu elección se recuerda entre sesiones.

**El README y la Guía de usuario de este repositorio están disponibles en los 6 idiomas:**

| Idioma | README | Guía de usuario |
|--------|--------|-----------------|
| 🇬🇧 English | [README.md](README.md) | [USER_GUIDE.md](USER_GUIDE.md) |
| 🇻🇳 Tiếng Việt | [README.vi.md](README.vi.md) | [USER_GUIDE.vi.md](USER_GUIDE.vi.md) |
| 🇨🇳 中文 (简体) | [README.zh.md](README.zh.md) | [USER_GUIDE.zh.md](USER_GUIDE.zh.md) |
| 🇰🇷 한국어 | [README.ko.md](README.ko.md) | [USER_GUIDE.ko.md](USER_GUIDE.ko.md) |
| 🇯🇵 日本語 | [README.ja.md](README.ja.md) | [USER_GUIDE.ja.md](USER_GUIDE.ja.md) |
| 🇪🇸 Español | [README.es.md](README.es.md) | [USER_GUIDE.es.md](USER_GUIDE.es.md) |

---

## 📲 Instalar como aplicación (PWA)

Una vez desplegada (por HTTPS), puedes instalarla como una aplicación real:

| Plataforma | Cómo |
|------------|------|
| **Escritorio** (Chrome/Edge) | Abre la URL → botón **📲** o el icono de instalación en la barra de direcciones → **Instalar** |
| **Android** (Chrome) | Abre la URL → menú **⋮** → **Añadir a pantalla de inicio** |
| **iPhone/iPad** (Safari) | Abre la URL → botón **Compartir** → **Añadir a pantalla de inicio** |

> **Importante:** las PWA deben servirse por **HTTPS** (GitHub Pages, Netlify y Vercel lo hacen). No puedes instalar al abrir un `file://` directamente.

---

## 🌐 Botones de cambio de idioma

Cada `README.<código>.md` empieza con una **barra de botones de cambio de idioma** (los botones de arriba). Para añadirla a un README nuevo, pega esto al principio:

```markdown
<p align="center">
  <a href="README.md"><img alt="English" src="https://img.shields.io/badge/English-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.vi.md"><img alt="Tiếng Việt" src="https://img.shields.io/badge/Ti%E1%BA%BFng%20Vi%E1%BB%87t-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.zh.md"><img alt="中文" src="https://img.shields.io/badge/%E4%B8%AD%E6%96%87-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ko.md"><img alt="한국어" src="https://img.shields.io/badge/%ED%95%9C%EA%B5%AD%EC%96%B4-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.ja.md"><img alt="日本語" src="https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.es.md"><img alt="Español" src="https://img.shields.io/badge/Espa%C3%B1ol-1a3fd6?style=for-the-badge"></a>
</p>
```

Usa un color distinto (p. ej. `22d3ee`) para el botón del idioma **actual**.

---

## ❓ Preguntas frecuentes

**¿Se suben mis datos a algún sitio?**
No. Todo se ejecuta en tu navegador — nada se envía por la red.

**¿El archivo se abre pero no aparecen colores?**
Comprueba que sea un archivo `.aco` válido. Algunas aplicaciones exportan ACO con una estructura no estándar.

**¿Cómo funciona la mezcla de colores?**
La app mezcla colores por proporción (media ponderada) — como mezclar pintura. Arrastra un control para hacer un color "más pesado".

**¿Cómo mezclo solo algunos colores de un archivo?**
Abre el ACO en la pestaña **Mezclar colores** → haz clic para deseleccionar los colores que no quieras → pulsa **Añadir colores a la mezcla**.

---

## 📚 Guías

Guía de usuario (los 6 idiomas):
- 🇬🇧 [USER_GUIDE.md](USER_GUIDE.md) · 🇻🇳 [USER_GUIDE.vi.md](USER_GUIDE.vi.md) · 🇨🇳 [USER_GUIDE.zh.md](USER_GUIDE.zh.md) · 🇰🇷 [USER_GUIDE.ko.md](USER_GUIDE.ko.md) · 🇯🇵 [USER_GUIDE.ja.md](USER_GUIDE.ja.md) · 🇪🇸 [USER_GUIDE.es.md](USER_GUIDE.es.md)

Despliegue y compilación (paso a paso): [HUONG_DAN_TUNG_BUOC.md](HUONG_DAN_TUNG_BUOC.md)

---

## 📄 Licencia

Libre para uso personal y comercial.
