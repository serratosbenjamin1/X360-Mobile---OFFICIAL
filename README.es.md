# X360 Mobile - Emulador de Xbox 360 para Android

<p align="center">
  <img src="https://x360mobile.com/logo.png" alt="Logo X360 Mobile" width="180" style="border-radius: 20%;"/>
</p>

<p align="center">
  <b>Un emulador experimental nativo de Xbox 360 para Android, basado nativamente en Xenia Canary.</b>
</p>

<p align="center">
  <a href="https://www.x360mobile.com"><b>Sitio Web Oficial: www.x360mobile.com</b></a>
</p>

<p align="center">
  Choose Language / Scegli la lingua / Sprache wählen / Choisir la langue / Seleccionar idioma:
  <br>
  <a href="README.md">English</a> |
  <a href="README.it.md">Italiano</a> |
  <a href="README.de.md">Deutsch</a> |
  <a href="README.fr.md">Français</a> |
  <b>Español</b>
</p>

---

Bienvenido al repositorio oficial de **X360 Mobile**, un emulador experimental nativo de Xbox 360 diseñado específicamente para la plataforma Android. Desarrollado utilizando tecnologías modernas ARM64 y Vulkan 1.3, X360 Mobile es el **pionero en la integración nativa del aclamado núcleo Xenia Canary en Android**, aportando optimizaciones avanzadas y un alto rendimiento directamente a tus dispositivos móviles de gama alta.

> [!NOTE]
> **Propósito del repositorio:** 
> Con el fin de salvaguardar la integridad del código fuente y mantener las mejoras propietarias de rendimiento, **X360 Mobile es de código cerrado (closed-source)**. Este repositorio oficial no contiene el código fuente del emulador. En su lugar, sirve como **archivo de versiones oficial y plataforma de distribución principal** para el lanzamiento de paquetes APK, la gestión de problemas de compatibilidad (Issues) y el intercambio de guías de usuario.

---

## Características Principales

* **Cimientos nativos en Xenia Canary:** El primer emulador para Android diseñado de forma nativa en torno a Xenia Canary desde su concepción, en lugar de migrar posteriormente de Xenia Master, garantizando una arquitectura y rendimiento superiores.
* **Backend de Vulkan Moderno:** Aprovecha las API Vulkan 1.3 para ofrecer una utilización óptima del hardware, altas tasas de fotogramas (FPS) y una mínima sobrecarga de sistema.
* **Controles Táctiles Personalizados:** Mandos virtuales completamente personalizables con respuesta háptica, fluidez analógica y diseños adaptados a cualquier tamaño de pantalla.
* **Soporte para Mandos Físicos:** Compatibilidad plug-and-play instantánea con controladores externos a través de Bluetooth o USB-OTG (incluyendo mandos de Xbox Series X|S, DualSense, DualShock 4 y los principales controladores móviles).
* **Perfiles Específicos para cada Juego:** Ajusta resoluciones, opciones de compilación de shaders y limitaciones de memoria individualmente por juego para exprimir al máximo la potencia de tu dispositivo.
* **Optimizaciones para Móviles:** Traducción dinámica integrada del código de ensamblaje PowerPC a instrucciones nativas ARM64 con microoptimizaciones específicas para chipsets Snapdragon y Dimensity.

---

## Requisitos del Sistema

La emulación de Xbox 360 es un proceso experimental y sumamente exigente a nivel de computación, el cual requiere una traducción de hardware compleja en tiempo real. Por favor, consulta la siguiente tabla para entender el rendimiento esperado de tu dispositivo.

| Especificación | Requisitos Mínimos | Recomendados (Para velocidad fluida) |
| :--- | :--- | :--- |
| **Sistema Operativo** | Android 12 (64 bits) | Android 13 o posterior (64 bits) |
| **Procesador y GPU** | Qualcomm Snapdragon con GPU Adreno (series 600/700/800) | Qualcomm Snapdragon de gama alta (se recomienda Snapdragon 8 Gen 1 o superior) |
| **RAM (Memoria)** | 6 GB de RAM | 8 GB - 12 GB de RAM (o superior) |
| **Almacenamiento (Velocidad)** | Almacenamiento rápido (se recomienda UFS 3.1 o superior) | Almacenamiento ultra-rápido UFS 3.1/4.0 |

> [!WARNING]
> Los dispositivos equipados con procesadores que tengan GPU Mali, GPU Samsung Xclipse (basadas en AMD RDNA), GPU Adreno obsoletas (anteriores a la serie 600) o chipsets de gama de entrada/económicos sufrirán graves limitaciones de rendimiento, errores gráficos, estrangulamiento térmico (thermal throttling) severo o fallos de la aplicación. Se recomienda encarecidamente un procesador Qualcomm Snapdragon moderno con GPU Adreno para obtener resultados óptimos.

---

## Guía de Inicio Rápido

1. **Descarga el APK:** Dirígete a nuestra sección de [Releases](https://github.com/Ashnar2602/X360-Mobile---OFFICIAL/releases) y descarga el último paquete `.apk` estable.
2. **Habilita Orígenes Desconocidos:** Si se te solicita, permite que tu navegador web o administrador de archivos instale aplicaciones de fuentes desconocidas en los ajustes de seguridad de Android.
3. **Instala y Ejecuta:** Instala el archivo APK descargado e inicia **X360 Mobile**.
4. **Configura los Directorios:** Crea una carpeta dedicada en el almacenamiento interno o externo de tu dispositivo (por ejemplo, `/Emulación/Xbox360/Juegos`) y coloca allí tus archivos de juegos obtenidos legalmente.
5. **Formatos de Juego:** El emulador admite oficialmente los formatos `.iso`, `.xex` y carpetas descomprimidas (unpacked).
6. **Carga y Juega:** Dirige el emulador a tu carpeta de juegos, selecciona un título y ¡comienza a jugar!

---

## Preguntas Frecuentes (FAQ)

### ¿X360 Mobile es gratuito?
**Sí.** X360 Mobile se puede descargar y utilizar de forma completamente gratuita. No cobramos tarifas ni incluimos publicidad intrusiva que pueda arruinar la experiencia de juego.

### ¿Por qué el proyecto es de código cerrado?
Decidimos mantener X360 Mobile como código cerrado para evitar bifurcaciones fraudulentas, distribuciones modificadas con malware (por ejemplo, inyección de adware/spyware en nuestras compilaciones) y para proteger nuestra línea exclusiva de conversión ARM64 y optimizaciones del compilador. Queremos asegurarnos de que los usuarios reciban únicamente paquetes seguros, altamente optimizados y firmados oficialmente de forma directa desde este repositorio o nuestro sitio web oficial.

### ¿Está X360 Mobile relacionado con el proyecto de escritorio Xenia?
X360 Mobile se basa en el increíble código fuente de **Xenia Canary** (un proyecto de código abierto para PC). Hemos portado, reestructurado y optimizado los motores de renderizado y ejecución originales para que funcionen bajo Android. Respetamos profundamente a los desarrolladores originales de Xenia y nuestro objetivo es ofrecer el mismo nivel de excelencia en dispositivos móviles.

### ¿Qué juegos puedo ejecutar en este momento?
La compatibilidad es un esfuerzo constante. Actualmente se han **probado más de 300 títulos**, de los cuales aproximadamente el **40% es totalmente jugable**.

Para obtener una lista de compatibilidad completa y actualizada, visita nuestro sitio web oficial en [www.x360mobile.com](https://www.x360mobile.com). Aunque los títulos Arcade clásicos, los juegos independientes y los juegos 3D ligeros funcionan excelente, los títulos AAA más exigentes (como *Red Dead Redemption*, *Halo 3* o *Gears of War*) se pueden ejecutar y alcanzar velocidades jugables en los procesadores Snapdragon insignia más recientes, aunque aún pueden presentar pequeños errores gráficos o caídas de fotogramas aleatorias.

---

## Reportar Problemas

Si encuentras fallas, errores gráficos o problemas de compatibilidad:
1. Dirígete a la sección de [Issues](https://github.com/Ashnar2602/X360-Mobile---OFFICIAL/issues).
2. Comprueba si el problema ya ha sido reportado por otro usuario.
3. Si no es así, abre un nuevo reporte utilizando nuestra plantilla e incluye:
   * El modelo de tu dispositivo y su procesador (p. ej., Samsung Galaxy S23, Snapdragon 8 Gen 2).
   * La versión exacta de Android y la cantidad de RAM.
   * El título del juego y su formato (.iso o .xex).
   * Una descripción detallada del error y, si es posible, capturas de pantalla o vídeos.

---

## Notas Legales y Descargo de Responsabilidad

* **Xbox 360** es una marca registrada de Microsoft Corporation. **X360 Mobile** no está afiliado, autorizado, patrocinado ni respaldado de ninguna manera por Microsoft Corporation, sus filiales o subsidiarias.
* Todos los títulos de juegos, imágenes y recursos de marca son marcas registradas de sus respectivos propietarios.
* **X360 Mobile** no incluye ningún archivo de juego, software del sistema (dashboard) ni ROM protegida por derechos de autor. Los usuarios están legalmente obligados a poseer copias físicas de los juegos y realizar su copia de seguridad (dump) para uso personal y no comercial.
* Al descargar y utilizar este software, aceptas nuestros términos de servicio y reconoces que la emulación es una tecnología experimental utilizada bajo tu propio riesgo.

---

<p align="center">
  © 2026 X360 Mobile Team. Todos los derechos reservados. <br>
  Para noticias, actualizaciones y más, visita <a href="https://www.x360mobile.com">www.x360mobile.com</a>.
</p>
