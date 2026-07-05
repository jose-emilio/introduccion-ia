# 4.2 Fundamentos de Prompting

## Técnica 1: Acotar Roles

Asignar un rol experto al modelo reduce las respuestas genéricas.

**Ejemplo básico:** «Dame consejos financieros.» → vago, sin contexto

**Ejemplo experto:** «Actúa como auditor senior de riesgos financieros con 20 años de experiencia en banca europea...» → preciso y accionable

## Técnica 2: Dar Contexto

Especifica siempre: **audiencia** (¿para quién?), **objetivo** (¿para qué?) y **restricciones** (¿qué NO quieres?).

**Ejemplo:** «Escribe este reporte para el comité directivo; evita tecnicismos y no superes una página.»

## Técnica 3: Pedir Estructura

Solicita un formato de salida concreto: tablas, listas, pasos numerados, JSON.

**Ejemplo:** «Resume estos 10 emails en una tabla con columnas: Remitente, Prioridad, Acción requerida.»

## Prompts: De Nivel Básico a Experto

| | Prompt Básico | Prompt Experto |
|---|---|---|
| Ejemplo | «Haz un email para un cliente» | «Actúa como gestor de cuentas. Escribe un email de seguimiento B2B... Usa una tabla. Máximo 150 palabras.» |
| Resultado | Genérico, requiere edición | Casi listo para enviar |

## Técnica Avanzada: Iteración y Feedback

La IA mejora con cada corrección. Frases útiles: «Te has pasado de largo», «Usa menos adjetivos», «Hazlo más formal», «Añade ejemplos concretos».

---

[Volver al índice](index.md) | [Siguiente: 4.3 Desarrollo asistido con Copilot](03-desarrollo-copilot.md)
