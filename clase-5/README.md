# 🧩 Clase 5 - Proceso Unificado y Casos de Uso

Apunte de estudio para dominar el `Proceso Unificado (UP)` y la captura de requisitos guiada por `casos de uso`.

## Índice de Contenidos
- [🚀 1. Qué es el Proceso Unificado](#-1-qué-es-el-proceso-unificado)
- [🔄 2. Fases del Proceso Unificado](#-2-fases-del-proceso-unificado)
- [📌 3. Principios Clave](#-3-principios-clave)
- [🎯 4. Captura de Requisitos](#-4-captura-de-requisitos)
- [🧠 5. Casos de Uso](#-5-casos-de-uso)
- [🛠️ 6. Estructura de un Caso de Uso](#️-6-estructura-de-un-caso-de-uso)
- [🏛️ 7. Casos de Uso y Arquitectura](#️-7-casos-de-uso-y-arquitectura)
- [🔁 8. Casos de Uso en el Ciclo de Vida](#-8-casos-de-uso-en-el-ciclo-de-vida)
- [🧪 9. Beneficios, Buenas Prácticas y Errores](#-9-beneficios-buenas-prácticas-y-errores)

## 🚀 1. Qué es el Proceso Unificado

- 🏗️ **Definición:** metodología iterativa e incremental para desarrollo de software.
- 🧑‍🔬 **Origen:** Rational Software (Jacobson, Booch, Rumbaugh).
- 📐 **Lenguaje estándar:** `UML` para modelado.
- 🎯 **Eje central:** todo gira alrededor de **casos de uso**.

## 🔄 2. Fases del Proceso Unificado

| Fase | Objetivo principal | Resultado |
|---|---|---|
| **Inicio** | Definir alcance, objetivos y riesgos iniciales | Visión de proyecto |
| **Elaboración** | Entender dominio y base arquitectónica | Arquitectura validada |
| **Construcción** | Desarrollar iteración tras iteración | Incrementos funcionales |
| **Transición** | Pasar a producción y ajustar | Sistema operativo |

- 🔁 **Importante:** cada fase incluye iteraciones internas con entregas parciales.

## 📌 3. Principios Clave

| Principio | Aplicación práctica |
|---|---|
| **Iterativo e incremental** | Entregar valor en ciclos cortos |
| **Gestión continua de requisitos** | Refinar alcance de forma progresiva |
| **Arquitectura por componentes** | Separar responsabilidades |
| **Verificación temprana y continua** | Detectar fallas antes |
| **Control de cambios e integración frecuente** | Reducir riesgo de integración tardía |

## 🎯 4. Captura de Requisitos

- 📌 **Requisito:** necesidad o condición que el sistema debe cumplir.
- ⚠️ **Riesgo común:** mala captura = retrabajo, fallas y pérdida de valor.
- 👤 **Enfoque UP:** capturar desde perspectiva del usuario.

| Tipo de requisito | Qué describe | Ejemplo |
|---|---|---|
| **Funcional** | Funcionalidades del sistema | Registrar usuario |
| **No funcional** | Calidad del servicio | Rendimiento, seguridad, usabilidad |
| **Restricción** | Condiciones impuestas | Norma legal, tecnología obligatoria |

## 🧠 5. Casos de Uso

- 🎬 **Definición:** secuencia de interacción entre actor externo y sistema para lograr un objetivo.
- 👤 **Actor:** rol externo (persona, sistema o dispositivo).
- 🧭 **Perspectiva correcta:** hablar en lenguaje de negocio/usuario, no de implementación técnica.

| Ejemplos de actor | Tipo |
|---|---|
| 👤 Cliente | Persona |
| 🖥 Sistema de pagos | Sistema externo |
| 📱 App móvil externa | Dispositivo/plataforma |

| Sí es caso de uso | No es caso de uso |
|---|---|
| `Registrar usuario` | `Validar email` |
| `Realizar compra` | `Pantalla de login` |
| `Emitir factura` | `Método de base de datos` |

| Qué NO es un caso de uso | Motivo |
|---|---|
| Especificación técnica | Describe solución interna, no valor externo |
| Diagrama de clases | Modela estructura, no interacción de actor |
| Diseño de interfaz gráfica | No expresa objetivo funcional completo |
| Detalle interno de implementación | No está centrado en el actor |

| Nivel de detalle | Cuándo conviene |
|---|---|
| **Breve** | Exploración inicial |
| **Principal** | Definición estándar de alcance |
| **Extendido** | Reglas de negocio complejas |

## 🛠️ 6. Estructura de un Caso de Uso

| Campo | Contenido esperado |
|---|---|
| **Nombre** | Verbo + objeto (`Realizar compra`) |
| **Actor(es)** | Quién inicia la interacción |
| **Precondiciones** | Qué debe cumplirse antes |
| **Flujo principal** | Camino exitoso paso a paso |
| **Flujos alternativos** | Variantes válidas |
| **Flujos de excepción** | Errores o interrupciones |
| **Postcondiciones** | Estado esperado al final |

| Tipo de flujo | Definición |
|---|---|
| **Principal** | Secuencia normal hasta éxito |
| **Alternativo** | Camino distinto pero válido |
| **Excepción** | Condición que interrumpe el flujo |

| Mini flujo ejemplo: `Registrar usuario` | Pasos |
|---|---|
| **Principal** | 1) Ingresa al formulario 2) Completa datos 3) Presiona registrar 4) Sistema valida 5) Sistema crea cuenta |
| **Alternativos** | A1: usuario ya registrado · A2: email inválido |
| **Postcondición** | Usuario activo en el sistema |

| Ejemplo 2: `Realizar compra` | Resumen |
|---|---|
| **Actor principal** | Cliente |
| **Precondición** | Cliente autenticado con carrito cargado |
| **Flujo principal** | Revisa carrito -> confirma productos -> elige medio de pago -> ingresa datos -> sistema procesa |
| **Postcondición** | Compra registrada y pago confirmado |

## 🏛️ 7. Casos de Uso y Arquitectura

| Relación | Impacto en diseño |
|---|---|
| Casos de uso -> arquitectura | Guían decisiones arquitectónicas |
| Casos de uso -> responsabilidades | Ayudan a definir clases/servicios/componentes |
| Casos de uso -> entregables | Cada caso puede ser una unidad funcional entregable |

| Organización jerárquica | Uso |
|---|---|
| **Include** (inclusión/composición) | Reutilizar comportamiento común |
| **Generalización** (especialización/herencia) | Extender comportamientos sin duplicar |

## 🔁 8. Casos de Uso en el Ciclo de Vida

| Etapa del UP | Aporte de casos de uso |
|---|---|
| **Inicio** | Ayudan a delimitar alcance |
| **Elaboración** | Permiten estimar esfuerzo |
| **Construcción** | Guían diseño y desarrollo |
| **Transición** | Base para pruebas de aceptación |

| Área operativa | Uso de casos de uso |
|---|---|
| **Testing** | Escenarios de prueba funcional y trazabilidad completa |
| **BDD** | Facilitan automatización por comportamiento |
| **Gestión de cambios** | Evaluar impacto por caso afectado y reducir riesgo |

| Cómo identificar buenos casos de uso | Criterio |
|---|---|
| Identificar actores | Quién busca valor |
| Listar objetivos | Qué intenta lograr |
| Agrupar escenarios similares | Evitar duplicación |
| Confirmar con usuarios | Validar realidad de negocio |

| Criterios de calidad | Validación |
|---|---|
| Genera valor observable | Sí/No |
| Tiene inicio y fin claros | Sí/No |
| Representa interacción completa | Sí/No |
| No es épico ni trivial | Sí/No |

## 🧪 9. Beneficios, Buenas Prácticas y Errores

| Beneficio de trabajar con casos de uso | Impacto |
|---|---|
| **Mejor comprensión de requisitos** | Menos ambigüedad |
| **Mejor comunicación técnico-negocio** | Decisiones más alineadas |
| **Base para pruebas funcionales** | Mayor trazabilidad |
| **Priorización por iteraciones** | Entrega de valor temprana |

| Buenas prácticas ✅ | Errores frecuentes ❌ |
|---|---|
| Validar con usuarios finales | Nombrar casos como pantallas |
| Documentar alternativos y excepciones | Confundir tareas técnicas con funcionalidades |
| Usar lenguaje simple y centrado en valor | Redactar desde la lógica interna del sistema |
| Reutilizar patrones comunes | Dejar casos demasiado grandes o triviales |
