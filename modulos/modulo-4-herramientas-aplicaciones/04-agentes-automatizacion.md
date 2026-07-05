# 4.4 Agentes y Automatización

## ¿Qué es un Agente de IA?

Un LLM con acceso a herramientas externas y capacidad de razonamiento multi-paso para cumplir objetivos complejos de forma autónoma.

**Tres capacidades clave:**
- **Memoria:** Retiene contexto entre pasos
- **Planificación:** Descompone objetivos en subtareas
- **Ejecución:** Llama a APIs, navega la web y lee archivos

## Model Context Protocol (MCP)

Estándar abierto que permite a cualquier modelo conectarse a cualquier fuente de datos o herramienta.

```
Cliente (LLM) ←→ Servidor MCP ←→ Fuente de Datos
```

## Frameworks de Agentes

| Framework | Enfoque | Nivel de Control |
|-----------|---------|-----------------|
| **CrewAI** | Equipos de agentes con roles jerárquicos | Alto |
| **AutoGen** | Conversación dinámica entre agentes | Muy Alto |
| **LangGraph** | Grafos de control explícitos (DAGs) | Máximo |

## Copilot Studio

| | Agent Builder | Copilot Studio |
|---|---|---|
| Perfil | No-code, agentes departamentales rápidos | Plataforma empresarial |
| Complejidad | Baja | Alta |
| Integraciones | SharePoint, documentos | SAP, Salesforce, SQL |

## Casos de Uso Empresarial

- **RRHH:** Agente de selección que lee CVs, puntúa candidatos y agenda entrevistas
- **Ventas:** Actualización automática de CRM tras llamadas y reuniones
- **Soporte:** Resolución autónoma de incidencias técnicas

---

[Volver al índice](index.md)
