# 3.4 RAG y Fine-tuning

## Fine-Tuning vs. Modelos Destilados

| Aspecto | Fine-Tuning | Modelos Destilados |
|---------|-------------|-------------------|
| Proceso | Re-entrenar con datos propios | Modelo pequeño que imita a uno grande |
| Coste | Alto | Mucho más económico |
| Precisión | Muy alta en tareas acotadas | Buena, sacrifica capacidad general |
| Actualización | Requiere re-entrenar | Más fácil de actualizar |

## La Revolución del RAG

**RAG — Retrieval Augmented Generation:** Permite que el modelo responda basándose en tus propios documentos, no solo en su entrenamiento.

> Para el 90% de las empresas, RAG es la mejor estrategia inicial de implementación de IA con datos propios.

## ¿Qué es RAG?

Es como dar al modelo un libro abierto antes del examen:

1. **Busca en tus documentos:** El sistema recupera los fragmentos más relevantes.
2. **Los añade al prompt:** El contexto recuperado se inyecta junto a la pregunta.
3. **El LLM responde con evidencia:** La respuesta se basa en fuentes reales.

## Comparativa: Fine-Tuning vs. RAG

| Característica | Fine-Tuning | RAG |
|---------------|-------------|-----|
| Actualización de datos | Difícil (requiere re-entrenar) | Inmediata (subir archivo) |
| Transparencia | Opaco (caja negra) | Cita las fuentes utilizadas |
| Coste | Alto | Bajo / Medio |
| Alucinaciones | Posibles | Minimizadas |

## Privacidad de Datos Corporativos

**Riesgo: IAs Públicas** — Los planes gratuitos pueden usar conversaciones para reentrenar modelos.

**Solución: API / Enterprise** — Garantías contractuales: los datos no se usan para entrenar modelos.

---

[Volver al índice](index.md)
