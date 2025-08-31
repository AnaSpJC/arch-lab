# ADR 0003 – Evaluación ATAM: Registro de actividades y alertas

**Escenario de calidad:**  
“El sistema debe registrar una actividad y emitir una alerta en menos de 2 segundos en una PC modesta.”

**Atributos priorizados:**  
- Rendimiento  
- Usabilidad  
- Mantenibilidad

- [Ver atributos priorizados](../docs/atributos-priorizados.md)


**Decisión técnica:**  
FastAPI + SQLite en local

**Análisis ATAM:**  
- Sensibilidad: base de datos afecta rendimiento y mantenibilidad  
- Trade-off: simplicidad vs escalabilidad  
- Riesgo: SQLite puede limitar crecimiento futuro

**Conclusión:**  
Se acepta para MVP. Se revisará en fase de escalabilidad.
