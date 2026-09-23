---
date: 2026-09-23
aliases: [resumen-2026-09-23]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-09-23

> [!warning] Duodécima vez consecutiva que la rutina se dispara antes de medianoche Guatemala — sin resolver
> Al momento del pull (2026-09-23 05:50 UTC = **2026-09-22 23:50 hora de Guatemala, GMT-6**), el día calendario 2026-09-23 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-09-22** (a ~10 min de su cierre real, aún sujeta a la ventana de atribución de leads). Esta nota documenta esa lectura casi-final de 2026-09-22.
>
> Se confirmó vía `list_triggers` que el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") **sigue con el cron `50 5 * * *` (UTC) = 23:50 GT**, sin cambios desde su creación (2026-08-28) y sin cambios desde que se documentó el problema por primera vez (11 ocurrencias previas documentadas en notas anteriores, esta es la duodécima). `next_run_at` confirma que disparará mañana a la misma hora. **Acción requerida del usuario:** editar el horario manualmente en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ, idealmente a las 00:30–01:00 GT.

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-09-22** (a ~10 minutos del cierre real, sujeta aún a cambios por ventana de atribución de leads):

| Campaña | Status | Gasto | Leads | CPL | CTR | Emoji |
|---------|--------|-------|-------|-----|-----|-------|
| Odoo Test (GT) | ACTIVE | $4.39 | 2 | **$2.20** 🟢 | 1.71% 🟡 | 🟢 |
| Toma El control de tu pyme (GT) | ACTIVE | $11.88 | 4 | $2.97 🟢 | 2.04% 🟡 | 🟢 |
| Pyme Colombia (COL) | ACTIVE | $9.87 | 1 | $9.87 🔴 | 1.88% 🟡 | 🟡 |
| Beco (GT) | ACTIVE | $9.71 | 1 | $9.71 🔴 | 0.88% 🔴 | 🔴 |
| Pyme El Salvador (SV) | ACTIVE | $10.70 | 0 ⚠️ | N/D | 0.81% 🔴 | ⚠️ |
| Toma El control de tu pyme (USA) | PAUSED | $0.00 | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - PY | PAUSED | $0.00 | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED | $0.00 | - | - | - | ⏸️ |

**Ninguna acción manual ni automatizada fue realizada sobre las campañas hoy** — se revisaron sus métricas y el activity log de la cuenta, pero no se hicieron cambios de presupuesto, targeting, copy ni estado.

### ⚠️ Pyme El Salvador sin leads confirmados por primera vez en varios cierres

Después de ser la campaña más eficiente de la cuenta en los últimos cierres consecutivos (CPL $6.10–$6.13, dentro de meta), hoy registra **0 leads confirmados** pese a gastar $10.70 y generar 17 clicks. Puede deberse a la ventana de atribución (leads de las últimas horas del día aún sin resolver al momento del pull) o a un problema de conversión puntual. Requiere confirmación con el Reporte Performance formal de mañana (~7 AM GT) antes de tratarlo como una caída real.

### 🆕 Pyme Colombia supera su presupuesto diario configurado

La campaña, lanzada ayer (09-21) con presupuesto corregido a **$7.50/día**, gastó **$9.87** hoy — **31.6% por encima** de su presupuesto diario. Esto es consistente con el patrón de sobregasto ya documentado previamente en el ad set "Urgencia" de GT; vale la pena revisar el `daily_budget` efectivo vs. el pacing real de esta campaña en su segundo día completo de vida.

---

## 🔬 Investigación Realizada

- Se revisaron las 5 campañas activas de la cuenta a nivel cuenta/campaña con `date_preset=today` (equivalente a 2026-09-22 en horario de cuenta).
- Se revisó el activity log de la cuenta (2026-09-22 00:00–23:51 GT): solo se registraron eventos de tipo "Ad delivered" (entrega automática de Meta), ningún cambio manual de presupuesto, targeting, copy o estado.
- **Segundo caso del mismo patrón de `campaign_id` no resoluble:** el activity log registra 13 eventos de entrega ("Ad delivered") durante todo el día para un anuncio llamado `AD Pyme Urgencia COL_Group_1`, referenciando el `campaign_id` `120256952282790211` — que, igual que el caso de `AD Pyme Urgencia SV_Group_1` documentado ayer, **no resuelve a ninguna campaña consultable en esta cuenta**. Ya son dos mercados distintos (SV y COL) con el mismo síntoma: un anuncio con nombre "Urgencia" cuyo `campaign_id` de activity log no coincide con ningún id de campaña visible vía API. Patrón real, no aislado — queda pendiente de investigar con más profundidad (posible discrepancia entre IDs de campaign vs ad set en el log, o estructura duplicada/histórica no visible a nivel API).
- Se confirmó el estado del trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` vía `list_triggers`: cron sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde su creación el 2026-08-28. Duodécima ocurrencia consecutiva del disparo prematuro documentada.
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## ✏️ Cambios Realizados

- **Ninguno.** No se detectaron cambios manuales en el activity log de la cuenta durante la ventana del día (2026-09-22, horario GT), y esta sesión tampoco realizó modificaciones a campañas, presupuestos, targeting o creativos.

---

## 📊 Análisis e Insights

- **Las 4 campañas establecidas mejoran fuerte vs. el cierre confirmado de ayer:** CPL promedio ponderado baja de $8.49 a **$5.24** (-38.3%), leads confirmados suben de 5 a 7 (+40%), con menor gasto (-13.6%). Es la mejor combinación de eficiencia y volumen de las últimas notas — aunque el resultado de El Salvador en $0 leads amerita confirmación antes de celebrar la mejora completa.
- **Odoo Test (GT) toma el liderazgo de eficiencia de la cuenta:** $2.20 CPL con 2 leads, su mejor cierre reciente y muy por debajo de la meta de $6-7.
- **Toma El control de tu pyme (GT) revierte su peor racha:** de $15.69 (peor CPL de la cuenta ayer) a $2.97 hoy con 4 leads — la mejora más marcada de la cuenta, aunque esta campaña ha mostrado alta volatilidad día a día en notas anteriores.
- **Beco repite un solo lead a CPL alto ($9.71)**, consistente con su patrón intermitente de las últimas semanas — el problema de atribución reportado antes sigue sin resolverse de forma sostenida.
- **Pyme Colombia, en su segundo día, gasta 31.6% por encima de su presupuesto diario** — ver detalle en Campañas Revisadas.
- Incluyendo Colombia, el CPL blendeado de las 5 campañas activas es **$5.82**, dentro del rango objetivo de $6-7 (ligeramente por debajo).
- Ninguna investigación de competencia o tendencias externas se realizó en esta sesión — el foco estuvo en revisar las 5 campañas activas, el activity log del día y dar seguimiento al patrón de `campaign_id` no resoluble.

---

## 📊 Datos Clave del Día

| Métrica (4 campañas establecidas: GT×3 + SV) | 2026-09-22 (casi-cierre) | 2026-09-21 (cierre confirmado) | Variación |
|---------|---------------------------|----------------------------------|-----------|
| Gasto Total | $36.68 | $42.43 | 🟢 -13.6% |
| Leads Confirmados | 7 | 5 | 🟢 +40.0% |
| CPL Promedio (ponderado) | **$5.24** | $8.49 | 🟢 -38.3% |
| CTR Promedio (ponderado) | 1.33% | 1.49% | 🔻 -10.9% |
| CPC Promedio | $0.42 | $0.39 | 🔻 +6.9% |
| CPM Promedio | $5.53 | $5.75 | 🟢 -3.8% |
| Impresiones | 6,633 | 7,385 | 🔻 -10.2% |
| Clicks | 88 | 110 | 🔻 -20.0% |
| Alcance (Reach) | 5,181 | 5,844 | 🔻 -11.3% |
| Mejor CPL del día | Odoo Test: **$2.20** | Odoo Test: $4.00 | Mismo líder, CPL mejora |
| Peor CPL del día | Pyme El Salvador: 0 leads ⚠️ (Beco: $9.71 confirmado) | Toma El control GT: $15.69 | Cambio de peor performer |

**Pyme Colombia (2do día, sin comparación previa completa):** $9.87 gastados sobre $7.50/día de presupuesto configurado (+31.6%), 1 lead, CPL $9.87.

**Cuenta completa (5 campañas activas, incluyendo Colombia):** Gasto $46.55 | Leads 8 | CPL blendeado $5.82 | CTR 1.39% | CPC $0.45 | CPM $6.26 | Impresiones 7,433 | Clicks 103 | Reach 5,742.

> [!caution] No confirmar como cierre real
> Estas cifras corresponden a una lectura tomada ~10 minutos antes del cierre real de 2026-09-22 y pueden moverse al resolverse la ventana de atribución de leads — en particular el resultado de Pyme El Salvador. Confirmar con el Reporte Performance formal cuando esté disponible (~7 AM GT).

---

## 📋 Próximas Acciones

- [ ] Confirmar mañana (~7 AM GT) el cierre real de 2026-09-22 vía Reporte Performance, en especial el resultado de Pyme El Salvador (0 leads en esta lectura casi-final)
- [ ] Revisar el `daily_budget` efectivo de Pyme Colombia — gastó $9.87 sobre $7.50/día configurado (+31.6%) en su segundo día
- [ ] Dar seguimiento al patrón de `campaign_id` no resoluble para anuncios "Urgencia" — ya son 2 casos (SV el 09-21, COL el 09-22)
- [ ] **Usuario:** corregir el horario del trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` (actualmente dispara a las 23:50 GT en vez de después de medianoche) — 12ª ocurrencia consecutiva sin resolver
- [ ] Retomar el A/B testing pendiente de los 5 nuevos copys en "Toma El control de tu pyme" (GT), documentado en el proyecto pero aún sin iniciar en esta cuenta

---

## 🔗 Enlaces

- [[Reports/2026-09-21 - Reporte Performance]] — último reporte de cierre confirmado disponible (el de 2026-09-22 se genera mañana ~7 AM GT)
- [[Daily notes/2026-09-22 - Resumen del Dia]] — resumen del día anterior
- Tags: #daily-note #summary #meta-ads #octopus
