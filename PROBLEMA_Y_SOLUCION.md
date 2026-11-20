# OMNIMORPH: Problema y Solución

**Proyecto:** Omnimorph v3 | **Convocatoria:** IBM SkillsBuild AI Lab México 2026  
**Entregable Oficial:** Documento Ejecutivo (Límite estricto: ≤ 500 palabras)

---

## 1. El Problema: Saturación en la Élite, Invisibilidad en el Llano

El fútbol padece una fractura que desconecta el dato del factor humano:

En la élite, el cuerpo técnico dispone de solo 15 minutos de medio tiempo para revisar más de 40,000 coordenadas de telemetría. Reciben tablas densas y mapas de calor estáticos que ningún entrenador logra traducir en ajustes tácticos inmediatos bajo presión.

En el fútbol formativo y amateur —con más de 1.5 millones de partidos semanales en México y Latinoamérica—, el 95% del talento es invisible. Las visorías masivas duran 15 minutos para 200 jóvenes; el evaluador, presionado por el tiempo, incurre en sesgos documentados: favorece la corpulencia física o al delantero que anotó un gol fortuito. Perfiles tácticos clave como el mediocentro que sostiene la compacidad o el extremo que genera rupturas sin balón quedan descartados por falta de métricas. Herramientas de élite como Catapult o Wyscout ($2,000 a $10,000 USD anuales) resultan inviables para el 99% de las ligas locales.

## 2. La Solución Omnimorph e Innovación Técnica

Omnimorph convierte video estándar monocular (transmisión broadcast o celular) en radar métrico 2D cenital y crónica táctica en español en tiempo real, mediante una arquitectura híbrida de bajo costo:

1. **Percepción local estabilizada:** Seis agentes de visión en GPU rastrean 22 jugadores, árbitros y balón. Aplica homografía adaptativa normalizada ($H/H_{2,2}$) para eliminar vibración, Algoritmo Húngaro para preservar identidades tras oclusiones, y derivadas Savitzky-Golay con cota fisiológica estricta ($v \le 9.5\text{ m/s}$).
2. **Orquestación en IBM Cloud:** Los vectores estabilizados se comprimen en ventanas tácticas de 4.0 segundos (< 500 bytes) y se procesan en CPU con **watsonx Orchestrate ADK** en menos de 1.5 segundos.
3. **Razonamiento con Granite 3 8B:** El modelo **`ibm/granite-3-8b-instruct`** interpreta compacidad de bloque, basculaciones y líneas de pase, generando síntesis táctica precisa con temperatura 0.3.
4. **Gobernanza activa (Monitor M3):** Registra cada inferencia en `governance_audit.jsonl` y valida afirmaciones del modelo contra métricas físicas, erradicando alucinaciones tácticas.

## 3. Impacto y Viabilidad

Omnimorph democratiza la captación mediante el **Pasaporte Táctico Objetivo**: una ficha métrica certificada por partido que registra velocidad punta, coberturas defensivas y lectura espacial en lenguaje de entrenador. Esto elimina el sesgo geográfico y el compadrazgo, permitiendo a los clubes evaluar prospectos del llano con la misma objetividad que en primera división.

Viabilidad económica garantizada: al delegar la percepción visual al borde y la síntesis semántica a micro-cargas en IBM Cloud, el costo de inferencia es de solo ~$0.003 USD por minuto analizado, permitiendo un modelo B2B para clubes y un esquema freemium para academias comunitarias.

---

**Conteo total verificado:** 470 palabras (100% del archivo, incluidos títulos y metadatos) | Cumple límite estricto ≤ 500 palabras.
