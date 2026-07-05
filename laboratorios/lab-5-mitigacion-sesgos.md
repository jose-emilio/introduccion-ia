# Laboratorio 5: Mitigación Activa de Sesgos en la Redacción Corporativa

**Módulo:** 5 — Ética, Regulación y Gobernanza de la IA
**Duración estimada:** 30 min
**Tipo:** Ejercicio práctico individual
**Herramientas:** ChatGPT (chat.openai.com) o Gemini (gemini.google.com)

---

## Objetivos

Al completar este laboratorio, podrás:

- Detectar sesgos de género, raza, cultura e idioma en textos e imágenes generados por IA
- Aplicar técnicas de prompting (rol, contexto e inyección de perspectiva) para obtener resultados neutrales e inclusivos
- Evaluar críticamente borradores corporativos y usar la autocrítica del modelo para corregirlos
- Auditar el sesgo visual en imágenes generadas por IA

---

## ¿Qué vas a necesitar?

- Un navegador web
- Acceso a **ChatGPT** (chat.openai.com) o **Gemini** (gemini.google.com) en su versión gratuita
- Un documento para anotar tus observaciones

---

## ¿Por qué es importante este laboratorio?

Los LLMs se entrenan con textos de internet escritos por humanos. Si internet contiene sesgos históricos, el modelo los absorbe y los amplifica con apariencia de objetividad. Una oferta de empleo, un comunicado interno o un perfil de puesto redactado por IA puede perpetuar estereotipos sin que quien lo escribe sea consciente.

> La IA no es neutral: refleja los sesgos de sus datos de entrenamiento. Detectarlos y corregirlos es responsabilidad del profesional.

---

## Actividad 1: Prompt genérico — detecta el sesgo (5 min)

### Paso 1: Solicita un borrador con prompt genérico

Abre ChatGPT o Gemini y escribe **exactamente** este prompt:

> *"Redacta una comunicación interna anunciando la búsqueda de un nuevo director de ventas para la empresa. Describe el perfil ideal y las cualidades que debe tener."*

Pulsa Enter y observa el resultado.

**Pega aquí el texto que generó:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 2: Evalúa críticamente el texto

Relee el texto generado y responde:

**Sesgo de género:**
- ¿El texto usa genéricos masculinos ("el director", "el candidato", "él") por defecto? [ ] Sí [ ] No
- ¿Alterna entre masculino y femenino o usa formas neutras? [ ] Sí [ ] No
- ¿Las cualidades descritas están asociadas a estereotipos masculinos ("agresivo", "competitivo", "dominante")? [ ] Sí [ ] No

**Sesgo de diversidad:**
- ¿El perfil asume implícitamente cierta edad, procedencia o disponibilidad? [ ] Sí [ ] No
- ¿Menciona explícitamente que la empresa valora la diversidad e inclusión? [ ] Sí [ ] No

**Sesgo de idioma:**
- ¿Asume que el candidato debe ser nativo en un idioma específico sin justificación? [ ] Sí [ ] No

**Anota aquí los sesgos que detectaste:**
> _________________________________________________________________
> _________________________________________________________________

---

## Actividad 2: Redacta con rol y contexto — prompt neutral (7 min)

### Paso 1: Reescribe el prompt con técnicas de mitigación

Ahora vas a aplicar las técnicas de **rol** y **contexto** para forzar a la IA a ser neutral e inclusiva.

Copia esta plantilla y complétala con los detalles de tu empresa:

> *"Actúa como un responsable de diversidad e inclusión con 10 años de experiencia en comunicación corporativa. Redacta una comunicación interna anunciando la búsqueda de un nuevo director de ventas. Requisitos obligatorios:*
> - *Utiliza lenguaje inclusivo durante todo el texto (alterna géneros, usa formas neutras como 'la persona candidata' cuando sea posible).*
> - *Describe cualidades profesionales sin asociarlas a estereotipos de género.*
> - *Incluye una frase explícita sobre el compromiso de la empresa con la diversidad e inclusión.*
> - *No asumas edad, procedencia ni situación familiar.*
> - *Destaca que la empresa valora perfiles diversos y experiencias variadas.*
> *La empresa es [nombre de tu empresa], del sector [sector], con [X] empleados. La comunicación va dirigida a toda la plantilla por correo interno."*

**Tu prompt completo:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 2: Ejecuta el nuevo prompt

Pega el prompt completo en el chat y pulsa Enter.

**Pega aquí el nuevo texto generado:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 3: Compara los resultados

| Aspecto | Prompt genérico (Act. 1) | Prompt con rol y contexto (Act. 2) |
|---------|-------------------------|-----------------------------------|
| ¿Usa lenguaje inclusivo? | [ ] Sí [ ] No | [ ] Sí [ ] No |
| ¿Alterna géneros o usa neutros? | [ ] Sí [ ] No | [ ] Sí [ ] No |
| ¿Menciona diversidad explícitamente? | [ ] Sí [ ] No | [ ] Sí [ ] No |
| ¿Evita estereotipos? | [ ] Sí [ ] No | [ ] Sí [ ] No |
| ¿Lo publicarías tal cual? | [ ] Sí [ ] No | [ ] Sí [ ] No |

**Responde:**
1. ¿Qué diferencias notas entre ambos textos? _________________________________
2. ¿El segundo texto sigue teniendo algún sesgo sutil? _________________________________
3. ¿Crees que sin un prompt explícito la IA sería naturalmente inclusiva? _________________________________

---

## Actividad 3: Caso extremo — perfil de puesto sin sesgo (5 min)

### Paso 1: Perfil genérico (sesgado)

Escribe este prompt:

> *"Redacta el perfil de un ingeniero informático para una oferta de empleo. Describe las habilidades técnicas y personales necesarias."*

Pulsa Enter y analiza el resultado.

**¿Qué sesgos detectas?**
> _________________________________________________________________

### Paso 2: Perfil neutral forzado

Ahora escribe:

> *"Actúa como un reclutador especializado en contratación inclusiva. Redacta una oferta de empleo para un puesto de ingeniería informática. Requisitos obligatorios:*
> - *Lenguaje inclusivo durante todo el texto.*
> - *Las habilidades personales no deben estar asociadas a estereotipos de género.*
> - *Incluye una frase sobre igualdad de oportunidades y diversidad.*
> - *No uses 'él' como pronombre por defecto.*
> - *Especifica que la empresa anima a postularse a mujeres, minorías y otros grupos infrarrepresentados en el sector tecnológico.*
> *La empresa es [nombre de tu empresa], una empresa tecnológica con 200 empleados."*

**Pega aquí el perfil neutral generado:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 3: Contraste final

Compara ambos perfiles:

| Elemento | Perfil genérico | Perfil neutral forzado |
|----------|----------------|----------------------|
| Pronombre por defecto | | |
| Cualidades personales | | |
| ¿Incluye diversidad? | | |
| ¿Lo usarías en una oferta real? | | |

---

## Actividad 4: Inyección de perspectiva — autocrítica del modelo (5 min)

Una técnica avanzada para detectar sesgos es pedir al propio modelo que evalúe su respuesta desde diferentes perspectivas.

### Paso 1: Pide una autocrítica

Toma el texto que generaste en la **Actividad 2** (el prompt neutral) y pégalo en un nuevo chat. A continuación, añade este prompt:

> *"Evalúa críticamente el texto anterior desde tres perspectivas:*
> - *Perspectiva de género: ¿hay algún sesgo de género implícito?*
> - *Perspectiva cultural: ¿asume valores o referencias culturales occidentales sin justificación?*
> - *Perspectiva de diversidad funcional: ¿excluye implícitamente a personas con discapacidad?*
> *Para cada perspectiva, indica: (1) qué problema detectas, (2) en qué frase concreta aparece y (3) cómo lo corregirías."*

Pulsa Enter.

**Pega aquí la autocrítica del modelo:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 2: Aplica las correcciones

Pide al modelo que reescriba el texto original incorporando las correcciones que él mismo sugirió:

> *"Reescribe el texto original incorporando todas las correcciones que acabas de sugerir. El resultado debe ser un texto inclusivo en género, cultura y diversidad funcional."*

**Pega aquí el texto corregido tras la autocrítica:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 3: Comprobación final

Pasa el texto corregido por esta verificación:

| Requisito | Cumple |
|-----------|--------|
| ¿Usa lenguaje inclusivo de género? | [ ] Sí [ ] No |
| ¿Evita referencias culturales exclusivas de un país o región? | [ ] Sí [ ] No |
| ¿Incluye consideraciones de accesibilidad o diversidad funcional? | [ ] Sí [ ] No |
| ¿El tono sigue siendo profesional y adecuado para una comunicación interna? | [ ] Sí [ ] No |

**Responde:**
1. ¿La IA fue capaz de autodetectar sus propios sesgos? ______
2. ¿Las correcciones que sugirió fueron sustanciales o superficiales? ______
3. ¿Aplicarías esta técnica de "doble prompt" (generar + autoevaluar) en tu trabajo diario? ______

---

## Actividad 5: Auditoría de sesgo visual — el caso de la imagen corporativa (5 min)

**Nota:** Esta actividad es opcional solo si usas una herramienta con generación de imágenes (ChatGPT con DALL-E, Gemini con Imagen). Si no, haz el ejercicio de forma teórica.

### Paso 1: Genera una imagen con prompt neutro

Escribe en el chat:

> *"Genera la imagen de una persona exitosa en los negocios. La imagen será usada en la web corporativa de la empresa."*

Si tu herramienta no genera imágenes, pasa al Paso 2 directamente y haz el análisis conceptual.

**Pega aquí la descripción de la imagen generada:**
> _________________________________________________________________

### Paso 2: Análisis de sesgo visual

Responde sobre la imagen (o sobre lo que esperarías):

- ¿La persona aparece como hombre o mujer? ______
- ¿Su apariencia física corresponde a un grupo étnico predominante? ______
- ¿Lleva ropa formal occidental? [ ] Sí [ ] No
- ¿La postura y expresión facial transmiten poder, cercanía u otra cosa? ______
- ¿Hay diversidad en la imagen si salen varias personas? ______

### Paso 3: Prompt corregido para inclusión visual

Ahora escribe:

> *"Genera 3 imágenes variadas de personas exitosas en los negocios para una web corporativa. Requisitos obligatorios:*
> - *Diversidad de género: incluye hombres y mujeres.*
> - *Diversidad étnica: distintas procedencias y tonos de piel.*
> - *Diversidad de edad: desde los 30 hasta los 60 años.*
> - *Ropa profesional variada (no solo traje occidental).*
> - *Posturas diversas: algunas colaborando, otras liderando, otras innovando.*
> *Las imágenes deben ser realistas y profesionales."*

**Compara las imágenes generadas con el primer resultado. ¿Hay mejora en diversidad?**
> _________________________________________________________________

---

## Actividad 6: Reflexión y guía práctica (3 min)

Basándote en lo que has experimentado en todo el laboratorio, completa esta guía de mitigación:

**Para evitar sesgos de género:**
> _____________________________________________________________

**Para evitar sesgos de raza o cultura:**
> _____________________________________________________________

**Para evitar presunciones de edad o situación personal:**
> _____________________________________________________________

**Lista de verificación para revisar cualquier texto generado por IA antes de publicarlo:**
- [ ] ¿Alterna géneros o usa lenguaje neutro?
- [ ] ¿Las cualidades no están asociadas a estereotipos?
- [ ] ¿Incluye una declaración de diversidad e inclusión?
- [ ] ¿Evita asunciones sobre edad, procedencia o situación familiar?
- [ ] ¿El tono es profesional sin sesgos implícitos?

---

## Resumen del laboratorio

- [ ] Solicité un borrador con prompt genérico y detecté sesgos (Act. 1)
- [ ] Reescribí el prompt con rol y contexto para forzar neutralidad (Act. 2)
- [ ] Repetí el ejercicio con un perfil de puesto técnico (Act. 3)
- [ ] Apliqué inyección de perspectiva para autocrítica del modelo (Act. 4)
- [ ] Analicé sesgo visual en generación de imágenes corporativas (Act. 5)
- [ ] Creé mi guía personal de mitigación de sesgos (Act. 6)

---

## Soluciones

### Actividad 1 — Sesgos típicos en el prompt genérico [↑ Volver](#actividad-1-prompt-genérico--detecta-el-sesgo-5-min)

| Sesgo | Lo que suele aparecer |
|-------|----------------------|
| **Género** | "El candidato debe ser...", "buscamos a un director..." (masculino por defecto) |
| **Estereotipos** | "Liderazgo fuerte", "capacidad de imponerse", "competitivo" (cualidades asociadas culturalmente a hombres) |
| **Edad** | "Buscamos talento joven", "recién titulado" (implícito) |
| **Disponibilidad** | "Disponibilidad para viajar constantemente", "dedicación exclusiva" (asume que el candidato no tiene cargas familiares) |

### Actividad 2 — Frases recomendadas para inclusión [↑ Volver](#actividad-2-redacta-con-rol-y-contexto--prompt-neutral-7-min)

| Para incluir | Ejemplo textual |
|-------------|----------------|
| Lenguaje neutro | "La persona candidata", "dirección", "liderazgo del equipo" |
| Diversidad explícita | "Valoramos positivamente candidaturas de perfiles diversos" |
| Alternancia | Usar "el/la responsable" o redactar en plural "las personas del equipo" |

### Actividad 3 — Perfil de puesto: antes y después [↑ Volver](#actividad-3-caso-extremo--perfil-de-puesto-sin-sesgo-5-min)

**Perfil genérico típico:** "Buscamos un ingeniero informático con capacidad de liderazgo, resolutivo y con disponibilidad para viajar. Valoraremos positivamente candidatos jóvenes con energía."

**Perfil neutral:** "Buscamos una persona con formación en ingeniería informática para incorporarse a nuestro equipo técnico. Valoramos la capacidad de resolución de problemas, el trabajo en equipo y la diversidad de perspectivas. Animamos especialmente a postularse a mujeres y otros grupos infrarrepresentados en el sector."

### Actividad 4 — Inyección de perspectiva [↑ Volver](#actividad-4-inyección-de-perspectiva--autocrítica-del-modelo-5-min)

| Técnica | Cómo aplicarla | Ejemplo de prompt |
|---------|---------------|------------------|
| **Autoevaluación** | Pedir al modelo que critique su propio output | "Evalúa tu respuesta anterior desde perspectiva de género, cultura y diversidad funcional" |
| **Inyección de perspectiva** | Forzar al modelo a considerar puntos de vista alternativos | "Reescribe el texto desde la perspectiva de una persona con discapacidad visual" |
| **Doble prompt** | Generar + autoevaluar + corregir en 3 pasos | Secuencia: prompt inicial → crítica → reescritura |

La técnica de **doble prompt** es especialmente potente porque aprovecha que el modelo suele detectar mejor los sesgos en un texto ya escrito que al generarlo desde cero.

### Actividad 5 — Sesgo visual [↑ Volver](#actividad-5-auditoría-de-sesgo-visual--el-caso-de-la-imagen-corporativa-5-min)

Los modelos de generación de imágenes (DALL-E, Imagen, Midjourney) tienen sesgos aún más acusados que los de texto:

| Sesgo visual típico | Lo que suele aparecer | Cómo mitigarlo |
|--------------------|----------------------|---------------|
| **Género** | Hombre trajeado como "executive" | Especificar "hombres y mujeres en posiciones de liderazgo" |
| **Etnia** | Personas caucásicas por defecto | Incluir "diversidad étnica: personas de distintas procedencias" |
| **Edad** | Profesionales de 30-40 años | Especificar rango: "desde los 25 hasta los 65 años" |
| **Contexto** | Oficinas modernas occidentales | Describir entornos variados si aplica |
| **Ropa** | Traje y corbata como estándar | Indicar "vestimenta profesional variada" |

### Actividad 6 — Guía práctica de mitigación [↑ Volver](#actividad-6-reflexión-y-guía-práctica-3-min)

**Regla de oro:** Si el prompt no especifica neutralidad, la IA replicará los sesgos mayoritarios de sus datos de entrenamiento. La mitigación no es opcional: es parte de la instrucción.

Las tres técnicas más efectivas son:
1. **Rol especializado** ("actúa como un responsable de diversidad")
2. **Contexto explícito** ("la empresa valora la inclusión")
3. **Restricciones concretas** ("no uses 'él' como pronombre por defecto, alterna géneros")

**Y una cuarta avanzada:**
4. **Doble prompt o inyección de perspectiva** — genera, pide una autocrítica y reescribe incorporando las correcciones.

---

[Volver a laboratorios](index.md)
