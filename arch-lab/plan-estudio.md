# 🧭 Programa curatorial – Arquitectura de Software

**Autora:** Ana  
**Versión:** 1.0  
**Duración estimada:** 6–9 meses  
**Objetivo:** Consolidar una base sólida en arquitectura de software aplicada, con evidencia curatorial, proyectos reales y documentación profesional.

---

## 🧱 Pilares del aprendizaje

| Pilar | Por qué importa | Qué producir | Recursos clave |
|-------|------------------|--------------|----------------|
| Fundamentos de arquitectura | Te da lenguaje y criterio (atributos de calidad, estilos, trade-offs) | Resumen de estilos, catálogo de atributos, 6–8 ADRs | Guía y katas de arquitectura (ES), curso Univ. Alberta (auditar) |
| Documentación visual | Comunica decisiones sin fricción | 1 set de diagramas C4 por proyecto | diagrams.net (offline), PlantUML/Mermaid |
| Proyecto “monolito bien diseñado” | Demuestra mantenibilidad sin usar cloud ni contenedores | API + PWA con capas/hexagonal, tests, ADRs | Stack: Python + SQLite; PWA vanilla/React liviano |
| Arquitectura aplicada (katas) | Practicás trade-offs en problemas nuevos | 6–10 katas breves con solución argumentada | Katas de arquitectura |
| Calidad y automatización mínima | Disciplina profesional sin consumo de recursos | Tests, lint, pre-commit, CI simple | GitHub Actions básicos (si hay conectividad) |
| Presentación y empleabilidad | Convertís tu proceso en evidencia | README curatorial, changelog, demo local, CV orientado a arquitectura | Plantillas de ADR, portafolio en GitHub |

---

## 📅 Fases del plan

### 🔹 Fase 1 (Semanas 1–4) — Fundamento y setup

- Estilos arquitectónicos: capas, hexagonal, event-driven, microservicios
- Atributos de calidad: mantenibilidad, performance, seguridad, observabilidad
- Evaluación de trade-offs: método ATAM aplicado
- Herramientas livianas: VS Code/VSCodium, Git, Python 3.x, SQLite, diagrams.net
- Hábitos curatoriales: repo `arquitectura-lab`, carpetas para notas, ADRs y katas

### 🔹 Fase 2 (Semanas 5–8) — Proyecto principal sin “nube”

- Dominio elegido: sistema de actividades y alertas con trazabilidad
- Arquitectura: capas o hexagonal; persistencia en SQLite; API REST; frontend PWA
- Evidencias: 6–8 ADRs, diagramas C4 (Contexto, Contenedores, Componentes), tests, métricas básicas, checklist de atributos

### 🔹 Fase 3 (Semanas 9–12) — Katas y refinamiento

- Katas de arquitectura: 2 por semana con contexto, atributos, alternativas, decisión y consecuencias
- Refactor arquitectónico: aislamiento de módulos críticos, interfaz para notificaciones, medición de impacto

### 🔹 Fase 4 (Meses 4–6+) — Señales al mercado

- Segundo proyecto breve: variante event-driven local (sin Kafka, solo colas en memoria/archivo)
- Empleabilidad: CV/LinkedIn orientado a “desarrollo con enfoque arquitectónico”; destacar ADRs, decisiones y trade-offs
- Posicionamiento: roles de developer senior/semisenior, tech lead en pymes, arquitectura aplicativa

---

## 📎 Fuentes recomendadas

- Curso auditable: *Arquitectura de Software* – Universidad de Alberta (Coursera)
- Guías y katas: Manuel Zapata (blog y repositorios en español)
- Diagramación: [diagrams.net](https://app.diagrams.net/), [Mermaid](https://mermaid-js.github.io/), [PlantUML](https://plantuml.com/)
- Documentación técnica: ADRs (MADR), C4 Model, changelog curatorial

---

## ✍️ Notas curatoriales

Este plan está vivo. Se versiona, se adapta y se documenta. Cada fase incluye entregables técnicos y reflexiones curatoriales. El objetivo no es solo aprender, sino **mostrar cómo se aprende**.

