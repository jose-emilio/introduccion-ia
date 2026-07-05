# Laboratorio 4: Vigilancia Regulatoria y Trazabilidad con Perplexity AI

**Módulo:** 5 — Ética, Regulación y Gobernanza de la IA
**Duración estimada:** 20 min
**Tipo:** Ejercicio práctico individual
**Herramientas:** Perplexity AI (perplexity.ai)

---

## Objetivos

Al completar este laboratorio, podrás:

- Investigar normativas reales (IA Act, GDPR, ENS) usando Perplexity AI
- Extraer respuestas estructuradas con fuentes oficiales explicitas
- Validar críticamente si el output incurre en alucinaciones analizando los enlaces proporcionados

---

## ¿Por qué es importante este laboratorio?

Los LLMs tradicionales pueden inventar regulaciones, citar artículos que no existen o mezclar jurisdicciones. En un contexto de cumplimiento normativo, una alucinación puede costar una multa o un litigio.

**Perplexity AI** se diferencia porque **cita las fuentes explicitamente** mediante enlaces. Esto permite al profesional verificar la información antes de usarla en una decisión corporativa.

> La trazabilidad de las fuentes no es un lujo: es un requisito legal en entornos regulados.

---

## ¿Qué vas a necesitar?

- Un navegador web
- Acceso a **Perplexity AI** (perplexity.ai) en su versión gratuita
- La página oficial del IA Act, GDPR o ENS abierta en otra pestaña para contrastar

---

## Actividad 1: Consulta estructurada sobre el IA Act (5 min)

### Paso 1: Abre Perplexity

Ve a https://perplexity.ai e inicia sesión con tu cuenta de Google o email.

Asegúrate de que el botón de **"Búsqueda en profundidad"** o **"Pro"** esté desactivado (modo estándar).

### Paso 2: Activa el foco en fuentes

Antes de escribir, haz clic en el selector de **foco** (Focus) y selecciona **"Académico"** o **"Web"**. Esto hará que Perplexity priorice fuentes oficiales y publicaciones revisadas.

> Usar el foco correcto evita que la herramienta busque en foros o blogs sin autoridad.

### Paso 3: Formula la consulta

Copia y pega **exactamente** esta consulta:

> *"Clasificación de riesgos del IA Act europeo: explica los cuatro niveles de riesgo (inaceptable, alto, limitado, mínimo) y los requisitos de transparencia para sistemas de IA generativa. Cita los artículos concretos del reglamento y sus fuentes oficiales de la UE."*

Pulsa Enter y espera la respuesta.

**Pega aquí la respuesta de Perplexity (o un resumen con las fuentes que citó):**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 4: Identifica las fuentes

Perplexity muestra la respuesta con números en línea (`[1]`, `[2]`, etc.) y las fuentes al final. Anota las fuentes que citó:

| Fuente | Tipo (web oficial / blog / noticia) | ¿Es una fuente autorizada? |
|--------|-------------------------------------|---------------------------|
| | | [ ] Sí [ ] No |
| | | [ ] Sí [ ] No |
| | | [ ] Sí [ ] No |

**Responde:**
1. ¿Cuántas fuentes citó Perplexity? ______
2. ¿Alguna fuente es de dominio `.europa.eu` o `.gov`? ______
3. ¿La respuesta incluye números de artículo concretos del reglamento? ______

---

## Actividad 2: Consulta sobre GDPR y sanciones (5 min)

### Paso 1: Nueva consulta

Haz clic en **"Nuevo hilo"** (o el icono de nueva conversación) para empezar limpio.

Escribe esta consulta:

> *"¿Cuáles son las multas máximas por incumplimiento del GDPR/RGPD en 2026? Detalla los criterios que determinan la cuantía de la sanción y cómo afecta el uso de IA al cálculo de la multa. Proporciona URLs oficiales de la AEPD o del Parlamento Europeo."*

Pulsa Enter.

**Pega aquí la respuesta de Perplexity:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 2: Verificación cruzada

Ahora abre en otra pestaña del navegador la web oficial de la **AEPD** (https://www.aepd.es) o del **Parlamento Europeo**.

Busca el artículo sobre sanciones del GDPR (Artículo 83) y compáralo con lo que dijo Perplexity.

**Responde:**
1. ¿La cifra de la multa máxima coincide con la fuente oficial? ______
2. ¿Perplexity citó correctamente el Artículo 83 del GDPR? ______
3. ¿Las URLs que proporcionó funcionan y llevan al contenido correcto? ______

---

## Actividad 3: Detección de alucinaciones (5 min)

### Paso 1: Consulta trampa

Los LLMs a veces alucinan cuando se les pregunta por normativas muy recientes o específicas. Escribe esta consulta:

> *"¿Qué dice el Esquema Nacional de Seguridad (ENS) sobre el uso de inteligencia artificial en las administraciones públicas? Cita el artículo concreto y el BOE donde se publicó la última actualización."*

Espera la respuesta.

**Pega la respuesta aquí:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 2: Valida las fuentes

Pincha en cada enlace que proporcionó Perplexity. Verifica:

| Fuente citada | ¿El enlace funciona? | ¿El contenido coincide con lo que dijo Perplexity? |
|---------------|---------------------|---------------------------------------------------|
| | [ ] Sí [ ] No | [ ] Sí [ ] No |
| | [ ] Sí [ ] No | [ ] Sí [ ] No |
| | [ ] Sí [ ] No | [ ] Sí [ ] No |

### Paso 3: Juicio crítico

**Responde:**
1. ¿Alguna fuente no existe o no dice lo que Perplexity afirmó? ______
2. ¿El número de artículo o BOE citado es correcto? ______
3. **Conclusión:** ¿Confiarías en esta respuesta para una decisión corporativa? ¿Por qué?

> _________________________________________________________________
> _________________________________________________________________

**Mi veredicto sobre la respuesta:** [ ] Fiable [ ] Parcialmente fiable [ ] No fiable

---

## Actividad 4: Extracción estructurada con tabla (5 min)

### Paso 1: Consulta con formato exigido

Ahora vas a forzar a Perplexity a devolverte una tabla estructurada. Escribe:

> *"Compara el IA Act europeo, el GDPR/RGPD y el ENS en una tabla con las siguientes columnas: Normativa | Año de publicación | Ámbito de aplicación | Máxima sanción | Requisitos para IA. Para cada celda, incluye la fuente oficial entre paréntesis."*

Pulsa Enter.

**Pega aquí la tabla que devolvió Perplexity:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 2: Verifica una fila completa

Elige **una fila** de la tabla y verifica **cada fuente** de esa fila.

**Fila elegida:** _____________________________________________________

| Columna | Lo que dice Perplexity | Fuente citada | ¿Coincide con la fuente real? |
|---------|----------------------|---------------|------------------------------|
| | | | [ ] Sí [ ] No |
| | | | [ ] Sí [ ] No |
| | | | [ ] Sí [ ] No |

**Responde:**
1. ¿La estructura en tabla facilitó la verificación? ______
2. ¿Preferirías esta respuesta para un informe ejecutivo frente a un párrafo? ______
3. ¿Qué porcentaje de las fuentes dirías que son correctas? ______%

---

## Resumen del laboratorio

- [ ] Consulté sobre el IA Act con fuentes oficiales
- [ ] Consulté sobre sanciones del GDPR y verifiqué contra la AEPD
- [ ] Hice una consulta "trampa" sobre el ENS y validé críticamente las fuentes
- [ ] Extraje una tabla comparativa estructurada
- [ ] Verifiqué manualmente al menos un enlace de cada consulta

---

## Soluciones

### Actividad 1 — ¿Qué esperar del IA Act? [↑ Volver](#actividad-1-consulta-estructurada-sobre-el-ia-act-5-min)

Perplexity debería citar fuentes como:
- https://artificialintelligenceact.eu (dominio .eu)
- https://eur-lex.europa.eu (diario oficial de la UE)
- https://www.linkedin.com/pulse/ (artículos de expertos, menor prioridad)

Los cuatro niveles de riesgo deben aparecer claramente: inaceptable (prohibido), alto (permitido con auditorías), limitado (transparencia) y mínimo (sin obligaciones).

### Actividad 2 — Sanción del GDPR [↑ Volver](#actividad-2-consulta-sobre-gdpr-y-sanciones-5-min)

La multa máxima es del **4% de la facturación global anual** o **20 millones de euros** (lo que sea mayor), según el Artículo 83 del GDPR.

Si Perplexity da una cifra diferente o no cita el Artículo 83, **desconfía**: es una posible alucinación.

### Actividad 3 — Detección de alucinaciones [↑ Volver](#actividad-3-detección-de-alucinaciones-5-min)

El ENS (RD 311/2022) no menciona explícitamente la IA, pues su última actualización es anterior al boom generativo. Si Perplexity cita artículos del ENS que hablan de "inteligencia artificial" textualmente, lo más probable es que esté **alucinando** o interpretando libremente.

**Señales de alarma de alucinación:**
- El enlace no funciona (404)
- El enlace existe pero no menciona lo que dice Perplexity
- La cita es vaga ("según el BOE") sin número concreto
- El artículo citado no existe en la normativa real

### Actividad 4 — Validación de tabla [↑ Volver](#actividad-4-extracción-estructurada-con-tabla-5-min)

| Normativa | Sanción máxima | Fuente esperada |
|-----------|---------------|-----------------|
| IA Act | 35M€ o 7% facturación global | eur-lex.europa.eu |
| GDPR | 20M€ o 4% facturación global | Art. 83, eur-lex.europa.eu |
| ENS | No económica (pérdida de certificación) | RD 311/2022, boe.es |

Si la tabla de Perplexity no coincide con estos valores, revisa las fuentes que citó: probablemente esté usando información desactualizada o interpretaciones de terceros sin autoridad.

---

[Volver a laboratorios](index.md)
