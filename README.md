# Corrector de Armonía

Aplicación web interactiva para escribir, escuchar y analizar ejercicios de armonía clásica a cuatro voces (Soprano, Contralto, Tenor y Bajo). Diseñada como herramienta de apoyo para estudiantes y profesores de lenguaje musical y armonía.

🌍 **[Probar la aplicación en vivo](https://patgmez.github.io/Corrector-de-Armon-a/)**

## Características Principales

* **Análisis Armónico y Sintáctico:** Detecta acordes, inversiones, grados funcionales, modulaciones y tipos de cadencias (Perfecta, Plagal, Rota, Semicadencia, Tercera Picarda, etc.).
* **Corrección de Reglas Clásicas:** Señala errores visualmente en la partitura con códigos de color:
  * Quintas y octavas paralelas y directas.
  * Cruzamientos de voces y solapamientos.
  * Saltos melódicos prohibidos.
  * Resoluciones incorrectas de la sensible y disonancias (séptimas, novenas).
  * Notas fuera de tesitura y problemas de espaciado.
* **Partitura Interactiva y Piano Virtual:** Renderizado en tiempo real. Permite introducir notas haciendo clic en el teclado virtual, usando el teclado del PC (teclas A-G) o arrastrando las notas directamente en el pentagrama.
* **Reproducción de Audio:** Sintetizador integrado con varios instrumentos (Piano, Cuerdas, Voces, Arpa). Incluye una opción para destacar el volumen de una voz específica.
* **Modo Audición (Ear Training):** Oculta la partitura para practicar dictados armónicos y entrenamiento auditivo.
* **Sugerencia de Acordes:** Motor inteligente que recomienda acordes o los construye a partir de un bajo cifrado, garantizando que no se cometan faltas de enlace con el contexto anterior y posterior.
* **Gestión de Archivos:** Permite importar/exportar en formato `.abc` (texto plano) y `.json` (proyectos completos), así como exportar la partitura resultante a PNG o PDF.

## Cómo usarlo

1. **Configuración:** Selecciona la tonalidad y el compás en la barra superior.
2. **Escritura:** Selecciona una voz (Soprano, Contralto, Tenor o Bajo) y un acorde. Usa el piano inferior o el teclado para añadir notas.
3. **Análisis:** Pulsa el botón verde **Analizar** para ejecutar el motor de corrección. Los resultados aparecerán en una ventana flotante y los errores se trazarán sobre las propias notas.
4. **Edición:** Desde el menú "Edición" puedes añadir anacrusas, cambiar valores rítmicos, insertar silencios, generar cifrado interválico o abrir el editor de código ABC puro.

## Tecnologías Utilizadas

* **HTML5, CSS3, JavaScript (Vanilla):** Lógica principal y motor de reglas estructurado sin frameworks pesados.
* **[ABCJS](https://www.abcjs.net/):** Para el renderizado de la partitura musical en notación estándar.
* **[Tone.js](https://tonejs.github.io/):** Para la síntesis y reproducción de audio en el navegador usando Web Audio API y Soundfonts.
* **[jsPDF](https://parall.ax/products/jspdf):** Para la exportación de gráficos vectoriales a PDF.

## Instalación Local

No requiere instalación, dependencias de Node ni servidor de backend.
1. Clona el repositorio: `git clone https://github.com/patgmez/Corrector-de-Armon-a.git`
2. Abre el archivo `index.html` en cualquier navegador web moderno.
*(Nota: Se requiere conexión a internet para cargar las librerías de ABCJS y los samples de Tone.js la primera vez).*


Si encuentras algún error o tienes sugerencias, por favor repórtalo en la pestaña Issues