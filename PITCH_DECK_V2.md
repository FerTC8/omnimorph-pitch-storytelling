# Omnimorph v3 — Pitch Deck Oficial (Versión Ejecutiva v2)

Este documento contiene la estructura y contenido exacto de las 6 diapositivas ejecutivas del archivo `PITCH_DECK_IBM_V2.pptx`, alineado milimétricamente con el guion final de 3:00 minutos de `Omnimorph · Guion final del video (3_00) v2.pdf` y bajo los principios de diseño de IBM Carbon y Apple Executive.

---

## Diapositiva 1: El Problema
* **Kicker:** `OMNIMORPH · IBM SKILLSBUILD AI EXPERIENTIAL LEARNING LAB`
* **Título:** **El Problema: La Ceguera Táctica y la Dependencia del Papel**

### Tarjeta 1 — Diagnóstico Tardío
* **Premisa:** En el fútbol todos opinan después del partido.
* Siempre hay alguien que asegura saber exactamente qué debió hacerse una vez cerrado el marcador.
* Un cuerpo técnico necesita tomar decisiones antes y durante el encuentro, no cuando ya es tarde.
* Sin herramientas de análisis automatizadas, analizar significa pausar manualmente una grabación y tomar notas en una libreta.

### Tarjeta 2 — El Coste de la Imprecisión
* **Premisa:** Un dato equivocado es peor que no tener datos.
* Métricas cinemáticas defectuosas provocan cambios tácticos errados en momentos cruciales.
* El 95% de los clubes no pueden pagar sistemas de $20,000 USD anuales (Catapult, TRACAB o Veo).
* La industria exige rigor matemático, validación automática y accesibilidad sin necesidad de hardware propietario.

### Cierre de Impacto
> **Conclusión del Reto:** El fútbol no necesita más cámaras estáticas ni tablas densas de números incomprensibles. Necesita una herramienta que traduzca el video en explicaciones espaciales verificables.

---

## Diapositiva 2: Audiencia Objetivo
* **Kicker:** `OMNIMORPH · ECOSISTEMA DE IMPACTO`
* **Título:** **Audiencia Objetivo: Del Banquillo Profesional a la Cancha Formativa**

### Columna A — Segmento Profesional & Semiprofesional (Cuerpos Técnicos y Analistas)
* **Dolor actual:**
  * Ventana crítica de 15 minutos en el medio tiempo: imposible procesar hojas de cálculo con 40,000 coordenadas.
  * Desconfianza en datos brutos: temor constante a basar un cambio táctico en un error de detección.
* **Propuesta Omnimorph:**
  * Radar cenital inmediato que revela ocupación de espacios y compacidad de líneas.
  * Narración y consultas en lenguaje natural para obtener diagnósticos tácticos sin intermediarios técnicos.

### Columna B — Segmento Formativo & Comunidad (Fútbol Formativo, Equipos Menores y Visorías)
* **Dolor actual:**
  * Invisibilidad del talento: las visorías tradicionales solo llegan a las capitales o requieren redes de contactos personales.
  * Único recurso disponible: grabaciones caseras de celular realizadas desde la banda por padres o entrenadores.
* **Propuesta Omnimorph:**
  * Telemetría objetiva sin sensores corporales ni cámaras especiales: análisis directo desde el video del smartphone.
  * Democratización del semillero: telemetría verificable para que ningún jugador quede fuera por falta de datos.

---

## Diapositiva 3: La Solución
* **Kicker:** `OMNIMORPH · PROPUESTA TECNOLÓGICA`
* **Título:** **La Solución: De Video Monocular a Telemetría Explicada**

### Los 4 Pilares Modulares:
1. **01 · Visión Robusta (Cámara Dinámica & Tracking):**
   * Detecta a los 22 jugadores y el balón en tiempo real. La cámara se mueve todo el tiempo y, aun así, calcula con exactitud matemática dónde está cada uno sobre el terreno.
   * *Base técnica:* Normalización $H/H_{2,2}$ y Algoritmo Húngaro para preservar identidades tras oclusiones.
2. **02 · Radar Cenital 2D (Ocupación y Espacio Métrico):**
   * Proyecta el partido en una perspectiva cenital de 120×70m. Permite ver en qué mitad se juega, qué tan adelantado está cada bloque y cuánto espacio útil ocupa cada equipo.
   * *Base técnica:* Verificable cuadro a cuadro directamente sincronizado sobre el video original.
3. **03 · Narrador MATEO + Granite (Explicación Táctica en Español):**
   * IBM Granite en watsonx.ai analiza las posiciones y redacta el diagnóstico táctico; el agente MATEO lo narra en español con voz en off en sincronía con la jugada.
   * *Base técnica:* Traducción inmediata de coordenadas abstractas a conceptos de fútbol real.
4. **04 · Rigor y Consulta Interactiva (Validación 9/9 y Chatbot):**
   * Cada métrica pasa por 9 revisiones automáticas. Lo que aún no alcanza confianza estadística se marca 'Por validar'. Además, el usuario puede preguntar al Chatbot cualquier detalle del partido.
   * *Base técnica:* Respuestas basadas estrictamente en la telemetría del partido completo.

---

## Diapositiva 4: Diagrama de Arquitectura y Gobernanza
* **Kicker:** `OMNIMORPH · ARQUITECTURA TÉCNICA Y ÉTICA`
* **Título:** **Diagrama de Arquitectura Híbrida y Gobernanza Responsable**

### Pipeline en 3 Fases:
* **Capa 1: Percepción en el Borde (Procesamiento Local GPU/Edge):**
  * Video monocular sin sensores corporales.
  * Homografía adaptativa normalizada + Algoritmo Húngaro (identidades).
  * Derivadas de Savitzky-Golay acotadas físicamente ($v \le 9.5\text{ m/s}$).
* **Capa 2: Razonamiento e IA Cloud (IBM Granite en watsonx.ai):**
  * Vector cinemático comprimido ($< 500\text{ bytes}$).
  * Orquestación desarrollada con IBM Bob.
  * watsonx Orchestrate ADK ($< 1.5\text{s}$) e inferencia táctica estructurada.
* **Capa 3: Experiencia Sincronizada (Dashboard Multimodal):**
  * Video con marcas + Radar 2D de 120×70m.
  * MATEO: Narración de voz en off en español.
  * Chatbot interactivo en tiempo real y Página de Partido (diagrama de goles).

### Compromisos de IA Responsable & Ética:
1. **Privacidad Total por Diseño:** El video jamás sale del dispositivo. El procesamiento computacional se ejecuta en local y se descarta de memoria volátil inmediatamente.
2. **Cero Rastreo Biométrico:** No se analizan rasgos faciales ni identidades personales; únicamente coordenadas cinemáticas relativas $(x, y)$ de siluetas deportivas.
3. **Honestidad Algorítmica (9 de 9 Comprobaciones):** Marcado explícito 'Por validar' en toda métrica con incertidumbre física, erradicando alucinaciones tácticas.

---

## Diapositiva 5: Demostración
* **Kicker:** `OMNIMORPH · VALIDACIÓN CON DATOS REALES`
* **Título:** **Demostración: Caso de Prueba Costa Rica vs. San Cristóbal y Nieves**

### Caso de Estudio en Competición Real
* **Clip de prueba:** 36 segundos continuos del partido oficial Costa Rica vs. San Cristóbal y Nieves.
* **Desafío de cámara:** Tomas en paneo, zoom continuo y oclusiones masivas entre jugadores en mediocampo.
* **Resultados visuales demostrados:**
  1. Panel con marcas: bounding boxes estables y seguimiento de trayectoria del balón.
  2. Radar cenital sincronizado: proyección inmediata de líneas de presión y bloques.
  3. Página de Partido: navegación interactiva con el diagrama analítico de goles.

### Interacción en Lenguaje Natural & Validación
* **Pregunta del usuario:** *«¿Por qué el equipo A perdió el mediocampo en el minuto 20?»*
* **Respuesta de IBM Granite:** *«El bloque se expandió a 38 metros de separación. La distancia entre los centrales y el mediocentro defensivo generó una zona libre aprovechada en tres recepciones consecutivas.»*
* **Análisis Verificado (9 de 9 Comprobaciones):** Toda métrica fuera del rango fisiológico normal se clasifica como 'Por validar' antes de alimentar la respuesta del modelo, protegiendo la veracidad táctica.

---

## Diapositiva 6: Cierre y Visión de Futuro
* **Kicker:** `OMNIMORPH · VISIÓN DE FUTURO E IMPACTO`
* **Título:** **Cierre: Democratización del Análisis Deportivo Global**

### Nuestro Propósito Central
> **«Que ningún jugador quede fuera por falta de datos.»**  
> *Omnimorph demuestra que el análisis táctico de alto nivel no requiere sensores corporales millonarios ni estadios inteligentes. Hoy es un prototipo validado sobre partidos reales; el siguiente paso es llevarlo a los videos de celular que tienen los equipos más chicos de cualquier rincón del mundo.*

### Escalabilidad & Oportunidad Futura
* **Extensión a dispositivos móviles:** Ingesta directa desde tomas laterales de smartphones para academias y ligas comunitarias.
* **Semillero transparente:** Generación de perfiles cinemáticos comparables para visorías objetivas en comunidades marginadas.
* **Metodología ágil:** Construido en 7 semanas gracias a IBM Granite en watsonx.ai y el apoyo de IBM Bob.

### Cierre de Marca
> **OMNIMORPH**  
> *Para que la próxima vez... no te lo cuente tu cuñado.*  
> Táctica explicable y accesible para todo el fútbol.
