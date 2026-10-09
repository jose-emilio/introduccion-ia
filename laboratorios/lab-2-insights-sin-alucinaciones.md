# Laboratorio 2: Extracción de Insights sin Alucinaciones

**Módulo:** 3 — IA Generativa
**Duración estimada:** 15 min
**Tipo:** Ejercicio práctico individual
**Herramientas:** NotebookLM (notebooklm.google.com) o Gemini (gemini.google.com)

---

## Objetivos

Al completar este laboratorio, podrás:

- Analizar grandes volúmenes de texto con IA minimizando el riesgo de alucinaciones
- Crear una FAQ automática a partir de un documento extenso
- Verificar que la IA cita la fuente exacta dentro del documento original

---

## ¿Qué vas a necesitar?

- Un navegador web
- Acceso a NotebookLM (notebooklm.google.com) o Gemini (gemini.google.com) en su versión gratuita
- Un documento público extenso (el informe anual de una empresa o un pliego de condiciones)

---

## ¿Por qué es importante este laboratorio?

Los LLMs alucinan: inventan datos con apariencia de verdad. En entornos corporativos, una cifra inventada en un informe financiero o un riesgo mal identificado en una licitación puede tener consecuencias graves.

Herramientas como **NotebookLM** o **Gemini** permiten «anclar» las respuestas a un documento real que tú subes, forzando a la IA a citar la fuente exacta. Así reduces drásticamente las alucinaciones y garantizas la trazabilidad.

---

## Actividad 1: Consigue tu documento (2 min)

Necesitas un documento público extenso (mínimo 15-20 páginas). Elige UNO:

| Opción | Dónde conseguirlo |
|---|---|
| **Informe anual de una empresa** | Busca en Google "[nombre empresa] informe anual 2025 PDF" |
| **Pliego de condiciones de una licitación** | Busca en Google "pliego de condiciones licitación PDF" |
| **Memoria de sostenibilidad** | Busca en Google "memoria de sostenibilidad 2025 PDF" |
| **Un documento largo que ya tengas** | Asegúrate de que sea público y no contenga datos confidenciales |

> **Importante:** Usa solo documentos públicos. No subas datos confidenciales de tu empresa. Este laboratorio es para practicar la técnica.

**Nombre del documento que elegiste:** _________________________________

**URL o ruta del archivo:** ____________________________________________

---

## Actividad 2: Sube el documento a la herramienta (3 min)

### Si usas NotebookLM (recomendado):

1. Abre https://notebooklm.google.com e inicia sesión con tu cuenta de Google.
2. Crea un nuevo cuaderno: haz clic en **"Nuevo cuaderno"** y asígnale un nombre (ej: "Lab 2 - Insights").
3. Haz clic en **"Añadir fuente"** y selecciona tu archivo PDF.
4. Espera a que NotebookLM lo procese e indexe (suelen ser unos segundos).

### Si usas Gemini:

1. Abre https://gemini.google.com e inicia sesión con tu cuenta de Google.
2. Busca el icono de **subir archivo** (clip o +) junto al campo de texto.
3. Selecciona tu PDF y espera a que se procese.

**Marca aquí cuando lo hayas hecho:**
- [ ] He subido el documento a la herramienta
- [ ] La herramienta lo ha procesado sin errores

---

## Actividad 3: Crea una FAQ automática (4 min)

Pide a la herramienta que genere una FAQ basada exclusivamente en el documento que acabas de subir.

### Con NotebookLM

Escribe este prompt exacto en el chat del cuaderno:

> "Genera una FAQ con las 5 preguntas más importantes que cualquier lector debería hacerse sobre este documento. Para cada respuesta, cita el fragmento exacto del documento del que has extraído la información, indicando el número de página o sección."

### Con Gemini

Pega este prompt después de haber subido el archivo:

> "He subido un documento PDF. Genera una FAQ con las 5 preguntas más importantes sobre su contenido. Para cada respuesta, indica la fuente exacta dentro del documento (número de página o sección) de donde has extraído la información."

Pulsa Enter y observa el resultado.

**Pega aquí la FAQ que obtuviste:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

**Responde:**
1. ¿Cada respuesta incluye la fuente exacta (página o sección)? ______
2. ¿Las preguntas cubren los temas más importantes del documento? ______
3. ¿Confiarías en esta FAQ para usarla en tu trabajo? ¿Por qué? ________

---

## Actividad 4: Preguntas cruzadas complejas (4 min)

Ahora vas a forzar a la IA a cruzar información de diferentes partes del documento. Esto es donde las alucinaciones son más probables si la herramienta no cita fuentes.

Elige la pregunta que corresponda al tipo de documento que subiste:

**Si subiste un informe anual o memoria financiera:**
> "¿Cuáles son los tres principales riesgos operativos mencionados en el documento y cómo afectan al presupuesto o resultados financieros? Para cada riesgo, indica la página exacta donde se menciona y la página donde aparece su impacto económico."

**Si subiste un pliego de condiciones o licitación:**
> "¿Cuáles son los tres requisitos técnicos más estrictos que debe cumplir el licitador y qué penalizaciones aplican en caso de incumplimiento? Para cada requisito, indica la página donde se define y la página donde se especifica la penalización."

**Si subiste otro tipo de documento:**
> "Identifica los 3 datos o cifras más importantes del documento. Para cada uno, indica: (1) qué dice exactamente, (2) en qué página aparece y (3) si hay alguna discrepancia o contradicción con otra parte del documento."

Pega la pregunta en el chat y pulsa Enter.

**Pega aquí la respuesta:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

**Responde:**
1. ¿La respuesta cita páginas o secciones diferentes para cada punto? ______
2. ¿Puedes abrir el documento en esas páginas y verificar que la cita es correcta? ______
3. Si la IA hubiera alucinado, ¿cómo lo detectarías gracias a las citas? ______

---

## Actividad 5: Prueba de verificación (2 min)

Elige UNA de las citas que te devolvió la IA en la Actividad 4 y verifícala manualmente:

1. Abre tu documento PDF.
2. Navega hasta la página o sección que citó la IA.
3. Comprueba si el contenido coincide exactamente con lo que dijo la IA.

**Cita a verificar:**
> _________________________________________

**Página que indica la IA:** _________

**¿Coincide con el documento real?** [ ] Sí [ ] No

**Si no coincide, ¿qué dijo la IA y qué dice realmente el documento?**
> _________________________________________________________________

---

## Resumen del laboratorio

- [ ] Elegí y descargué un documento público extenso
- [ ] Lo subí a NotebookLM o Gemini
- [ ] Generé una FAQ automática con fuentes citadas
- [ ] Hice una pregunta compleja que cruza información de distintas partes
- [ ] Verifiqué manualmente al menos una cita contra el documento real

---

## Soluciones

### Actividad 3 — ¿Qué esperar de la FAQ? [↑ Volver](#actividad-3-crea-una-faq-automática-4-min)

Una FAQ bien generada debe tener esta estructura para cada pregunta:

**Pregunta:** ¿Cuál fue el ingreso total en 2025?
**Respuesta:** El ingreso total fue de 12.450M€ (Fuente: pág. 15, Estado de Resultados).
**Pregunta:** ¿Qué mercados geográficos crecieron más?
**Respuesta:** América Latina creció un 23% y Asia-Pacífico un 18% (Fuente: pág. 22, Desglose por región).

Si alguna respuesta **no incluye fuente**, desconfía: podría ser una alucinación.

### Actividad 4 — Verificación cruzada [↑ Volver](#actividad-4-preguntas-cruzadas-complejas-4-min)

Una respuesta fiable debe citar **más de una página** para cada punto. Por ejemplo:

> **Riesgo 1: Volatilidad del tipo de cambio** (pág. 18)
> **Impacto:** Reducción del margen operativo en 2,3 puntos porcentuales (pág. 42)

Si la IA solo da una respuesta genérica sin páginas, o si todas las citas apuntan a la misma página, probablemente no está extrayendo realmente de todo el documento.

### Actividad 5 — ¿Qué hago si la IA alucinó? [↑ Volver](#actividad-5-prueba-de-verificación-2-min)

Si la cita no coincide:
1. **Reformula la pregunta** añadiendo: "Verifica que tu respuesta sea textual del documento. Si no encuentras la información, dímelo en lugar de inventarla."
2. **Vuelve a preguntar** por un fragmento más concreto.
3. Si la herramienta insiste en el error, reporta el incidente: esa fuente no es fiable para ese tipo de consulta.

La trazabilidad (que la IA muestre la página exacta) es tu principal defensa contra las alucinaciones. Sin ella, cualquier respuesta puede ser inventada.

---

[Volver a laboratorios](index.md)
