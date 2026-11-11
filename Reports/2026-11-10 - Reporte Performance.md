---
date: 2026-11-10
aliases: [reporte-2026-11-10, performance-10-nov]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-11-10

> [!warning] Nota sobre el historial reciente
> Esta nota documenta el cierre real de **2026-11-10** obtenido vía `ads_get_ad_entities` para `act_2530001557366648` (GT | Octopus Innovations) en la rutina ejecutada el 2026-11-11. Se detectó que el archivo [[Daily notes/2026-11-11 - Resumen del Dia]] contiene (bajo la fecha 2026-11-11) datos que coinciden con el cierre de ayer (2026-11-10) — parecen corresponder a esta misma jornada pero etiquetados con la fecha de ejecución en vez de la fecha del dato. Además, [[Daily notes/2026-11-10 - Resumen del Dia]] (sin acento) afirma que el conector estuvo bloqueado "19 días consecutivos" ese mismo día, lo cual contradice que sí hay datos reales disponibles para esa fecha. Se deja esta nota como la versión corregida y con fecha verificada; recomendado revisar y conciliar ambos archivos con el usuario.

## 📋 Resumen Ejecutivo

| Métrica (blendeada, 7 campañas lead-gen) | Valor 2026-11-10 | Meta | Status |
|---|---|---|---|
| CPL Promedio | $11.44 USD | $6-7 | 🔴 Muy por encima de la meta (+63% sobre el techo) |
| Gasto Total (lead-gen) | $102.97 USD | - | — |
| Gasto Total de cuenta (incl. evento) | $109.84 USD | - | — |
| Leads Totales | 9 | 4-5/día | 🟢 Por encima del mínimo, pero 🔴 -44% vs. ayer |
| CTR Promedio | 1.53% | 3-4% | 🔴 Por debajo de meta (aunque mejoró vs. ayer) |
| Impresiones (lead-gen) | 11,059 | - | — |
| Clicks (lead-gen) | 169 | - | — |
| ROAS | No aplica | - | Lead-gen sin tracking de valor de compra |

**Lectura rápida:** el CPL blendeado se deterioró fuertemente frente al día anterior — pasó de $5.15 (dentro de meta, 2026-11-09) a **$11.44** (muy por encima de la meta $6-7), mientras los leads cayeron de 16 a 9 (-44%) con un gasto mayor (+24.5%). El CTR mejoró levemente (1.24% → 1.53%) pero sigue muy por debajo de la meta 3-4%.

## 🎯 Performance por Campaña (2026-11-10, ranked por CPL)

| # | Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|---|
| 1 | SLV \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $10.33 | 1,211 | 25 | 2.06% | 3 | **$3.44** |
| 2 | COL \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $10.31 | 758 | 7 | 0.92% | 2 | $5.16 |
| 3 | SLV \| Beco \| CP \| Conjuntos | 🟡 ACTIVE | $10.53 | 1,193 | 21 | 1.76% | 1 | $10.53 |
| 4 | GT \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $14.84 | 1,557 | 34 | 2.18% | 1 | $14.84 |
| 5 | GT \| Odoo \| CP \| Servicios | 🔴 ACTIVE | $34.19 | 3,384 | 59 | 1.74% | 2 | $17.10 |
| 6 | PY \| Odoo \| CP \| Servicios | 🔴 ACTIVE | $12.47 | 1,689 | 17 | 1.01% | 0 | — (sin leads) |
| 7 | PY \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $10.30 | 1,267 | 6 | 0.47% | 0 | — (sin leads) |
| — | Evento: gestión de nómina (Odoo) | ⚪ ACTIVE (EVENT_RESPONSES, no lead-gen) | $6.87 | 11,574 | 264 | 2.28% | n/a (86 RSVP) | n/a |

**Resto de la cuenta — todo PAUSED, sin cambios conocidos:** "[2026-08][Lead Generation][Odoo][GT] - Toma El control de tu pyme", "...[USA]", "...[COL] - Pyme Colombia", "...[SV] - Pyme El Salvador", "...[GT] - Beco", "...[GT] - Odoo Test", COL Odoo/Beco (versión anterior), ambos boosts de "Evento: Odoo en Acción", Accurate Partners - Loyalti, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales.

## 💡 Insights Clave

1. **Deterioro generalizado de CPL impulsado por las dos campañas de mayor gasto.** GT Odoo (33% del gasto lead-gen, $34.19) cayó de 8 a 2 leads vs. el día anterior con gasto casi idéntico ($32.53→$34.19); su CPL pasó de $4.07 a $17.10. GT Beco cayó de 3 a 1 lead ($3.95→$14.84 de CPL). Entre las dos explican la mayor parte del aumento del CPL blendeado de la cuenta.
2. **PY | Odoo colapsó a 0 leads** tras ser la campaña más eficiente el día anterior ($2.84 CPL, 3 leads) — con gasto incluso mayor ($12.47 vs $8.52). Señal de posible fatiga de creativo, problema de landing/formulario, o variación normal de volumen bajo; requiere revisión antes de seguir invirtiendo igual.
3. **PY | Beco acumula 2 días consecutivos sin ningún lead** (2026-11-09 y 2026-11-10) con gasto sostenido (~$10/día) — mismo patrón de alerta que ya se documentó el día anterior, ahora confirmado como tendencia y no un evento aislado.
4. **Lado positivo:** SLV Odoo y COL Odoo mejoraron notablemente — SLV Odoo bajó de $7.64 a $3.44 de CPL (3 leads) y COL Odoo de $8.19 a $5.16 (2 leads). SLV Beco generó su primer lead confirmado del período reciente.
5. **CTR sigue estructuralmente bajo** (1.53% vs meta 3-4%), aunque mejoró respecto a ayer (1.24%) — consistente con el diagnóstico de [[CLAUDE.md]] sobre copys genéricos sin urgencia, que sigue sin probarse en A/B en las campañas activas actuales.
6. **ROAS no aplica** — cuenta 100% lead-gen sin pixel de valor de compra configurado para estas campañas.

## ✅ Recomendaciones Accionables

- [ ] **Prioridad alta:** Revisar GT | Odoo y GT | Beco (las dos campañas de mayor gasto) antes de seguir gastando al mismo ritmo — la caída de leads con gasto estable sugiere fatiga de creativo o problema de conversión click→lead, no de presupuesto.
- [ ] Investigar por qué PY | Odoo pasó de 3 leads/$2.84 CPL a 0 leads de un día a otro con mayor gasto — revisar landing page, formulario y entrega del ad set.
- [ ] Pausar o reestructurar PY | Beco si no genera leads un tercer día consecutivo (lleva 2 días a $0 leads con ~$10/día de gasto).
- [ ] Aplicar el diagnóstico de CTR bajo de [[CLAUDE.md]] (copys genéricos sin urgencia) a las 7 campañas activas — el síntoma (CTR 1.53% vs meta 3-4%) persiste en toda la estructura nueva.
- [ ] Mantener el enfoque en SLV Odoo y COL Odoo (mejoraron hoy) y documentar qué cambió ahí para replicarlo en las campañas que empeoraron.
- [ ] Conciliar y corregir los archivos de días anteriores con fechas/datos inconsistentes (ver nota al inicio de este reporte) para que el historial de [[Daily notes]] quede confiable.

## 🔗 Seguimiento

- Daily note del día: [[Daily notes/2026-11-10 - Resumen del Día]]
- Reporte anterior: [[Reports/2026-11-09 - Reporte Performance]]
- Contexto de cuenta y metas: [[CLAUDE.md]]

#daily-note #performance #meta-ads #octopus
