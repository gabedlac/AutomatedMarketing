---
date: 2026-09-26
aliases: [reporte-2026-09-26, performance-26-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-26

> [!info] Datos de cierre confirmados
> Pull realizado la mañana del 2026-09-27 (rutina "Daily Meta Ads Performance Report - 7 AM Guatemala") con `time_range` explícito (`2026-09-26` a `2026-09-26`), día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto $45.53, impresiones 6,897, clicks 90, y `cost_per_lead` blendeado $15.18 = $45.53 / 3 leads confirmados). El activity log de la cuenta para la ventana 2026-09-26 00:00 UTC hasta el momento de este pull está **vacío** — sin cambios manuales registrados, a diferencia del cierre anterior (5 eventos).

> [!note] Corrección de `Daily notes/2026-09-26 - Resumen del Dia.md`
> Esa nota fue creada por la rutina "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que su lectura de "hoy" correspondía en realidad a **2026-09-25**, no a 2026-09-26 (bug de zona horaria documentado 16 veces consecutivas en el proyecto, sin corrección disponible salvo por el usuario). Este reporte corrige esa nota con los datos reales y confirmados de 2026-09-26 — ver sección de enlaces.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $15.18 USD | $6-7 | 🔴 Más del doble de la meta, +150.9% vs. 09-25 ($6.05) — peor cierre confirmado documentado en el proyecto |
| **Gasto Total** | $45.53 USD | - | 🟢 -5.9% vs. 09-25 ($48.41) |
| **Leads Totales** | 3 | 4-5/día | 🔴 Muy por debajo de meta, -62.5% vs. 09-25 (8) |
| **CTR Promedio** | 1.30% | 3-4% | 🔴 Por debajo de meta, -9.7% vs. 09-25 (1.44%) |
| **CPC Promedio** | $0.51 USD | - | 🔻 +24.4% vs. 09-25 ($0.41) |
| **CPM Promedio** | $6.60 USD | - | 🔻 +12.8% vs. 09-25 ($5.85) |
| **Impresiones** | 6,897 | - | 🔻 -16.6% vs. 09-25 (8,271) |
| **Clicks** | 90 | - | 🔻 -24.4% vs. 09-25 (119) |
| **Alcance (Reach)** | 5,393 | - | 🔻 -16.9% vs. 09-25 (6,486) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL de cuenta se dispara a $15.18 (+150.9% vs. 09-25), más del doble del techo de la meta $6-7 — el peor cierre confirmado documentado en el proyecto hasta ahora. La causa es puramente una caída de conversión: el gasto se mantiene prácticamente estable (-5.9%) mientras los leads confirmados caen de 8 a 3 (-62.5%). Tres de las 5 campañas activas (Pyme Colombia, Beco, Odoo Test) cierran hoy en cero leads, incluyendo a Beco, que ayer había registrado su mejor cierre documentado ($3.64 CPL, 3 leads).

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Toma El control de tu pyme]] (GT) — Sigue liderando, pero cae a la mitad de leads 🟡
```
CPL: $6.38 USD 🟡
Leads: 2
Gasto: $12.75 USD
Clicks: 37
CTR: 1.49%
CPC: $0.34 USD
CPM: $5.14 USD
Impresiones: 2,482
Reach: 1,994
```
**Status:** ACTIVE — Presupuesto del único ad set activo ("TestA/B Urgencia"): $15.00 (gasto = 85.0% del presupuesto)
**Insight:** Sigue siendo la única campaña con leads consistentes y dentro del límite superior de meta, pero sus leads bajan de 4 a 2 (-50%) y su CPL sube +77.4% vs. 09-25 ($3.59→$6.38) — pierde el margen amplio que mantenía en los últimos cierres.

### 2. [[Pyme El salvador]] (SV) — Logra 1 lead pero a CPL muy alto 🔴
```
CPL: $12.92 USD 🔴
Leads: 1
Gasto: $12.92 USD
Clicks: 22
CTR: 1.20%
CPC: $0.59 USD
CPM: $7.02 USD
Impresiones: 1,841
Reach: 1,510
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 103.4% del presupuesto)
**Insight:** Rompe su racha de ceros del cierre anterior (0 leads el 09-25), pero con un CPL que casi duplica el techo de la meta — no es aún una recuperación saludable.

### 3. [[Pyme Colombia]] (COL) — Pierde su único lead, cierra en cero 🔴
```
Leads: 0
Gasto: $8.12 USD
Clicks: 9
CTR: 1.58%
CPC: $0.90 USD
CPM: $14.27 USD
Impresiones: 569
Reach: 386
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 108.3% del presupuesto)
**Insight:** Pierde el único lead que había logrado el 09-25 con su primer día completo del nuevo creativo "Urgencia" — insuficiente aún para concluir sobre el desempeño real del creativo, requiere más cierres.

### 4. [[Beco]] (GT) — Colapsa de ser el segundo mejor performer a cero leads 🔴
```
Leads: 0
Gasto: $7.47 USD
Clicks: 14
CTR: 1.04%
CPC: $0.53 USD
CPM: $5.54 USD
Impresiones: 1,348
Reach: 1,187
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 74.7% del presupuesto)
**Insight:** Venía de su mejor cierre confirmado documentado el 09-25 ($3.64 CPL, 3 leads) y hoy cierra en cero — el mayor contraste de la cuenta. Sin cambio manual en el activity log que lo explique.

### 5. [[Odoo Test]] (GT) — Cierra en cero leads, extiende patrón recurrente 🔴
```
Leads: 0
Gasto: $4.27 USD
Clicks: 8
CTR: 1.22%
CPC: $0.53 USD
CPM: $6.50 USD
Impresiones: 657
Reach: 504
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 86.6% del presupuesto)
**Insight:** Ya van 4 de los últimos 6 cierres confirmados en cero leads para esta campaña — refuerza que su patrón de ceros intermitentes es más estructural (creativo, tracking o audiencia) que variance de bajo volumen.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🧪 A/B Test — "Toma El control de tu pyme" (GT)

| Ad Set | Status | Presupuesto/día | Gasto | % del presupuesto | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-------|--------------------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $12.75 | 85.0% | 37 | 1.49% | 2 | $6.38 |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | - | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | - | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | - | 0 | - | - | - |

**Nota:** "Urgencia" sigue siendo el único ad set activo del A/B test formal; su gasto baja frente al presupuesto (85.0% vs. 95.8% el cierre anterior) y su CPL sube de $3.59 a $6.38 (+77.4%), aunque sigue siendo el mejor performer de la cuenta.

## 🔄 Cambios de cuenta detectados (confirmado vía activity log)

- **Sin cambios manuales registrados.** El activity log de la cuenta para la ventana 2026-09-26 00:00 UTC hasta el momento de este pull está vacío — a diferencia del cierre anterior (reemplazo de creativo en Pyme Colombia + nuevo administrador agregado), hoy no hubo ninguna acción manual sobre presupuesto, targeting, creativo o estado de campañas.

## 💡 Insights Clave

- **El CPL de cuenta se dispara a $15.18 (+150.9% vs. 09-25), más del doble del techo de la meta $6-7** — el peor cierre confirmado documentado en el proyecto hasta ahora.
- **Los leads confirmados caen de 8 a 3 (-62.5%) con el gasto prácticamente estable (-5.9%, $48.41→$45.53)** — la caída es puramente de conversión a lead, no de inversión.
- **Tres de cinco campañas activas cierran en cero leads confirmados (Pyme Colombia, Beco, Odoo Test)** — la peor distribución documentada en el proyecto; incluye a Beco, que el cierre anterior había sido el segundo mejor performer con su mejor resultado documentado ($3.64 CPL, 3 leads).
- **CTR cae a 1.30% (-9.7% vs. 09-25) y CPC sube a $0.51 (+24.4%)** — el tráfico fue menos eficiente y se agrava también el problema de conversión click→lead.
- **CPM sube a $6.60 (+12.8% vs. 09-25)** — a diferencia de cierres anteriores donde el CPM se mantenía estable, hoy sí hay presión al alza en el costo de exposición, no solo en clics y conversión.
- **Sin ningún cambio manual registrado en el activity log** — el deterioro no está asociado a ninguna acción operativa visible; podría deberse a fluctuación normal de subasta/audiencia en una cuenta de bajo volumen, o requerir revisión de tracking/pixel de leads.
- **Este cierre confirma, con variaciones mínimas, la lectura casi-final documentada en [[Daily notes/2026-09-27 - Resumen del Dia]]:** CPL confirmado $15.18 vs. $15.08 casi-final, 3 leads en ambas lecturas, gasto $45.53 vs. $45.23 — la ventana de atribución no sumó leads adicionales tras el cierre.

## ✅ Recomendaciones Accionables

- [ ] **Investigar el colapso de Beco** (de $3.64 CPL / 3 leads el cierre anterior a $0 leads hoy) sin cambio manual registrado — evaluar si es volatilidad normal o requiere revisión de creativo/targeting.
- [ ] **Dar seguimiento a Pyme El Salvador:** logra 1 lead pero con CPL $12.92, casi el doble del techo de meta — no es aún una recuperación saludable.
- [ ] **Investigar por qué Pyme Colombia pierde su único lead** tras el primer día completo con el nuevo creativo "Urgencia" — requiere más cierres para evaluar el creativo con confianza.
- [ ] **Investigar el patrón recurrente de ceros en Odoo Test** (4 de los últimos 6 cierres confirmados en cero) — sugiere un problema estructural más que variance de bajo volumen.
- [ ] **Ajustar el `daily_budget` de Pyme Colombia y Pyme El Salvador:** ambas cierran sobre presupuesto (108.3% y 103.4% respectivamente).
- [ ] Retomar el A/B testing pendiente de los 5 nuevos copys en "Toma El control de tu pyme" (GT), documentado en el proyecto pero aún sin iniciar formalmente en esa campaña.
- [ ] **Usuario:** dado el peor cierre confirmado del proyecto (CPL $15.18, más del doble de la meta) y que 3 de 5 campañas activas cierran en cero leads sin explicación operativa, evaluar revisar el pixel/tracking de leads de la cuenta o pausar temporalmente las campañas en cero hasta identificar la causa.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche — 16ª ocurrencia consecutiva documentada, causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior. Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo (rechazado explícitamente por el sistema en sesiones anteriores).

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-26 - Resumen del Dia]] - Nota del día (corregida con el cierre confirmado; antes contenía por error datos casi-finales de 09-25)
- [[Daily notes/2026-09-27 - Resumen del Dia]] - Lectura casi-final registrada anoche por la otra rutina automatizada, consistente con este cierre confirmado
- [[Reports/2026-09-25 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7; A/B test de 5 copys mejorados pendiente de formalizar
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-26
Tags: #daily-note #performance #meta-ads #octopus
