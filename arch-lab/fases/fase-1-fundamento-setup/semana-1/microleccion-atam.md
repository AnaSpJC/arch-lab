# 🧠 Microlección 01 – Método ATAM (Architecture Tradeoff Analysis Method)

**Fecha:** 2025-08-30  
**Fase:** 1 – Fundamento y setup  
**Semana:** 1  
**Estado:** Completada  
**Autora:** Ana

---

## 🎯 Objetivo

Entender qué es ATAM, cómo se aplica en proyectos reales, y cómo usarlo para evaluar decisiones técnicas según atributos de calidad.

---

## 📘 1. Explicación clara y progresiva

### ¿Qué es ATAM?

ATAM es un método desarrollado por el Software Engineering Institute (SEI) para evaluar arquitecturas de software en función de sus atributos de calidad (como rendimiento, seguridad, mantenibilidad, etc.) y los trade-offs que implican las decisiones técnicas.

### ¿Para qué sirve?

- Entender las consecuencias de cada decisión arquitectónica  
- Identificar riesgos, sensibilidades y compensaciones  
- Priorizar atributos de calidad según el contexto del sistema

### ¿Cómo funciona?

ATAM se basa en escenarios de calidad: situaciones hipotéticas que ponen a prueba la arquitectura.  
Ejemplo: “El sistema debe responder en menos de 1 segundo cuando hay 100 usuarios simultáneos.”

Luego se analizan:
- Puntos de sensibilidad: decisiones que afectan varios atributos  
- Relaciones de intercambio (trade-offs): mejorar un atributo puede afectar otro  
- Riesgos: decisiones que pueden fallar o generar problemas futuros

---

## 🧩 2. Ejemplo narrativo aplicado a mi proyecto

**Proyecto:** Sistema de actividades y alertas

**Escenario de calidad:**  
“El sistema debe permitir registrar una actividad y emitir una alerta en menos de 2 segundos, incluso en una PC con recursos limitados.”

**Atributos involucrados:**  
- Rendimiento  
- Usabilidad  
- Mantenibilidad

**Decisión técnica:**  
Usar FastAPI + SQLite en local, sin procesos paralelos ni colas.

**Evaluación ATAM:**
- Sensibilidad: elección de base de datos afecta rendimiento y mantenibilidad  
- Trade-off: SQLite es liviana y fácil de mantener, pero no escala bien  
- Riesgo: si el sistema crece, SQLite puede volverse un cuello de botella

**Resultado:**  
Se acepta la decisión para el MVP, pero se documenta el riesgo en un ADR.

---

## 🔗 Fuente complementaria

- [Caso de estudio sobre ATAM – studocu.com](https://www.studocu.com/cl/document/universidad-nacional-andres-bello/teoria-de-la-arquitectura/caso-de-estudio-atam-metodologia-atam/68164821)

