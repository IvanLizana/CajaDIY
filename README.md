<div align="center">
  <img src="https://img.shields.io/badge/ASTROREMOTO-Precision_Software-blue?style=for-the-badge" alt="Astroremoto" />
  <br>
  <p>
    <strong>
      <a href="#-español-documentación-oficial">🇪🇸 ESPAÑOL (LEER PRIMERO)</a>
      &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
      <a href="#-english-official-documentation">🇬🇧 ENGLISH (READ BELOW)</a>
    </strong>
  </p>
</div>

---

<a name="-español-documentación-oficial"></a>
# 📦 CajaDIY - Generador de Cajas Paramétricas (v0.4.0)

![Versión](https://img.shields.io/badge/Versión-v0.4.0-gold)
![Plataforma](https://img.shields.io/badge/Plataforma-Windows_10%2F11_x64-blue)
![Motor](https://img.shields.io/badge/Motor-OpenSCAD-cyan)
![Idiomas](https://img.shields.io/badge/Idiomas-ES_EN_PL_DE_FR-orange)
![Licencia](https://img.shields.io/badge/Licencia-MIT-green)

<div align="center">
  <h3>Cajas a medida para tus proyectos de electrónica, listas para imprimir en 3D</h3>
  <p><em>Le das las medidas de tu placa y tus conectores; CajaDIY te entrega el STL de la caja y de la tapa.</em></p>

  <a href="https://github.com/IvanLizana/CajaDIY/releases/latest">
    <img src="https://img.shields.io/badge/DESCARGAR_INSTALADOR_v0.4.0-Clic_Aquí-success?style=for-the-badge&logo=windows&logoColor=white" alt="Descargar Ahora" />
  </a>
  &nbsp;
  <a href="Manual_de_usuario_CajaDIY.pdf">
    <img src="https://img.shields.io/badge/MANUAL_DE_USUARIO-PDF-informational?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Manual de usuario" />
  </a>
</div>

> # ⚠️ REQUISITO CRÍTICO DE USO
> **PARA QUE ESTE SOFTWARE FUNCIONE CORRECTAMENTE:**
> 1.  **OpenSCAD:** debe estar instalado (gratuito, **no viene incluido**). Descárguelo de **[openscad.org/downloads](https://openscad.org/downloads.html)** e instálelo en su carpeta habitual (`C:\Program Files\OpenSCAD`).
>     * *CajaDIY lo usa para generar los STL y la vista previa 3D.*
>     * *La versión de desarrollo (**Development Snapshot**) genera los STL mucho más rápido.*
> 2.  **Sistema:** Windows 10 u 11 de **64 bits**.

---

## 📄 Descripción General

**CajaDIY** es un generador de cajas paramétricas para quienes arman proyectos con **ESP32, Arduino, Raspberry Pi** o cualquier placa. Usted define las medidas interiores, el tipo de tapa, los postes de la placa, los agujeros para los conectores y hasta sus logos; el programa dibuja la caja, **avisa de los choques antes de imprimir** (puertos contra pestañas, postes contra tabiques, tapa contra soportes…) y exporta la caja y la tapa en STL, listas para el laminador.

Todo se diseña pensando en la impresora: piezas que se imprimen **sin material de soporte**, holguras ajustables y perfiles que se guardan y se vuelven a abrir.

---

## ⚡ Novedades en v0.4.0

### 1. Soportes en Cuña 📐
Rieles pegados a las paredes interiores para apoyar una placa o una bandeja.
* Cara superior horizontal y cara inferior inclinada (**38–52°**, 45° por defecto): **se imprimen sin soporte**.
* Varios por pared y en las cuatro paredes; posición medida **desde la pared que usted elija**; se unen en las esquinas.

### 2. Bisagra Reforzada 🔩
* La tapa **ya no roza al abrir** (antes se trababa y podía partirse en la unión del nudillo central).
* Nudillo más grueso, **holgura propia de la bisagra** (0,4 mm, ajustable), muesca en la pared y agujero del pasador **en forma de gota** para imprimir acostado.
* La cara exterior de la tapa sigue siendo **plana**, cilindro incluido.

### 3. Tabiques con Largo Propio 🧱
* Ya no van siempre de pared a pared: posición e inicio **desde la pared que usted elija**, largo limitado al interior.
* Se pueden **cruzar aunque tengan alturas distintas**.

### 4. Esquinas a 90° por Defecto ⬛
* Esquinas exteriores e interiores en ángulo recto; cada radio se puede subir por separado.

---

## 📜 Historial de Versiones

### [v0.2.0] - Primera versión publicada
* 8 tipos de tapa, pestañas de montaje con amarras, postes con plantillas de placas.
* Agujeros en las 6 caras con catálogo de conectores.
* **Logos e imágenes en las caras** (relieve, grabado o calado), varios por cara y con rotación libre.
* Vista 2D con avisos de colisiones, vista previa en OpenSCAD y exportación de STL por separado.

---

## 🔬 Funcionalidades Core

* **8 Tapas:** con bisagra, a presión con broches, por fricción, con tornillos (exterior o embutida), con imanes, corredera y campana.
* **Pestañas de Montaje:** 2 o 4, con avellanado y puentes para amarras plásticas.
* **Postes para la Placa:** plantillas para ESP32 DevKit, Arduino UNO y Raspberry Pi 4/5.
* **Puertos en las 6 Caras:** rectangulares con radio o circulares, con catálogo (USB-C, micro-USB, USB-A, RJ45, jack, prensaestopas PG7 y M12, borneras, OLED, LED).
* **Logos e Imágenes:** convierte un PNG o JPG en relieve, grabado o calado, y lo escala solo a la cara.
* **Lienzo 2D:** planta, frontal, lateral e isométrica, con cotas, zoom y avisos en la barra de estado.
* **Perfiles:** cada caja se guarda en un archivo `.json` para volver a abrirla o compartirla.
* **Multi-idioma:** español, English, Polski, Deutsch y Français, cambiando en vivo.

---

## 📥 Instrucciones de Instalación y Uso

El instalador **no pide permisos de administrador** y se instala en su carpeta de usuario. Si ya tiene una versión anterior, se actualiza encima y conserva su configuración y sus perfiles.

1.  **OpenSCAD:** instálelo primero desde **[openscad.org/downloads](https://openscad.org/downloads.html)**.
2.  **Descargar:** vaya a **[Releases (Lanzamientos)](../../releases/latest)** y baje `CajaDIY_Setup_0.4.0.exe`.
3.  **Instalar:** ejecútelo y siga el asistente. Si no encuentra OpenSCAD, lo avisa y ofrece abrir su página de descarga.
4.  **Diseñar:** abra CajaDIY, elija una plantilla de placa, ajuste medidas, tapa y puertos, y mire los avisos en la barra de estado.
5.  **Exportar:** pulse **"Exportar Caja y Tapa"** y abra los STL en su laminador (Cura, PrusaSlicer, Bambu Studio…).

> **⚠️ Nota sobre Windows Defender / SmartScreen:**
> Al ser software gratuito desarrollado por un **aficionado** (sin certificado de firma de código), Windows puede mostrar una advertencia de "Editor Desconocido".
> * Esto es normal. Haga clic en **"Más información"** y luego en **"Ejecutar de todas formas"**.
> * Puede verificar el instalador con el **SHA-256** publicado en las notas de cada versión.

---

## 🤝 Comunidad

* **¿Encontró un fallo o tiene una idea?** Abra un **[Issue](../../issues/new/choose)** (adjunte el perfil `.json` de su caja si el problema es con una caja concreta).
* Antes de participar, lea el **[Código de Conducta](CODE_OF_CONDUCT.md)** y **[Cómo Colaborar](CONTRIBUTING.md)**.
* Problemas de seguridad: en privado, según **[SECURITY.md](SECURITY.md)**. Accesibilidad: **[ACCESSIBILITY.md](ACCESSIBILITY.md)**.

---
---

<a name="-english-official-documentation"></a>
# 📦 CajaDIY - Parametric Enclosure Generator (v0.4.0)

![Version](https://img.shields.io/badge/Version-v0.4.0-gold)
![Platform](https://img.shields.io/badge/Platform-Windows_10%2F11_x64-blue)
![Engine](https://img.shields.io/badge/Engine-OpenSCAD-cyan)
![Languages](https://img.shields.io/badge/Languages-ES_EN_PL_DE_FR-orange)
![License](https://img.shields.io/badge/License-MIT-green)

<div align="center">
  <h3>Custom enclosures for your electronics projects, ready to 3D print</h3>
  <p><em>Give it the size of your board and connectors; CajaDIY gives you the STL of the box and the lid.</em></p>

  <a href="https://github.com/IvanLizana/CajaDIY/releases/latest">
    <img src="https://img.shields.io/badge/DOWNLOAD_INSTALLER_v0.4.0-Click_Here-success?style=for-the-badge&logo=windows&logoColor=white" alt="Download Now" />
  </a>
  &nbsp;
  <a href="Manual_de_usuario_CajaDIY.pdf">
    <img src="https://img.shields.io/badge/USER_MANUAL-PDF_(Spanish)-informational?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="User manual" />
  </a>
</div>

> # ⚠️ CRITICAL REQUIREMENT
> **FOR THIS SOFTWARE TO WORK CORRECTLY:**
> 1.  **OpenSCAD:** must be installed (free, **not included**). Download it from **[openscad.org/downloads](https://openscad.org/downloads.html)** and install it in its default folder (`C:\Program Files\OpenSCAD`).
>     * *CajaDIY uses it to build the STL files and the 3D preview.*
>     * *The **Development Snapshot** builds STL files much faster.*
> 2.  **System:** Windows 10 or 11, **64-bit**.

---

## 📄 Overview

**CajaDIY** is a parametric enclosure generator for makers building projects with **ESP32, Arduino, Raspberry Pi** or any other board. You set the inner size, the lid type, the board standoffs, the connector holes and even your logos; the program draws the box, **warns you about collisions before printing** (ports vs. mounting tabs, standoffs vs. dividers, lid vs. supports…) and exports the box and the lid as STL files, ready for your slicer.

Everything is designed with the printer in mind: parts that print **without support material**, adjustable clearances, and profiles you can save and open again.

---

## ⚡ What's New in v0.4.0

### 1. Wedge Supports 📐
Rails attached to the inner walls to hold a board or a tray.
* Flat top face and slanted bottom face (**38–52°**, 45° by default): **they print without supports**.
* Several per wall and on all four walls; position measured **from the wall you choose**; they join at the corners.

### 2. Reinforced Hinge 🔩
* The lid **no longer rubs when opening** (it used to bind and could snap at the central knuckle).
* Thicker knuckle, **dedicated hinge clearance** (0.4 mm, adjustable), relief notch in the wall and a **teardrop pin hole** that prints lying down.
* The outer face of the lid stays **flat**, cylinder included.

### 3. Dividers with Their Own Length 🧱
* No longer always wall to wall: position and start measured **from the wall you choose**, length limited to the interior.
* They can **cross each other even with different heights**.

### 4. Square Corners by Default ⬛
* Outer and inner corners at 90°; each radius can be raised separately.

---

## 📜 Version History

### [v0.2.0] - First public release
* 8 lid types, mounting tabs with zip-tie bridges, standoffs with board templates.
* Holes on all 6 faces with a connector catalogue.
* **Logos and images on the faces** (embossed, engraved or cut through), several per face, with free rotation.
* 2D view with collision warnings, OpenSCAD preview and separate STL export.

---

## 🔬 Core Features

* **8 Lids:** hinged, snap-fit, friction, screws (outside or recessed), magnets, sliding and cap.
* **Mounting Tabs:** 2 or 4, with countersink and zip-tie bridges.
* **Board Standoffs:** templates for ESP32 DevKit, Arduino UNO and Raspberry Pi 4/5.
* **Ports on All 6 Faces:** rounded rectangles or circles, with a catalogue (USB-C, micro-USB, USB-A, RJ45, jack, PG7 and M12 cable glands, terminal blocks, OLED, LED).
* **Logos and Images:** turns a PNG or JPG into an emboss, engraving or cut-out, scaled to the face automatically.
* **2D Canvas:** plan, front, side and isometric views, with dimensions, zoom and warnings in the status bar.
* **Profiles:** each enclosure is saved as a `.json` file to reopen or share.
* **Multi-language:** Español, English, Polski, Deutsch and Français, switched live.

---

## 📥 Installation & Usage Instructions

The installer **does not need admin rights** and installs in your user folder. If you already have an older version, it upgrades in place and keeps your settings and profiles.

1.  **OpenSCAD:** install it first from **[openscad.org/downloads](https://openscad.org/downloads.html)**.
2.  **Download:** go to **[Releases](../../releases/latest)** and download `CajaDIY_Setup_0.4.0.exe`.
3.  **Install:** run it and follow the wizard. If OpenSCAD is missing, it warns you and offers to open its download page.
4.  **Design:** open CajaDIY, pick a board template, adjust sizes, lid and ports, and check the warnings in the status bar.
5.  **Export:** click **"Export Box and Lid"** and open the STL files in your slicer (Cura, PrusaSlicer, Bambu Studio…).

> **⚠️ Note on Windows Defender / SmartScreen:**
> Since this is free software developed by a **hobbyist** (without a code-signing certificate), Windows might show an "Unknown Publisher" warning.
> * This is normal. Click **"More info"** and then **"Run anyway"**.
> * You can verify the installer with the **SHA-256** published in each release's notes.

---

## 🤝 Community

* **Found a bug or have an idea?** Open an **[Issue](../../issues/new/choose)** (attach your enclosure's `.json` profile if the problem is with a specific box). Issues in English are welcome.
* Before taking part, read the **[Code of Conduct](CODE_OF_CONDUCT.md)** and **[Contributing](CONTRIBUTING.md)** (in Spanish).
* Security issues: privately, as described in **[SECURITY.md](SECURITY.md)**. Accessibility: **[ACCESSIBILITY.md](ACCESSIBILITY.md)**.

---

## 📜 License / Licencia
The executable is distributed under the **MIT** license (see `LICENSE`); the source code is not published. Third-party components and their licenses: `TERCEROS.md`.
*El ejecutable se distribuye bajo la licencia **MIT** (ver `LICENSE`); el código fuente no se publica. Componentes de terceros y sus licencias: `TERCEROS.md`.*

## 🤝 Credits / Créditos
* **Developer:** Iván Lizana (ASTROREMOTO powered by FourIndustry).
* **Tech Stack:** Python + Tkinter + OpenSCAD + OpenCV.
* **Support:** [GitHub Issues](../../issues).
