# Trabajo-Sostenibilidad
# Plan de Sostenibilidad para una Empresa de Desarrollo de Software (DAM)

## Datos del Módulo
* **Ciclo Formativo:** Desarrollo de Aplicaciones Multiplataforma (DAM)
* **Curso:** DAM2
* **Módulo:** Sostenibilidad
* **Título del Tema:** Tema 5. Plan para una empresa DAM

---

## Introducción del Tema

El crecimiento acelerado de los servicios digitales y la industria del software exige que la sostenibilidad deje de ser una consideración teórica y se integre directamente en las competencias técnicas del desarrollo de aplicaciones. Este tema aborda el diseño, la ejecución y el seguimiento de un **Plan de Sostenibilidad** adaptado al contexto de una empresa o departamento de desarrollo multiplataforma.

A lo largo del tema se establece un marco práctico con un **horizonte inicial de seis semanas**, donde se fijan metas de trabajo enfocadas en la eficiencia de recursos, la accesibilidad digital, la optimización de infraestructura en la nube y la gobernanza de datos. Como eje de aplicación real, se integra el proyecto intermodular **ReparaDAM**, una solución concebida para la gestión del inventario, mantenimiento y reutilización de equipos informáticos, uniendo la reducción del impacto ambiental del software con la extensión de la vida útil del hardware.

---

## Estructura y Contenidos Clave

### 1. Diagnóstico e Inventario Inicial
Antes de ejecutar cualquier acción técnica, el plan requiere un análisis previo del entorno:
* Inventariado de aplicaciones, entornos de despliegue, datos y hardware.
* Consulta y alineación con la plantilla y los usuarios finales.
* Selección de asuntos **ASG** (Ambiental, Social y Gobernanza) priorizando según impacto, riesgo, esfuerzo y calidad de las evidencias disponibles.

---

### 2. Plan de Acción (Horizonte de 6 semanas)

> *Nota: Las metas fijadas son objetivos de trabajo y no resultados garantizados.*

| Prioridad y Acción | Responsable y Plazo | Indicador / Evidencia |
| :--- | :--- | :--- |
| **Optimización de operaciones frecuentes**<br>Meta provisional: -15 % Wh por lote si existe medición fiable. | Desarrollo + Calidad<br>*(Semanas 1–4)* | Consumo energético (Wh/lote) y datos originales.<br>Límites: mantener latencia y evitar tasa de errores. |
| **Revisión de entornos ociosos**<br>Ajuste de horarios y dimensionamiento en servidores/nube. | Operaciones<br>*(Semanas 2–3)* | Horas reservadas evitables.<br>Verificación de disponibilidad y protocolos de recuperación. |
| **Accesibilidad en flujos críticos**<br>Corregir barreras en tres casos de uso clave. | Interfaces + Calidad<br>*(Semanas 2–5)* | Pruebas completadas con ayudas técnicas.<br>Resolución de incidencias de accesibilidad. |
| **Gobernanza y privacidad de datos**<br>Justificación de campos, accesos y política de conservación. | Producto + Responsable de Datos<br>*(Semanas 1–5)* | Inventario de campos y finalidades.<br>Revisión de matriz de permisos y plazos de retención. |
| **Mantenibilidad y soporte técnico**<br>Documentar dependencias, licencias y ciclo de vida (SBOM). | Equipo Técnico<br>*(Semanas 3–6)* | Inventario técnico actualizado.<br>Decisiones de compatibilidad y soporte de componentes. |
| **Transparencia y reporte**<br>Publicación de resultados (incluyendo resultados desfavorables). | Coordinación<br>*(Semana 6)* | Informe final con metodología, datos de referencia, cambios y límites de la medición. |

---

### 3. Principios Técnicos Aplicados

* **Infraestructura y Nube:** Aplicación de las directrices del pilar de sostenibilidad en la nube (como las recomendaciones de AWS), evaluando la desconexión de servicios ociosos, el redimensionamiento de instancias y la adaptación a patrones reales de consumo.
* **Programación Sensible al Carbono (*Carbon-Aware*):** Desplazamiento de cargas de trabajo flexibles (procesamientos por lotes, informes no urgentes) a periodos o regiones con menor intensidad de carbono, respetando siempre los requisitos de privacidad, latencia y costes de transferencia.
* **Evaluación Iterativa:** Separación analítica entre costes financieros, asignación de recursos, consumo energético y emisiones estimadas, evitando asumir que la reducción de uno implica automáticamente la de los demás.

---

### 4. Proyecto de Aplicación: ReparaDAM

**ReparaDAM** es la propuesta práctica del módulo para gestionar el préstamo, la reparación y el seguimiento de equipos informáticos.

* **Producto Mínimo Viable (MVP):** Control de inventario, apertura y seguimiento de incidencias de mantenimiento, registro de préstamos y generación de informes de estado.
* **Arquitectura Base:**
  * **Escritorio:** Gestión de inventario, filtros y generación de reportes.
  * **Móvil (opcional):** Alta rápida de incidencias y consulta básica.
  * **Backend & Persistencia:** Lógica de negocio, control de roles/permisos y modelo relacional (SQL).
* **Preguntas de Investigación:**
  1. *Sobre la aplicación:* ¿Una optimización en las consultas e intervalos de sincronización reduce el consumo energético manteniendo el nivel de servicio?
  2. *Sobre el proceso:* ¿El control del ciclo de vida de los equipos contribuye a incrementar el número de reparaciones y alargar la vida útil del hardware del centro?

---

## Criterios de Aceptación del Plan
* Los flujos del software funcionan sin pérdida de integridad ni fallos de permisos.
* Se cuenta con un método de prueba reproducible y datos de medición originales o datasets sintéticos documentados.
* El informe final distingue claramente entre métricas directamente observadas y estimaciones indirectas.
