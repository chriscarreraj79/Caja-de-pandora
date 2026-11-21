# Análisis de los prompts "Multiverse GPT"

Análisis de los dos prompts de ChatGPT creados hace un par de años, y de cómo se transformaron en la skill `code-cheater` (modo B).

## Prompt 1 — Ruta de 42 pasos (de Hofstede al pitch de 60 segundos)

### Lo que tiene de valioso
- **Visión integral:** une cultura (Hofstede), cliente (buyer persona, JTBD), inconsciente (Rapaille, Zaltman), identidad (Jung, Campbell, Pearson, Aaker), negocio (Osterwalder) y mensajes. Muy pocos marcos combinan todo esto.
- **Diferencial único:** usar los arcanos de *La Vía del Tarot* de Jodorowsky para construir el arquetipo de marca. Es original y coherente con tu enfoque.
- **Orientación práctica:** termina en entregables usables (anuncios, propuestas de valor de 144 caracteres, descripciones web, pitch).
- **Hay una validación con el usuario** (paso 3), lo que muestra intuición de que el proceso necesita pausas.

### Problemas y cómo se resolvieron
| Problema | Por qué afecta | Solución en la skill |
|---|---|---|
| "Analizas cada pregunta 10 veces" y "versión mejorada de GPT-4" | Es una fórmula de efecto placebo: el modelo no "piensa 10 veces" porque se lo pidan. Ocupa espacio sin mejorar la respuesta. | Se reemplaza por reglas de calidad concretas: tres niveles de análisis, hipótesis con validación, formato. |
| 42 pasos en un solo flujo | La calidad cae en los pasos finales, se pierde el contexto y el usuario recibe un muro de texto. | 6 fases con pausa de validación al final de cada una, más un menú de módulos sueltos. |
| Pasos repetidos (USP 3 veces, propuesta de valor 4, códigos culturales 3, listas de empresas 2, descripciones 3) | Respuestas redundantes y contradictorias entre sí. | Se agrupan en una sola fase cada uno. |
| Listas de empresas, sitios web, USP de competidores y proyecciones | Sin búsqueda en internet, el modelo **inventa** nombres y URLs con apariencia real. Es el mayor riesgo del prompt. | Regla de "cero datos inventados": solo datos verificados; si no, estructura para investigar y la marca [por verificar]. |
| "Analiza la categoría del negocio bajo el modelo de Hofstede" | Hofstede mide culturas **nacionales**, no categorías de negocio. Es un uso incorrecto del modelo. | Hofstede se aplica al país; la categoría se analiza con competencia, tendencias y códigos. |
| Rapaille presentado como certeza | Su método exige sesiones con personas reales; un chat solo puede formular hipótesis. Además se apoya en la teoría del cerebro triuno, hoy descartada. | Improntas y códigos como hipótesis, con un mini estudio de validación (entrevistas + imágenes estilo ZMET). |
| Orden ilógico (USP antes del buyer persona; listas de empresas en medio de la estrategia) | La USP depende del cliente; sin cliente definido es una frase vacía. | Orden: contexto → cliente → código → identidad → narrativa → modelo. |
| Miedos profundos sin marco ético | El mismo método que usaba Bernays puede derivar en publicidad que explota inseguridades. | Pacto ético: el miedo se nombra para resolverlo, con una propuesta honesta para cada uno. |
| Sin datos de entrada (etapa, presupuesto, valores) | El modelo rellena con suposiciones invisibles. | Fase 0 de encuadre con 6 datos y supuestos explícitos. |
| Sin formato de salida ni cierre | Difícil de reutilizar. | Tablas, conteo de caracteres y resumen de una página. |
| La marca como héroe | Contradice a Campbell aplicado a marca: el héroe es el cliente. | La marca es mentor o aliado. |
| Sin indicadores | No se sabe si la estrategia funciona. | Fase 6 con 5 métricas y plan de 90 días. |

## Prompt 2 — Módulos sueltos (JTBD, diferenciales, target, beneficios, improntas, códigos, metáforas)

### Lo que tiene de valioso
- **Modularidad:** cada pieza se puede pedir por separado. Es más útil en el día a día que la ruta de 42 pasos.
- **Beneficios en seis dimensiones** (físicos, mentales, emocionales, holísticos y de estilo de vida, ambientales y sociales): un marco más rico que el clásico funcional/emocional.
- **Improntas positivas y negativas en modo hipótesis:** muy buen instinto, porque reconoce que son suposiciones.
- **El contraste "lo que diría ChatGPT / la respuesta profunda":** obliga a separar la obviedad del insight.

### Problemas y cómo se resolvieron
| Problema | Solución en la skill |
|---|---|
| El bloque "Multiverse GPT" se repite en cada módulo y el formato "Chat GPT: … / Multiverse GPT: …" duplica la respuesta, una de ellas deliberadamente pobre. | El contraste se conserva con fundamento: **lo que se dice / lo que se siente / el código** (los tres niveles de las sesiones de Rapaille). Todo el texto es útil. |
| "Target" no es un marco de referencia; pedir "10 targets" sin criterio genera listas genéricas. | Segmentos con justificación y priorización de 2–3. |
| Los pasos 6 y 10 son el mismo prompt (metáforas desde Rapaille); 7 y 8 casi iguales (improntas). | Unificados en la fase 3, con un solo formato de tabla. |
| Metáforas solo desde Rapaille. | Se integra Zaltman (siete metáforas profundas) y se pide imagen visual + justificación. |
| JTBD sin formato. | Formato estándar *Cuando… quiero… para…*, con trabajos funcionales, emocionales y sociales. |
| Pasos 11 y 12 vacíos. | Completados por el resto del método (identidad, narrativa, modelo). |

## Resultado
Los dos prompts se fusionan en el **modo B** de la skill (`skills/code-cheater/references/metodo-marca.md`): la ruta completa del prompt 1, reordenada en 6 fases, y los módulos del prompt 2 como menú de acceso rápido. La skill suma además un **modo A** de consulta y un **modo C** de formación, ausentes en los originales.

Para usarlo en ChatGPT como GPT personalizado, ver `docs/prompt-gpt-codigo-simbolico.md`.
