---
date: 2026-11-09
aliases: [reporte-2026-11-09, performance-09-nov]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-11-09

> [!success] Conector Meta Ads restablecido — datos reales de vuelta tras 19 días de bloqueo
> Esta nota fue generada por la rutina "Daily Meta Ads Performance Report - 7 AM Guatemala" el 2026-11-10 a las 07:10 GT (13:10:26 UTC), con rango objetivo `2026-11-09`. A diferencia de los cierres del 10-23 al 11-08 (documentados en [[Daily notes/2026-11-10 - Resumen del Dia]] y reportes previos), esta vez las herramientas de Meta Ads respondieron con normalidad y se obtuvieron métricas reales de campaña vía `ads_get_ad_entities` para `act_2530001557366648` (GT | Octopus Innovations). **El bloqueo de 19 días consecutivos (10-23 a 11-10) queda roto desde este cierre.**
>
> **Cambio estructural importante:** la cuenta ya no gira alrededor de una sola campaña. La campaña histórica documentada en [[CLAUDE.md]] — "[2026-08][Lead Generation][Odoo][GT] - Toma El control de tu pyme" (CPL $9.29) — está **PAUSED**, igual que todo el resto de campañas legacy (USA, Odoo Test, Beco original, Pyme Colombia/El Salvador, Accurate Partners, Conversión Clientes Potenciales). La cuenta activa hoy corre **7 campañas de lead-gen** segmentadas por país × producto (GT/COL/PY/SLV × Odoo "Servicios" / Beco "Conjuntos") más 1 campaña de evento (EVENT_RESPONSES, no es lead-gen). Las metas de CPL/CTR/leads de [[CLAUDE.md]] y del README quedaron pensadas para la campaña antigua; se usan aquí como referencia de cuenta a falta de metas actualizadas, pero conviene confirmar con el usuario si siguen vigentes.

## 📋 Resumen Ejecutivo

| Métrica (blendeada, 7 campañas lead-gen) | Valor 2026-11-09 | Meta | Status |
|---|---|---|---|
| CPL Promedio | $5.15 USD | $6-7 | 🟢 Mejor que meta |
| Gasto Total (lead-gen) | $82.47 USD | - | — |
| Gasto Total de cuenta (incl. evento) | $86.55 USD | - | — |
| Leads Totales | 16 | 4-5/día | 🟢 Muy por encima (repartidos en 7 campañas) |
| CTR Promedio | 1.24% | 3-4% | 🔴 Por debajo |
| Impresiones (lead-gen) | 14,272 | - | — |
| Clicks (lead-gen) | 177 | - | — |
| ROAS | No aplica | - | Lead-gen sin tracking de valor de compra |

**Lectura rápida:** el CPL blendeado mejoró y ya está dentro/mejor que la meta histórica ($5.15 vs $6-7), pero el CTR sigue estructuralmente bajo (1.24% vs meta 3-4%) — el mismo problema de creativo/copy que documenta [[CLAUDE.md]] desde agosto, ahora repartido en más campañas. Dos de las 7 campañas activas **no generaron ningún lead** pese a gastar.

## 🎯 Performance por Campaña (2026-11-09, ranked por CPL)

| # | Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|---|
| 1 | PY \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $8.50 | 2,634 | 29 | 1.10% | 3 | **$2.83** |
| 2 | GT \| Beco \| CP \| Conjuntos | 🟢 ACTIVE | $11.85 | 1,562 | 27 | 1.73% | 3 | $3.95 |
| 3 | GT \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $32.44 | 4,340 | 70 | 1.61% | 8 | $4.06 |
| 4 | SLV \| Odoo \| CP \| Servicios | 🟡 ACTIVE | $7.54 | 1,453 | 13 | 0.89% | 1 | $7.54 |
| 5 | COL \| Odoo \| CP \| Servicios | 🟡 ACTIVE | $8.19 | 1,111 | 10 | 0.90% | 1 | $8.19 |
| 6 | PY \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $7.10 | 1,716 | 16 | 0.93% | 0 | — (sin leads) |
| 7 | SLV \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $6.85 | 1,456 | 12 | 0.82% | 0 | — (sin leads) |
| — | Evento: gestión de nómina (Odoo) | ⚪ ACTIVE (EVENT_RESPONSES, no lead-gen) | $4.08 | 7,004 | 160 | 2.28% | n/a | n/a |

**Resto de la cuenta — todo PAUSED, sin cambios conocidos:** "[2026-08][Lead Generation][Odoo][GT] - Toma El control de tu pyme", "...[USA]", "...[COL] - Pyme Colombia", "...[SV] - Pyme El Salvador", "...[GT] - Beco", "...[GT] - Odoo Test", COL Odoo/Beco (versión anterior), ambos boosts de "Evento: Odoo en Acción", Accurate Partners - Loyalti, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales.

## 💡 Insights Clave

1. **El conector volvió a funcionar** después de 19 días calendario de bloqueo (10-23 a 11-10) — primer cierre con datos reales desde el del 2026-10-22.
2. **CPL blendeado dentro de meta** ($5.15, mejor que el rango $6-7) impulsado principalmente por PY Odoo ($2.83) y GT Beco ($3.95); GT Odoo sigue siendo la campaña de mayor volumen (8 leads, $32.44 de gasto, 39% del gasto lead-gen del día).
3. **CTR sigue siendo el problema estructural** (1.24% vs meta 3-4%), igual que en el último dato confirmado de octubre — consistente con el diagnóstico de [[CLAUDE.md]] sobre copys genéricos sin urgencia, que sigue sin probarse en A/B.
4. **Dos campañas "Beco" (Conjuntos) no generaron leads hoy** — PY Beco ($7.10 gastados, 0 leads) y SLV Beco ($6.85 gastados, 0 leads) — pese a que SLV Beco sí tuvo 1 lead el día anterior (11-08) y PY Beco tuvo 3. Posible fatiga de creativo o problema de landing/formulario; requiere revisión antes de seguir escalando gasto ahí.
5. **La cuenta migró de estructura**: la campaña única que documentaba [[CLAUDE.md]] (y el Canvas de copys del 2026-08-24) está pausada. Las tareas abiertas de A/B testing de los 5 copys y el Canvas (https://claude.ai/code/artifact/a4d9fa0d-f791-4a4d-9896-63901c54ca68) probablemente quedaron obsoletas con este cambio — vale confirmar con el usuario si esas tareas se migran a las campañas nuevas o se cierran.

## ✅ Recomendaciones Accionables

- [ ] Revisar por qué "PY | Beco | CP | Conjuntos" y "SLV | Beco | CP | Conjuntos" cayeron a 0 leads el 11-09 (creativo, audiencia o landing) antes de seguir invirtiendo ahí.
- [ ] Aplicar el diagnóstico de CTR bajo de [[CLAUDE.md]] (copys genéricos sin urgencia) a las 7 campañas activas actuales, no solo a la campaña pausada original — el síntoma (CTR 1.24% vs meta 3-4%) persiste en la estructura nueva.
- [ ] Confirmar con el usuario si las tareas pendientes de [[CLAUDE.md]] (A/B testing de los 5 copys de "Toma El control de tu pyme") siguen vigentes dado que esa campaña está PAUSED, o si deben reescribirse para GT Odoo/Beco (las campañas activas de mayor volumen).
- [ ] Mantener/escalar presupuesto en GT Odoo, PY Odoo y GT Beco (mejores CPL del día); mantener vigilancia diaria sobre COL Odoo y SLV Odoo (CPL $7-8, sobre meta).
- [ ] Actualizar [[CLAUDE.md]] con la estructura de cuenta real (7 campañas país×producto) — el documento sigue describiendo solo la campaña antigua pausada.

## 🔗 Seguimiento

Ver [[Daily notes/2026-11-09 - Resumen del Dia]] para el resumen ejecutivo del día (actualizado en esta misma corrida con los datos reales de arriba, reemplazando el placeholder sin datos que tenía). Comparación día anterior en [[Daily notes/2026-11-09 - Resumen del Dia]]. Último cierre confirmado previo a este: [[Reports/2026-10-22 - Reporte Performance]].

#daily-note #performance #meta-ads #octopus
