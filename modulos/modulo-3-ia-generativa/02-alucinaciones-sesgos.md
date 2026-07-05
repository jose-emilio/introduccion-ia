# 3.2 Alucinaciones y Sesgos

## ¿Por qué ocurren las alucinaciones?

Una alucinación ocurre cuando el modelo genera información que suena plausible pero es incorrecta o inventada.

- **Naturaleza probabilística:** El modelo busca la respuesta más coherente, no necesariamente la más veraz.
- **Sin acceso a datos en tiempo real:** Los LLMs tienen una fecha de corte de entrenamiento.
- **Presión por responder:** El modelo raramente admite ignorancia.

## El Riesgo de la Verosimilitud

> «Una alucinación peligrosa es aquella que suena perfectamente lógica pero es totalmente falsa.»

**¿Cuándo es crítico?**
- Informes legales o contractuales con datos fabricados
- Consultas médicas o de cumplimiento normativo
- Análisis financieros con cifras inventadas

**Cómo mitigarlo:**
- Implementar sistemas RAG que anclen las respuestas a fuentes verificadas
- Exigir que el modelo cite la fuente
- Establecer revisión humana en flujos de alto riesgo

---

[Volver al índice](index.md) | [Siguiente: 3.3 Modelos actuales](03-modelos-actuales.md)
