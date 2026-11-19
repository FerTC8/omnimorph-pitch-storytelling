# 🧠 Reglas de Estilo, Tono y Arquitectura — Omnimorph v3

Este documento define el ADN comunicativo, los principios editoriales y las directrices técnicas obligatorias para cualquier modelo, agente o colaborador que genere contenido en el repositorio `omnimorph-pitch-storytelling`.

---

## 1. Misión del Proyecto y Audiencia

* **Propósito:** Diseñar y estructurar el **Pitch Deck, Storytelling y Guía de Demostración** de **Omnimorph** para el jurado evaluador de IBM (Maciel y directivos) y la comunidad del *IBM SkillsBuild AI Experiential Learning Lab | México 2026*.
* **Colaboración Modular con Roy (Líder Técnico):** Roy aportará los detalles específicos del agente de visión por computadora y percepción GPU local. Los entregables de este repositorio deben crear una **estructura modular** donde el bloque técnico de Roy embone de forma natural con la narrativa humana, sin duplicar ni chocar.
* **El Dualismo de Omnimorph:**
  1. **En la élite:** El analista deportivo profesional saturado de datos brutos que necesita un "traductor táctico" en tiempo real para tomar decisiones bajo presión.
  2. **En la comunidad:** La democratización del análisis para el fútbol amateur; convertir videos grabados con celulares comunes en canchas de tierra o pasto sintético en telemetría objetiva que sirva de semillero de talento para jóvenes invisibles para las visorías tradicionales.

---

## 2. Tono y Voz: Rigor Técnico con Pasión de Cancha

Escribimos y hablamos como **ingenieros y apasionados del deporte** que conocen tanto la terminal de Linux y los tensores de PyTorch como el olor a césped y la tensión de un vestidor al minuto 85.

### Principios Fundamentales:
* **Español 100% natural y conversacional:** Debe sonar a una persona real hablando con convicción en una sala de juntas o auditorio, no a un prompt corporativo traducido.
* **Verbos activos y ritmo dinámico:** Frases concisas, directas, con pausas dramáticas naturales.
* **Vocabulario auténtico de fútbol:** Usar terminología táctica real (bloque bajo, presión tras pérdida, basculación, tercer hombre, desmarque de ruptura, líneas de pase, achique, radar cenital, llano, visoría, semillero) sin sonar pedante.
* **Honestidad tecnológica:** Demostrar con orgullo lo que el motor hace hoy ($1080\text{p}$, homografía normalizada, Algoritmo Húngaro, Savitzky-Golay, `ibm/granite-3-8b-instruct`), reconociendo con transparencia los retos del video amateur y el roadmap de evolución.

---

## 3. Lista Negra Estricta: Cero Clichés de IA

Queda **estrictamente prohibido** el uso de muletillas, clichés y fórmulas acartonadas comunes en textos autogenerados. Si alguna de estas frases aparece en un borrador, debe reescribirse de inmediato:

| ❌ Frase Prohibida / Cliché de IA | ✅ Alternativa Natural y Directa |
| :--- | :--- |
| "En el vertiginoso mundo de hoy..." / "En la era digital..." | Directo al punto: *"En el fútbol profesional, cada segundo cuenta..."* |
| "Un faro de innovación..." | *"Una herramienta práctica que resuelve..."* |
| "Aprovechando el poder de la IA..." | *"Usando Granite 3 8B en IBM Cloud para..."* |
| "Revolucionando la forma en que..." | *"Cambiando el método tradicional de visorías..."* |
| "Es crucial / importante destacar que..." | Decirlo directamente sin preámbulos: *"El dato clave es..."* |
| "Un testimonio de la colaboración..." | *"El resultado del trabajo conjunto..."* |
| "Sumerjámonos en..." / "Profundicemos en..." | *"Veamos cómo funciona..."* / *"Revisemos el motor..."* |
| "Sin duda alguna..." / "Indudablemente..." | Afirmar con hechos y métricas. |
| "Desbloquear el potencial de..." | *"Permitir que un reclutador detecte a..."* |
| "Un tapiz de..." / "Piedra angular..." | Términos concretos: *"La base del sistema..."* |
| "En resumen podemos decir que..." | Conclusión contundente o llamado a la acción directo. |

---

## 4. Disciplina de Workspace y Anti-Junk (`clean-workspace-archive`)

1. **Pruebas en `/tmp/scratch/`:** Todo script desechable, clon temporal de repositorios, prueba de rendering o captura debe residir en `/tmp/scratch/`.
2. **Git Limpio:** Nada de binarios (`.mp4`, `.parquet`, `.weights`), variables de entorno (`.env`) o carpetas de paquetes (`node_modules`, `venv`) en el historial de Git.
3. **Verificación Post-Ship:** Antes de dar por terminado cualquier entregable, se realiza una lectura en frío simulando ser el jurado de IBM para eliminar fricciones y asegurar coherencia.

---

## 5. Hoja de Ruta para los Siguientes Agentes

* **`02 - Pitch & Storytelling Writer`:**
  - Redactará `PITCH_DECK.md` (estructura slide por slide: mensaje central, elemento visual sugerido y guión palabra por palabra para el orador).
  - Redactará `STORYTELLING.md` (la narrativa de los dos mundos: el analista de élite y el joven del llano).
  - Redactará `GUIA_DEMO_Y_QA.md` (guía paso a paso de los 4 paneles sincronizados y banco de preguntas difíciles para defender ante Maciel y directivos de IBM).
  - Redactará `README.md` (One-pager ejecutivo y elevator pitch de 60 segundos).
* **`03 - Naturalizer & Delivery QA`:**
  - Pulido fino de cadencia oral, ensayo de tiempos y validación de consistencia técnica.
