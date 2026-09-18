---
date: 2026-09-18
aliases: [resumen-2026-09-18]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-09-18

> [!warning] Séptima vez consecutiva que la rutina se dispara antes de medianoche Guatemala — sin resolver
> Al momento del pull (2026-09-18 05:50 UTC = **2026-09-17 23:50 hora de Guatemala, GMT-6**), el día calendario 2026-09-18 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-09-17** (a ~10 min de su cierre real, aún sujeta a la ventana de atribución de leads). Esta nota documenta esa lectura casi-final de 2026-09-17.
>
> Se confirmó vía `list_triggers` que el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") **sigue con el cron `50 5 * * *` (UTC) = 23:50 GT**, sin cambios desde que se documentó el problema por primera vez. Como se reportó ayer, esta sesión no tiene permiso para modificarlo vía API (*"this routine was created via http_api, not by an agent"*). **Acción requerida del usuario:** editar el horario manualmente en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ, idealmente a las 00:30–01:00 GT.

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-09-17** (a ~10 min del cierre real, sujeta aún a cambios por ventana de atribución de leads):

| Campaña | Status | Gasto | Leads | CPL | CTR | Emoji |
|---------|--------|-------|-------|-----|-----|-------|
| Toma El control de tu pyme (GT) | ACTIVE | $17.54 | 6 | **$2.92** 🟢 | **2.22%** | 🟢 |
| Pyme El salvador (SV) | ACTIVE | $14.17 | 2 | $7.09 🔴 | 1.86% | 🟡 |
| Beco | ACTIVE | $9.32 | Pendiente atribución | N/D | 0.80% 🔴 | 🟡 |
| Odoo Test | ACTIVE | $2.50 | Pendiente atribución | N/D | 0.87% | 🟡 |
| Toma El control de tu pyme (USA) | PAUSED | $0.00 | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - PY | PAUSED | $0.00 | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED | $0.00 | - | - | - | ⏸️ |

**Desglose de "Toma El control de tu pyme" (GT) — A/B test de copys:**

| Ad Set | Status | Presupuesto/día | Gasto hoy | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-----------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $17.54 (sobre-gasto leve) | 62 | 2.22% | 6 | **$2.92** |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | 0 | - | - | - |

**Cambios en la cuenta durante la ventana 2026-09-17 (según activity log):** ninguno manual. Solo eventos automáticos de Meta: inicio de entrega ("Ad delivered") en los 4 ad sets activos y creación automática de una audiencia personalizada (`asa_auto_custom_audience`, generada por Meta, no por el equipo). No hubo ajustes de presupuesto, pausas ni cambios de nombre hechos por Gabriel Calderon hoy — el día transcurrió con la configuración que quedó tras la decisión del A/B test de ayer (Urgencia activo con presupuesto duplicado, Excel pausado).

---

## 🔍 Análisis e Insights

- **La decisión del A/B test de ayer se ve validada:** con Urgencia activo todo el día y Excel pausado, "Toma El control de tu pyme" (GT) cierra la lectura casi-final en **$2.92 CPL** — el mejor resultado registrado hasta ahora, superando incluso el $3.53 casi-final del 09-16. 6 leads confirmados con solo $17.54 de gasto.
- **El ad set "Urgencia" gastó $17.54 contra un presupuesto diario de $15.00** (~17% sobre el límite configurado) — vale la pena revisar si esto es normal dentro de la tolerancia de entrega de Meta o si el presupuesto debería ajustarse al alza formalmente dado el excelente CPL.
- **Apareció un tercer ad set no documentado antes:** "TestA/B Productividad" ($5.00/día, pausado, sin gasto). No estaba mencionado en notas anteriores del vault — parece ser una variante de copy adicional creada en algún momento pero nunca activada. Requiere aclarar su origen y si se debe sumar al testing.
- **Beco y Odoo Test aún no muestran leads** en esta lectura parcial — es normal a ~10 minutos del cierre real por la ventana de atribución (mismo patrón visto en cierres anteriores), pero ambas muestran CTR bajo (0.80% y 0.87% respectivamente), por debajo de la meta de cuenta (3-4%).
- **Pyme El Salvador sigue siendo la campaña más cara de la cuenta** ($7.09 CPL, único sobre la meta de $6-7), aunque mejora frente al $10.79-$10.83 de días anteriores — posible señal de que ajustes previos de targeting/copy están ayudando, pero todavía no llega a la meta.
- Ninguna investigación de competencia o tendencias externas se realizó en esta sesión — el foco estuvo en revisar el resultado del A/B test recién decidido y confirmar el estado (sin resolver) del problema de horario del trigger.

---

## ✏️ Cambios Realizados

- **Ninguno realizado por esta sesión ni por el equipo hoy.** El activity log de la cuenta no registra ajustes manuales de presupuesto, pausas, ni cambios de nombre en la ventana 2026-09-17. Los únicos eventos fueron automáticos de Meta (inicio de entrega de anuncios, creación de audiencia personalizada automática).
- La configuración vigente durante todo el día fue la decidida ayer (09-16): Urgencia activo con $15/día, Excel pausado.

---

## 🔬 Investigación Realizada

- Se confirmó el estado del trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` vía `list_triggers`: cron sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde el diagnóstico de ayer. Séptima ocurrencia consecutiva del disparo prematuro documentada.
- Se revisaron los ad sets dentro de "Toma El control de tu pyme" (GT) para dar seguimiento al A/B test iniciado ayer — se descubrió el ad set no documentado "TestA/B Productividad".
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## 📊 Datos Clave del Día

| Métrica | 2026-09-17 (parcial ~cierre) | 2026-09-16 (cierre confirmado) | Variación |
|---------|-------------------------------|----------------------------------|-----------|
| Gasto Total (4 campañas activas) | $43.53 | $39.45 | 🔺 +10.3% |
| Leads Total (confirmados) | 8 (2 campañas aún pendientes de atribución) | 8 | Potencialmente mayor al cerrar |
| CTR Promedio (ponderado) | ~1.75% | 1.36% | 🟢 +28.7% |
| Mejor CPL del día | Toma El control GT: **$2.92** | Toma El control GT: $3.56 | 🟢 -18.0% |
| Peor CPL del día (con datos) | Pyme El salvador: $7.09 | Pyme El salvador: $10.83 | 🟢 -34.5% |

> [!caution] No confirmar como cierre real
> Estas cifras corresponden a una lectura tomada ~10 minutos antes del cierre real de 2026-09-17 y pueden moverse al resolverse la ventana de atribución de leads (especialmente Beco y Odoo Test, aún sin leads confirmados). Confirmar con el Reporte Performance formal cuando esté disponible (~7 AM GT).

---

## ✅ Próximas Acciones

- [ ] **Editar manualmente el horario del trigger** `trig_01DMJfrsQXaTY5KJntXisDPQ` en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ — mover de 23:50 GT a ~00:30-01:00 GT (séptima ocurrencia del problema, sigue sin resolverse)
- [ ] Confirmar el cierre oficial de 2026-09-17 con el Reporte Performance formal y verificar si el CPL de $2.92 en "Toma El control" se sostiene tras la atribución completa
- [ ] Aclarar el origen del ad set "TestA/B Productividad" (pausado, $5.00/día, no documentado antes) y decidir si se integra al testing o se elimina
- [ ] Revisar si el gasto de "Urgencia" ($17.54 vs $15.00 de presupuesto) requiere ajuste formal del presupuesto diario
- [ ] Investigar por qué "Beco" y "Odoo Test" muestran CTR bajo (0.80% y 0.87%) y aún sin leads confirmados
- [ ] Seguir dando seguimiento a "Pyme El Salvador": mejora vs días previos pero sigue sobre la meta de CPL

---

## 🔗 Enlaces

- [[Daily notes/2026-09-17 - Resumen del Dia]] - Resumen del día anterior (misma alerta de timing, sexta ocurrencia)
- [[Reports/2026-09-16 - Reporte Performance]] - Último reporte formal disponible (Reporte de 09-17 aún pendiente, se genera ~7 AM GT)
- [[CLAUDE.md]] - Tarea de A/B testing de copys, en progreso con resultados preliminares muy positivos

#daily-note #summary #meta-ads #octopus
