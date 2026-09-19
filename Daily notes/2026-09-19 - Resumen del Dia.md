---
date: 2026-09-19
aliases: [resumen-2026-09-19]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-09-19

> [!warning] Octava vez consecutiva que la rutina se dispara antes de medianoche Guatemala — sin resolver
> Al momento del pull (2026-09-19 05:50 UTC = **2026-09-18 23:50 hora de Guatemala, GMT-6**), el día calendario 2026-09-19 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-09-18** (a ~10 min de su cierre real, aún sujeta a la ventana de atribución de leads). Esta nota documenta esa lectura casi-final de 2026-09-18.
>
> Se confirmó vía `list_triggers` que el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") **sigue con el cron `50 5 * * *` (UTC) = 23:50 GT**, sin cambios desde que se documentó el problema por primera vez (7 ocurrencias previas documentadas en notas anteriores, esta es la octava). **Acción requerida del usuario:** editar el horario manualmente en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ, idealmente a las 00:30–01:00 GT.

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-09-18** (a ~10 min del cierre real, sujeta aún a cambios por ventana de atribución de leads):

| Campaña | Status | Gasto | Leads | CPL | CTR | Emoji |
|---------|--------|-------|-------|-----|-----|-------|
| Toma El control de tu pyme (GT) | ACTIVE | $14.65 | 2 | **$7.33** 🔴 | 1.28% 🔴 | 🟡 |
| Pyme El salvador (SV) | ACTIVE | $10.29 | 2 | **$5.15** 🟢 | 1.91% | 🟢 |
| Beco | ACTIVE | $8.58 | 1 | $8.58 🔴 | 1.21% 🔴 | 🟡 |
| Odoo Test | ACTIVE | $6.12 | 3 | **$2.04** 🟢 | 1.93% | 🟢 |
| Toma El control de tu pyme (USA) | PAUSED | $0.00 | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - PY | PAUSED | $0.00 | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED | $0.00 | - | - | - | ⏸️ |

**Desglose de "Toma El control de tu pyme" (GT) — A/B test de copys:**

| Ad Set | Status | Presupuesto/día | Gasto hoy | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-----------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $14.65 (dentro del presupuesto) | 30 | 1.28% | 2 | **$7.33** |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | 0 | - | - | - |

**Cambios en la cuenta durante la ventana 2026-09-18 (según activity log):** ninguno manual. Solo eventos automáticos de Meta: creación de 4 audiencias personalizadas (`asa_auto_custom_audience`, generadas automáticamente por Meta a las 4:10 AM, no por el equipo). No hubo ajustes de presupuesto, pausas ni cambios de nombre hechos por Gabriel Calderon hoy — el día transcurrió con la configuración vigente desde la decisión del A/B test (Urgencia activo, Excel pausado).

---

## 🔍 Análisis e Insights

- **"Toma El control de tu pyme" (GT) revierte su racha de mejora:** tras dos cierres confirmados consecutivos por debajo de la meta ($2.92 el 09-16, $2.98 el 09-17), la lectura casi-final de hoy muestra **$7.33 CPL** — de vuelta al rango problemático original documentado en [[CLAUDE.md]] ($9.29). El CTR también cae fuerte, de ~2.22-2.24% a **1.28%**. Con solo 30 clicks y 2 leads, la muestra es pequeña y podría tratarse de variación normal del día, pero merece confirmarse con el reporte de cierre formal antes de sacar conclusiones sobre el ad set "Urgencia".
- **Odoo Test y Beco muestran leads por primera vez en varios días:** ambas campañas habían reportado `results: Not available` en los cierres confirmados de 09-15 y 09-17 (problema de tracking documentado en el reporte del 09-17). Hoy Odoo Test registra 3 leads a **$2.04 CPL** (el mejor de la cuenta) y Beco registra 1 lead a $8.58 CPL. Posible señal de que el problema de atribución se resolvió, aunque conviene confirmar que no sea solo timing favorable de esta lectura parcial.
- **Pyme El Salvador continúa su tendencia de mejora sostenida:** $10.83 → $7.18 → **$5.15 CPL**, ya por debajo de la meta de cuenta ($6-7) por primera vez. Tercera mejora consecutiva documentada.
- **El ad set "Urgencia" gastó $14.65 dentro de su presupuesto de $15.00/día** — primera vez en varios días que no sobregasta (venía sobregastando 17-19% en los cierres anteriores), posiblemente relacionado con el CTR/clicks más bajos de hoy.
- Ninguna investigación de competencia o tendencias externas se realizó en esta sesión — el foco estuvo en revisar el estado de las 4 campañas activas y confirmar (sin resolver) el problema de horario del trigger.

---

## ✏️ Cambios Realizados

- **Ninguno realizado por esta sesión ni por el equipo hoy.** El activity log de la cuenta no registra ajustes manuales de presupuesto, pausas, ni cambios de nombre en la ventana 2026-09-18. Los únicos eventos fueron automáticos de Meta (creación de 4 audiencias personalizadas `asa_auto_custom_audience`).
- La configuración vigente durante todo el día fue la decidida en el A/B test previo: Urgencia activo con $15/día, Excel pausado.

---

## 🔬 Investigación Realizada

- Se confirmó el estado del trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` vía `list_triggers`: cron sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde el diagnóstico original. Octava ocurrencia consecutiva del disparo prematuro documentada.
- Se revisaron los 4 campañas activas y el desglose de ad sets de "Toma El control de tu pyme" (GT) para dar seguimiento al A/B test.
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## 📊 Datos Clave del Día

| Métrica | 2026-09-18 (parcial ~cierre) | 2026-09-17 (cierre confirmado) | Variación |
|---------|-------------------------------|----------------------------------|-----------|
| Gasto Total (4 campañas activas) | $39.64 | $44.22 | 🟢 -10.4% |
| Leads Total (confirmados) | 8 | 8 | Sin cambio (potencialmente mayor al cerrar) |
| CPL Promedio (ponderado) | $4.96 | $5.53 | 🟢 -10.3% |
| CTR Promedio (ponderado) | ~1.52% | 1.76% | 🔴 -13.6% |
| Mejor CPL del día | Odoo Test: **$2.04** | Toma El control GT: $2.98 | Cambio de líder |
| Peor CPL del día (con datos) | Beco: $8.58 | Pyme El salvador: $7.18 | 🔴 Empeora |

> [!caution] No confirmar como cierre real
> Estas cifras corresponden a una lectura tomada ~10 minutos antes del cierre real de 2026-09-18 y pueden moverse al resolverse la ventana de atribución de leads. Confirmar con el Reporte Performance formal cuando esté disponible (~7 AM GT).

---

## ✅ Próximas Acciones

- [ ] **Editar manualmente el horario del trigger** `trig_01DMJfrsQXaTY5KJntXisDPQ` en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ — mover de 23:50 GT a ~00:30-01:00 GT (octava ocurrencia del problema, sigue sin resolverse)
- [ ] Confirmar el cierre oficial de 2026-09-18 con el Reporte Performance formal, especialmente el CPL de $7.33 de "Toma El control" (¿reversión real o variación de muestra pequeña?)
- [ ] Verificar si Odoo Test y Beco mostrando leads hoy confirma que el problema de tracking de 09-15/09-17 se resolvió, o si vuelve a aparecer `results: Not available` en el cierre
- [ ] Investigar por qué el CTR de "Toma El control" (Urgencia) cayó de ~2.2% a 1.28% hoy
- [ ] Seguir dando seguimiento a "Pyme El Salvador": primera vez dentro de la meta de CPL ($5.15), confirmar que se sostiene

---

## 🔗 Enlaces

- [[Daily notes/2026-09-18 - Resumen del Dia]] - Resumen del día anterior (misma alerta de timing, séptima ocurrencia)
- [[Reports/2026-09-17 - Reporte Performance]] - Último reporte formal disponible (Reporte de 09-18 aún pendiente, se genera ~7 AM GT)
- [[CLAUDE.md]] - Tarea de A/B testing de copys; posible reversión de tendencia a confirmar

#daily-note #summary #meta-ads #octopus
