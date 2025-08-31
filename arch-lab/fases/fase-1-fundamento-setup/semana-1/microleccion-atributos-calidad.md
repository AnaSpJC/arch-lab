# 🧠 Microlección 02 – Atributos de calidad en arquitectura de software

**Fecha:** 2025-08-30  
**Fase:** 1 – Fundamento y setup  
**Semana:** 1  
**Estado:** Completada  
**Autora:** Ana

---

## 🎯 Objetivo

Comprender qué son los atributos de calidad, cómo se clasifican, cómo se priorizan según el contexto, y cómo se relacionan con decisiones arquitectónicas.

---

## 📘 1. Explicación clara y progresiva

### ¿Qué son los atributos de calidad?

Son **características no funcionales** que definen cómo debe comportarse un sistema más allá de “funcionar”.  
Ejemplo: no basta con que una API devuelva datos, debe hacerlo rápido, de forma segura, mantenible y escalable.

---

## 🧩 2. Clasificación de atributos clave

| Atributo | Qué significa | Ejemplo aplicado |
|----------|----------------|------------------|
| **Rendimiento (Performance)** | Qué tan rápido responde el sistema | La API devuelve actividades en <1s |
| **Mantenibilidad** | Qué tan fácil es modificar el sistema sin romperlo | Podés cambiar la lógica de alertas sin tocar la base |
| **Escalabilidad** | Qué tan bien crece el sistema ante más usuarios o datos | Podés pasar de SQLite a PostgreSQL sin rediseñar todo |
| **Disponibilidad** | Qué tan accesible está el sistema | El sistema funciona incluso si se cae una parte |
| **Seguridad** | Qué tan protegido está contra accesos indebidos | Solo usuarios autorizados pueden crear alertas |
| **Testabilidad** | Qué tan fácil es probar el sistema | Podés testear la lógica de actividades sin levantar el frontend |
| **Usabilidad** | Qué tan fácil es para el usuario final | La interfaz permite registrar actividades sin confusión |
| **Observabilidad** | Qué tan fácil es monitorear el sistema | Logs claros, métricas de respuesta, errores trazables |
| **Portabilidad** | Qué tan fácil es mover el sistema a otro entorno | Podés correrlo en tu PC o en otro servidor sin cambios grandes |
| **Modularidad** | Qué tan bien se separan las partes del sistema | Actividades y alertas están en módulos distintos |

---

## 🧠 3. ¿Cómo se priorizan?

No todos los atributos tienen el mismo peso en todos los proyectos.  
En tu sistema actual, por ejemplo:

- **Prioritarios:** mantenibilidad, rendimiento, testabilidad  
- **Secundarios:** escalabilidad, seguridad (por ahora), disponibilidad  
- **Latentes:** observabilidad, portabilidad (se activan en fases futuras)

# 👉 Cada ADR que escribas debe indicar qué atributos está priorizando.

---

## 🛠️ 4. Ejercicio práctico

Crear el archivo `atributos-priorizados.md` en `/docs/` con esta estructura:

```markdown
# 📋 Atributos de calidad priorizados – Proyecto Actividades y Alertas

**Fecha:** 2025-08-30  
**Versión:** 1.0

## 🔹 Prioritarios
- Mantenibilidad
- Rendimiento
- Testabilidad

## 🔸 Secundarios
- Escalabilidad
- Seguridad
- Usabilidad

## ⚪ Latentes
- Observabilidad
- Portabilidad
- Disponibilidad

## 🧠 Justificación
Se prioriza mantenibilidad para facilitar evolución curatorial.  
Rendimiento es clave por recursos limitados.  
Testabilidad permite validar lógica sin depender de interfaz.

