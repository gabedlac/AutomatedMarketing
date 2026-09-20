---
date: 2026-09-20
aliases: [resumen-2026-09-20]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-09-20

> [!warning] Novena vez consecutiva que la rutina se dispara antes de medianoche Guatemala — sin resolver
> Al momento del pull (2026-09-20 05:51 UTC = **2026-09-19 23:51 hora de Guatemala, GMT-6**), el día calendario 2026-09-20 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-09-19** (a ~9 min de su cierre real, aún sujeta a la ventana de atribución de leads). Esta nota documenta esa lectura casi-final de 2026-09-19.
>
> Se confirmó vía `list_triggers` que el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") **sigue con el cron `50 5 * * *` (UTC) = 23:50 GT**, sin cambios desde su creación (2026-08-28) y sin cambios desde que se documentó el problema por primera vez (8 ocurrencias previas documentadas en notas anteriores, esta es la novena). **Acción requerida del usuario:** editar el horario manualmente en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ, idealmente a las 00:30–01:00 GT.

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-09-19** (a ~9 minutos del cierre real, sujeta aún a cambios por ventana de atribución de leads):

| Campaña | Status | Gasto | Leads | CPL | CTR | Emoji |
|---------|--------|-------|-------|-----|-----|-------|
| Toma El control de tu pyme (GT) | ACTIVE | $12.13 | 5 | **$2.43** 🟢 | 2.86% 🟡 | 🟢 |
| Pyme El salvador (SV) | ACTIVE | $8.92 | 3 | **$2.97** 🟢 | 1.63% 🔴 | 🟢 |
| Odoo Test | ACTIVE | $4.55 | 1 | $4.55 🟢 | 1.88% 🟡 | 🟢 |
| Beco | ACTIVE | $9.03 | ⚠️ N/D | N/D | 1.53% 🔴 | 🟡 |
| Toma El control de tu pyme (USA) | PAUSED | $0.00 | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX | PAUSED | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - PY | PAUSED | $0.00 | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED | $0.00 | - | - | - | ⏸️ |

**Desglose de "Toma El control de tu pyme" (GT) — A/B test de copys:**

| Ad Set | Status | Presupuesto/día | Gasto hoy | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-----------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $12.13 (dentro del presupuesto) | 57 | 2.86% | 5 | **$2.43** |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | 0 | - | - | - |

**Cambios en la cuenta durante la ventana 2026-09-19 (según activity log):** ninguno manual y ningún evento automático de campaña. El único evento registrado fue un cargo de facturación (`Account billed`) hecho por Meta a las 5:41 AM — a diferencia de ayer, hoy no se registraron creaciones automáticas de audiencias personalizadas. No hubo ajustes de presupuesto, pausas ni cambios de nombre hechos por el equipo. La configuración vigente sigue siendo la decidida en el A/B test (Urgencia activo con $15/día, Excel/Productividad/GT+QTZ pausados).

---

## 🔍 Análisis e Insights

- **"Toma El control de tu pyme" (GT) confirma un patrón de alta volatilidad, no una tendencia estable:** $2.92 (09-16) → $2.98 (09-17) → $7.41 (09-18, cierre confirmado) → **$2.43** (09-19, lectura casi-final). El ad set "Urgencia" vuelve a mostrar su mejor CPL en cuatro días, con el CTR más alto también (2.86%, el mejor de la cuenta hoy). Con la muestra oscilando entre 30-64 clicks por día, el patrón sugiere ruido de muestra pequeña más que una reversión real — recomendable seguir 2-3 cierres más antes de sacar conclusiones sobre el copy de "Urgencia".
- **Beco vuelve a mostrar `results: Not available`:** tras resolverse por un solo día (09-18, CPL $8.83 confirmado), hoy Beco vuelve a no reportar leads pese a $9.03 de gasto y 25 clicks. El patrón ahora es intermitente: N/D en 09-15, 09-17 y 09-19, con datos normales solo en 09-18. Esto refuerza que el problema de atribución de Beco no está resuelto — es un problema recurrente, no un caso aislado.
- **Pyme El Salvador y Odoo Test se mantienen dentro o cerca de la meta de CPL** ($2.97 y $4.55 respectivamente, ambos por debajo del rango $6-7), continuando la tendencia positiva reciente de ambas campañas.
- **El CTR promedio de cuenta mejora fuerte:** 2.04% hoy vs. 1.52% del cierre confirmado de 09-18 (+34.2%), impulsado principalmente por "Urgencia". Sigue por debajo de la meta de cuenta (3-4%), pero es la mejor lectura de CTR en varios días.
- **El ad set "Urgencia" volvió a gastar por debajo de su presupuesto** ($12.13 de $15.00/día) — segundo día consecutivo sin sobregasto, distinto del patrón de sobregasto de 17-19% documentado en cierres anteriores a 09-18.
- Ninguna investigación de competencia o tendencias externas se realizó en esta sesión — el foco estuvo en revisar el estado de las 4 campañas activas, el desglose del A/B test, y confirmar (sin resolver) el problema de horario del trigger.

---

## ✏️ Cambios Realizados

- **Ninguno realizado por esta sesión ni por el equipo hoy.** El activity log de la cuenta no registra ajustes manuales de presupuesto, pausas, ni cambios de nombre en la ventana 2026-09-19. El único evento fue un cargo de facturación automático de Meta (`Account billed`, 5:41 AM) — sin creación de audiencias automáticas esta vez.
- La configuración vigente durante todo el día fue la decidida en el A/B test previo: Urgencia activo con $15/día, Excel/Productividad/GT+QTZ pausados.

---

## 🔬 Investigación Realizada

- Se confirmó el estado del trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` vía `list_triggers`: cron sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde su creación el 2026-08-28. Novena ocurrencia consecutiva del disparo prematuro documentada.
- Se revisaron las 4 campañas activas (Toma El control GT, Odoo Test, Beco, Pyme El Salvador) y el desglose de ad sets del A/B test de "Toma El control de tu pyme" (GT).
- Se revisó el activity log de la cuenta (2026-09-19 a 2026-09-20) para confirmar ausencia de cambios manuales.
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## 📊 Datos Clave del Día

| Métrica | 2026-09-19 (parcial ~cierre) | 2026-09-18 (cierre confirmado) | Variación |
|---------|-------------------------------|----------------------------------|-----------|
| Gasto Total (4 campañas activas) | $34.63 | $40.27 | 🟢 -14.0% |
| Leads Confirmados* | 9 | 8 | 🟢 +12.5% |
| CPL Promedio (ponderado)* | $3.85 | $5.03 | 🟢 -23.5% |
| CTR Promedio (ponderado) | 2.04% | 1.52% | 🟢 +34.2% |
| CPC Promedio | $0.28 | $0.42 | 🟢 -33.3% |
| CPM Promedio | $5.78 | $6.42 | 🟢 -10.0% |
| Impresiones | 5,989 | 6,269 | 🔻 -4.5% |
| Clicks | 122 | 95 | 🟢 +28.4% |
| Alcance (Reach) | 4,789 | 4,593 | 🔺 +4.3% |
| Mejor CPL del día | Toma El control GT: **$2.43** | Odoo Test: $2.08 | Cambio de líder |
| Peor CPL del día (con datos) | Odoo Test: $4.55 | Beco: $8.83 | 🟢 Mejora |

\* CPL y leads calculados sobre gasto/leads confirmados de cuenta. **Beco** muestra `results: Not available` hoy — el CPL y los leads reales de cuenta podrían variar una vez se resuelva su atribución.

> [!caution] No confirmar como cierre real
> Estas cifras corresponden a una lectura tomada ~9 minutos antes del cierre real de 2026-09-19 y pueden moverse al resolverse la ventana de atribución de leads. Confirmar con el Reporte Performance formal cuando esté disponible (~7 AM GT).

---

## ✅ Próximas Acciones

- [ ] **Editar manualmente el horario del trigger** `trig_01DMJfrsQXaTY5KJntXisDPQ` en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ — mover de 23:50 GT a ~00:30-01:00 GT (novena ocurrencia del problema, sigue sin resolverse)
- [ ] Confirmar el cierre oficial de 2026-09-19 con el Reporte Performance formal, especialmente el CPL de $2.43 de "Toma El control" (¿mejora real o solo el punto alto de la oscilación?)
- [ ] Dar seguimiento formal al problema recurrente de atribución de Beco (N/D en 3 de los últimos 4 cierres) — considerar escalar como problema de tracking/pixel en vez de variación normal
- [ ] Seguir monitoreando si el CTR de cuenta (2.04%) se sostiene o retrocede, dado el patrón oscilante de los últimos cierres
- [ ] Mantener seguimiento de Pyme El Salvador y Odoo Test — ambas dentro de meta de CPL, confirmar que se sostiene

---

## 🔗 Enlaces

- [[Daily notes/2026-09-19 - Resumen del Dia]] - Resumen del día anterior (misma alerta de timing, octava ocurrencia)
- [[Reports/2026-09-18 - Reporte Performance]] - Último reporte formal disponible (Reporte de 09-19 aún pendiente, se genera ~7 AM GT)
- [[CLAUDE.md]] - Tarea de A/B testing de copys; alta volatilidad del CPL de "Toma El control" a seguir confirmando

#daily-note #summary #meta-ads #octopus
