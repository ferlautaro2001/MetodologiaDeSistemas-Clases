# 📘 Clase 4 - Gestión de Proyectos y Cultura Ágil

Apunte integrado para estudiar fases del proyecto, ciclo de vida del software, marcos de gestión, `Cynefin`, requerimientos y documentación ágil.

## Índice de Contenidos
- [🚀 1. Fases de Gestión de Proyectos](#-1-fases-de-gestión-de-proyectos)
- [🔄 2. Ciclo de Vida del Software](#-2-ciclo-de-vida-del-software)
- [🛠️ 3. Enfoques de Gestión](#️-3-enfoques-de-gestión)
- [🧭 4. Marco Cynefin](#-4-marco-cynefin)
- [⚡ 5. Cultura Ágil](#-5-cultura-ágil)
- [🎯 6. Ingeniería de Requerimientos](#-6-ingeniería-de-requerimientos)
- [🗺️ 7. Mapeo de Requerimientos](#️-7-mapeo-de-requerimientos)
- [📂 8. Documentación y Seguimiento](#-8-documentación-y-seguimiento)
- [🧪 9. Entornos y Usuarios](#-9-entornos-y-usuarios)

## 🚀 1. Fases de Gestión de Proyectos

| Fase | Objetivo | Salida esperada |
|---|---|---|
| **Ideación** | Detectar oportunidad | Idea priorizada |
| **Validación** | Confirmar valor/viabilidad | Hipótesis validadas |
| **Planeamiento estratégico** | Definir rumbo y riesgos | Plan con alcance y métricas |
| **Construcción** | Desarrollar la solución | Incrementos funcionales |
| **Lanzamiento (MVP)** | Salir al mercado | Feedback real de usuarios |

| Planeamiento estratégico: componentes | Para qué sirven |
|---|---|
| **Análisis de mercado** | Entender demanda y competencia |
| **Prueba de concepto** | Validar viabilidad técnica/negocio |
| **Gestión de riesgos** | Anticipar contingencias |
| **Selección de MVP** | Definir mínimo entregable de valor |
| **Gestión de stakeholders** | Alinear expectativas e intereses |

## 🔄 2. Ciclo de Vida del Software

| Etapa | Pregunta guía | Entregables típicos |
|---|---|---|
| **Análisis** | ¿Qué hay que resolver? | Requerimientos |
| **Diseño** | ¿Cómo lo estructuramos? | Modelos de datos y comportamiento |
| **Codificación** | ¿Cómo lo construimos? | Código + pruebas unitarias |
| **Pruebas** | ¿Funciona bien? | Pruebas de integración y regresión |
| **Implementación** | ¿Cómo llega al usuario? | Deploy, capacitación, soporte |

| Modelo | Secuencia |
|---|---|
| **Cascada** | Análisis -> Diseño -> Codificación -> Prueba -> Implementación |
| **Iterativo incremental** | Repite mini-ciclos en iteraciones para entregar valor parcial |

## 🛠️ 3. Enfoques de Gestión

| Enfoque | Fortalezas | Riesgos |
|---|---|---|
| **Predictivo (Cascada)** | Plan claro desde el inicio | Baja flexibilidad a cambios |
| **Ágil (Iterativo/Incremental)** | Aprendizaje rápido y adaptación | Requiere alta disciplina de equipo |
| **Híbrido** | Balance entre control y adaptación | Mayor complejidad de coordinación |

## 🧭 4. Marco Cynefin

- 🧠 **Autores:** C. F. Kurtz y D. J. Snowden.
- 🎯 **Uso:** decidir según el tipo de contexto/problema.

| Dominio | Contexto | Práctica recomendada | Patrón de acción |
|---|---|---|---|
| **Simple** | Causa-efecto clara | Mejores prácticas | Detectar → Clasificar → Responder |
| **Complicado** | Requiere análisis experto | Buenas prácticas | Detectar → Analizar → Responder |
| **Complejo** | Alta incertidumbre | Prácticas emergentes | Experimentar → Detectar → Responder |
| **Caótico** | Crisis inmediata | Prácticas novedosas | Actuar → Detectar → Responder |
| **Desorden** | Dominio no identificado | Reducir incertidumbre | Mover al dominio correcto |

## ⚡ 5. Cultura Ágil

| Valor ágil | Se prioriza por sobre |
|---|---|
| 👤 **Individuos e interacciones** | Procesos y herramientas |
| ✅ **Software funcionando** | Documentación extensiva |
| 🤝 **Colaboración con cliente** | Negociación contractual |
| 🔄 **Respuesta al cambio** | Seguir un plan rígido |

- 🧠 **Mentalidad:** cocrear valor con el usuario.
- 🧪 **Práctica:** iterar en ciclos cortos con feedback frecuente.
- 📉 **Objetivo:** minimizar desperdicio y retrabajo.

## 🎯 6. Ingeniería de Requerimientos

| Tipo | Qué define | Ejemplo |
|---|---|---|
| **Funcional** | Qué hace el sistema | Registrar usuario |
| **No funcional** | Cómo debe comportarse | Seguridad, performance |
| **Restricción** | Límites externos | Norma legal o tecnología obligatoria |

- 🧷 **Representación común:** `UML` (casos de uso) o historias de usuario.
- 📌 **Regla práctica:** un requerimiento útil debe ser claro, verificable y priorizable.

## 🗺️ 7. Mapeo de Requerimientos

| Elemento | Función |
|---|---|
| **Requerimiento** | Agrupa funcionalidades relacionadas |
| **Funcionalidades** | Se ordenan por precedencia y tiempo |
| **Herramientas de mapeo** | Casos de uso (`UML`) e historias de usuario |

| Requerimiento ejemplo | Funcionalidades asociadas |
|---|---|
| **Req. 1** | Funcionalidad 1, 2 y 3 |
| **Req. 2** | Funcionalidad 4, 5 y 6 |

## 📂 8. Documentación y Seguimiento

| Nivel | Alcance típico | Horizonte temporal |
|---|---|---|
| **Épica** | Gran iniciativa | ~3 meses |
| **Feature** | Bloque funcional | ~1 mes |
| **Historia de usuario** | Necesidad puntual | ~2 semanas |

| Estructura de historia de usuario | Plantilla |
|---|---|
| **Formato** | `Como [rol], quiero [funcionalidad], para [beneficio]` |
| **Obligatorio** | Criterios de aceptación |

| Flujo Kanban | Sentido práctico |
|---|---|
| `Backlog` → `Activo` → `QA` → `En revisión` → `Terminado` | Visualizar estado, limitar trabajo en curso y detectar cuellos de botella |

## 🧪 9. Entornos y Usuarios

| Entorno | Característica típica |
|---|---|
| **Desarrollo** | Máquina local del developer |
| **Testing** | Servidor compartido en red interna |
| **Producción** | Servidor final para usuarios (nube) |

| Tipo de usuario mencionado | Nota |
|---|---|
| **Early adopters** | Grupo clave para validar valor temprano |
