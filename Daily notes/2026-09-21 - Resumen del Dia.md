---
date: 2026-09-21
aliases: [resumen-2026-09-21]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-09-21

> [!warning] Décima vez consecutiva que la rutina se dispara antes de medianoche Guatemala — sin resolver
> Al momento del pull (2026-09-21 05:50 UTC = **2026-09-20 23:50 hora de Guatemala, GMT-6**), el día calendario 2026-09-21 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-09-20** (a ~10 min de su cierre real, aún sujeta a la ventana de atribución de leads). Esta nota documenta esa lectura casi-final de 2026-09-20.
>
> Se confirmó vía `list_triggers` que el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") **sigue con el cron `50 5 * * *` (UTC) = 23:50 GT**, sin cambios desde su creación (2026-08-28) y sin cambios desde que se documentó el problema por primera vez (9 ocurrencias previas documentadas en notas anteriores, esta es la décima). **Acción requerida del usuario:** editar el horario manualmente en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ, idealmente a las 00:30–01:00 GT.

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-09-20** (a ~10 minutos del cierre real, sujeta aún a cambios por ventana de atribución de leads):

| Campaña | Status | Gasto | Leads | CPL | CTR | Emoji |
|---------|--------|-------|-------|-----|-----|-------|
| Toma El control de tu pyme (GT) | ACTIVE | $20.22 | 4 | $5.06 🟢 | 1.67% 🔴 | 🟢 |
| Pyme El salvador (SV) | ACTIVE | $15.63 | 4 | **$3.91** 🟢 | 1.93% 🟡 | 🟢 |
| Odoo Test | ACTIVE | $6.24 | 1 | $6.24 🟡 | 1.24% 🔴 | 🟢 |
| Beco | ACTIVE | $9.91 | 1 | $9.91 🔴 | 1.49% 🔴 | 🟡 |
| Toma El control de tu pyme (USA) | PAUSED | $0.00 | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - PY | PAUSED | $0.00 | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED | $0.00 | - | - | - | ⏸️ |

**Desglose de "Toma El control de tu pyme" (GT) — A/B test de copys:**

| Ad Set | Status | Presupuesto/día | Gasto hoy | Clicks | CTR | CPL |
|--------|--------|------------------|-----------|--------|-----|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | **$20.22 (⚠️ 134.8% del presupuesto)** | 58 | 1.67% | $5.06 |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | 0 | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | 0 | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | 0 | - | - |

**Cambios en la cuenta durante la ventana 2026-09-20 (según activity log):** ninguno — el activity log de la cuenta (`ads_account_get_activity_logs`, 2026-09-20T00:00 a 2026-09-21T00:00 GT) regresó **vacío**, sin eventos manuales del equipo ni automáticos de Meta (ni siquiera el cargo de facturación que apareció ayer). La configuración vigente sigue siendo la decidida en el A/B test (Urgencia activo con $15/día, Excel/Productividad/GT+QTZ pausados).

---

## 🔍 Análisis e Insights

- **El ad set "Urgencia" rompe su patrón de gasto y sobregasta fuerte hoy:** $20.22 gastados contra un presupuesto de $15.00/día (134.8%, +$5.22 sobre el límite). Los dos cierres confirmados anteriores (09-19 y 09-20 parcial de ayer) mostraron gasto *por debajo* del presupuesto; este es el primer sobregasto documentado desde antes del 09-18. Vale la pena confirmar si es un ajuste temporal de Meta por el pacing del A/B test o si amerita revisión manual del presupuesto.
- **"Toma El control de tu pyme" (GT) continúa su patrón de alta volatilidad:** $2.92 (09-16) → $2.98 (09-17) → $7.41 (09-18) → $2.43 (09-19, confirmado) → **$5.06** (09-20, casi-final). El CPL de hoy cae en el punto medio del rango oscilante de las últimas dos semanas — ni el mejor ni el peor cierre reciente. Con el sobregasto de hoy, el volumen de clicks (58) es similar al de 09-19 (57), así que el aumento de CPL no viene de más tráfico sino de una conversión click→lead más débil.
- **Beco vuelve a reportar datos, rompiendo (por ahora) el patrón intermitente de `results: Not available`:** a diferencia de 09-15, 09-17 y 09-19 (N/D), hoy sí hay 1 lead confirmado con CPL de $9.91 — el peor CPL de la cuenta y el único por encima de la meta de $6-7. No está claro todavía si el problema de atribución se resolvió o si esta lectura cambiará al confirmarse el cierre real (falta ~10 min); seguir de cerca en el reporte formal de mañana.
- **Pyme El Salvador se mantiene como la campaña más eficiente de la cuenta:** $3.91 CPL, muy por debajo de la meta de $6-7, continuando la racha de mejora sostenida documentada en días anteriores.
- **El gasto total de cuenta sube fuerte vs. el último cierre confirmado (09-19):** $52.00 hoy vs. $34.87 el 09-19 (+49.1%), impulsado principalmente por el sobregasto de "Urgencia" y, en menor medida, por Pyme El Salvador ($15.63 vs $8.95 el 09-19, +74.6%). Los leads también suben (10 vs 9) pero no proporcionalmente al gasto, lo que empuja el CPL promedio de cuenta al alza (+34.4%).
- **El activity log vacío contrasta con los últimos dos cierres**, que sí registraron al menos el cargo de facturación automático de Meta. No es necesariamente una anomalía (el cargo puede aparecer más tarde en el día), pero confirma que ningún cambio manual de presupuesto, pausa o nomenclatura se hizo hoy.
- Ninguna investigación de competencia o tendencias externas se realizó en esta sesión — el foco estuvo en revisar el estado de las 4 campañas activas, el desglose del A/B test (incluyendo el sobregasto detectado), y confirmar (sin resolver) el problema de horario del trigger.

---

## ✏️ Cambios Realizados

- **Ninguno realizado por esta sesión ni por el equipo hoy.** El activity log de la cuenta (ventana 2026-09-20 completa, hora Guatemala) regresó vacío — sin ajustes manuales de presupuesto, pausas, cambios de nombre, ni eventos automáticos de Meta.
- La configuración vigente durante todo el día fue la decidida en el A/B test previo: Urgencia activo con $15/día (hoy sobregastado a $20.22), Excel/Productividad/GT+QTZ pausados.

---

## 🔬 Investigación Realizada

- Se confirmó el estado del trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` vía `list_triggers`: cron sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde su creación el 2026-08-28. Décima ocurrencia consecutiva del disparo prematuro documentada; `next_run_at` confirma que seguirá disparando a la misma hora mañana.
- Se revisaron las 4 campañas activas (Toma El control GT, Odoo Test, Beco, Pyme El Salvador) a nivel cuenta y el desglose de ad sets del A/B test de "Toma El control de tu pyme" (GT) a nivel ad set.
- Se revisó el activity log de la cuenta (2026-09-20 00:00 a 2026-09-21 00:00, hora Guatemala) — regresó vacío, sin eventos.
- Se detectó y documentó el sobregasto del ad set "Urgencia" (134.8% de su presupuesto diario), un patrón nuevo no visto en los cierres confirmados recientes.
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## 📊 Datos Clave del Día

| Métrica | 2026-09-20 (casi-cierre) | 2026-09-19 (cierre confirmado) | Variación |
|---------|---------------------------|----------------------------------|-----------|
| Gasto Total (4 campañas activas) | $52.00 | $34.87 | 🔻 +49.1% |
| Leads Confirmados | 10 | 9 | 🟢 +11.1% |
| CPL Promedio (ponderado) | $5.20 | $3.87 | 🔻 +34.4% |
| CTR Promedio (ponderado) | 1.68% | 2.01% | 🔻 -16.4% |
| CPC Promedio | $0.34 | $0.29 | 🔻 +17.2% |
| CPM Promedio | $5.65 | $5.75 | 🟢 -1.7% |
| Impresiones | 9,203 | 6,063 | 🔺 +51.8% |
| Clicks | 155 | 122 | 🔺 +27.0% |
| Alcance (Reach) | 7,204 | 4,799 | 🔺 +50.1% |
| Mejor CPL del día | Pyme El Salvador: **$3.91** | Toma El control GT: $2.43 | Cambio de líder |
| Peor CPL del día (con datos) | Beco: $9.91 | Beco: N/D | Beco vuelve a reportar |

> [!caution] No confirmar como cierre real
> Estas cifras corresponden a una lectura tomada ~10 minutos antes del cierre real de 2026-09-20 y pueden moverse al resolverse la ventana de atribución de leads. Confirmar con el Reporte Performance formal cuando esté disponible (~7 AM GT).

---

## ✅ Próximas Acciones

- [ ] **Editar manualmente el horario del trigger** `trig_01DMJfrsQXaTY5KJntXisDPQ` en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ — mover de 23:50 GT a ~00:30-01:00 GT (décima ocurrencia del problema, sigue sin resolverse)
- [ ] Confirmar el cierre oficial de 2026-09-20 con el Reporte Performance formal, en particular si el sobregasto de "Urgencia" (134.8% del presupuesto) y el CPL de $9.91 de Beco se sostienen
- [ ] Investigar por qué "Urgencia" sobregastó su presupuesto diario hoy — ¿ajuste de pacing de Meta o necesidad de revisar el límite manualmente?
- [ ] Dar seguimiento al estado de atribución de Beco — hoy reportó datos por primera vez en 3 cierres, pero el patrón sigue siendo intermitente; no dar por resuelto sin más confirmaciones
- [ ] Mantener seguimiento de Pyme El Salvador — mejor CPL de la cuenta hoy, confirmar que se sostiene el crecimiento de gasto (+74.6% vs 09-19) sin deteriorar el CPL

---

## 🔗 Enlaces

- [[Daily notes/2026-09-20 - Resumen del Dia]] - Resumen del día anterior (misma alerta de timing, novena ocurrencia)
- [[Reports/2026-09-19 - Reporte Performance]] - Último reporte formal disponible (reporte de 09-20 aún pendiente, se genera ~7 AM GT)
- [[CLAUDE.md]] - Tarea de A/B testing de copys; alta volatilidad del CPL de "Toma El control" y nuevo sobregasto de "Urgencia" a seguir confirmando

#daily-note #summary #meta-ads #octopus
