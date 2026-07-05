# 3.1 LLMs, Tokens y Contexto

## ¿Qué son los LLMs?

**Large Language Models (LLMs):** Grandes Modelos de Lenguaje que impulsan herramientas como ChatGPT, Gemini y Claude.

Se entrenan con billones de palabras procedentes de libros, artículos, código y páginas web. El resultado es un modelo estadístico del lenguaje capaz de entender estructura, matiz e intención.

> Un LLM no recupera fragmentos guardados como una base de datos. Ha internalizado patrones de relación entre ideas, palabras y conceptos.

## El Ciclo de Predicción

```
Entrada → Codificación → Atención → Predicción
```

Cada token generado retroalimenta el proceso, manteniendo coherencia a lo largo de textos largos.

## La Revolución de los Transformers

**2017:** El paper «Attention is All You Need» introdujo la arquitectura Transformer, que permite procesar párrafos enteros de forma simultánea. El mecanismo de atención permite al modelo entender el contexto completo.

## ¿Qué es un Token?

Un token es la unidad mínima que procesa el modelo. 100 tokens equivalen aproximadamente a 75 palabras en inglés.

**¿Por qué importa?**
- **Coste:** Las APIs se facturan por tokens consumidos.
- **Límites:** La ventana de contexto se mide en tokens.

## Eficiencia por Idioma

Los LLMs se entrenaron mayoritariamente en inglés. El español consume más tokens por su morfología flexiva, incrementando el coste de API en un 20-25%.

## Ventana de Contexto de Modelos Actuales

| Modelo | Ventana de Contexto | Equivalencia |
|--------|-------------------|--------------|
| GPT-5.5 (OpenAI) | 1M tokens | ~3 000 páginas |
| Claude Sonnet 5 (Anthropic) | 1M tokens | ~3 000 páginas |
| Gemini 3.1 Pro (Google) | 1M tokens | ~3 000 páginas |

---

[Volver al índice](index.md) | [Siguiente: 3.2 Alucinaciones y sesgos](02-alucinaciones-sesgos.md)
