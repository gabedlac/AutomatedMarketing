---
date: 2026-09-24
aliases: [reporte-2026-09-24, performance-24-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-24

> [!info] Datos de cierre confirmados
> Pull realizado 2026-09-25 ~07:19 GT con `time_range` explícito (`2026-09-24` a `2026-09-24`), día ya cerrado completamente en horario de Guatemala (GMT-6). El total de cuenta a nivel `ad_account` cuadra exactamente con la suma de las 5 campañas activas (gasto, impresiones, clicks, leads, CTR, CPC y CPM idénticos), confirmando que no hay atribución pendiente. El activity log de la cuenta para la ventana 2026-09-24 00:00–2026-09-25 13:20 UTC vino vacío, sin cambios manuales ni automatizados registrados.

> [!note] Corrección de `Daily notes/2026-09-24 - Resumen del Dia.md`
> Esa nota fue creada por la rutina "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`), que se dispara a las 23:50 GT — antes de medianoche — por lo que su lectura de "hoy" correspondía en realidad a **2026-09-23**, no a 2026-09-24 (bug de zona horaria documentado 14 veces consecutivas en el proyecto, sin corrección disponible salvo por el usuario). Este reporte corrige esa nota con los datos reales y confirmados de 2026-09-24 — ver sección de enlaces.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $4.69 USD | $6-7 | 🟢 Dentro de meta y **el mejor cierre confirmado documentado en el proyecto** (supera incluso los $5.89 del 09-22) |
| **Gasto Total** | $42.20 USD | - | 🟢 -23.2% vs. 09-23 ($54.97) |
| **Leads Totales** | 9 | 4-5/día | 🟢 Casi duplica la meta, +80.0% vs. 09-23 (5) |
| **CTR Promedio** | 1.72% | 3-4% | 🔴 Por debajo de meta, aunque +23.7% vs. 09-23 (1.39%) |
| **CPC Promedio** | $0.34 USD | - | 🟢 -22.7% vs. 09-23 ($0.44) |
| **CPM Promedio** | $5.86 USD | - | 🟢 -4.6% vs. 09-23 ($6.14) |
| **Impresiones** | 7,198 | - | 🔻 -19.5% vs. 09-23 (8,947) |
| **Clicks** | 124 | - | ⏸️ Idéntico a 09-23 (124) |
| **Alcance (Reach)** | 5,321 | - | 🔻 -18.0% vs. 09-23 (6,488) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL de cuenta cae a $4.69 (-57.3% vs. 09-23), el mejor cierre confirmado documentado en el proyecto — por debajo tanto de la meta $6-7 como del histórico $9.29 de agosto que motivó el A/B test de copys. La causa es la combinación exacta opuesta a la de ayer: menos gasto (-23.2%) y más leads (+80.0%). Las 5 campañas activas cerraron con al menos 1 lead confirmado — ninguna en cero, revirtiendo por completo el problema de las 3 campañas en cero del cierre anterior.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Toma El control de tu pyme]] (GT) — Mejor CPL confirmado del día, lidera en volumen 🟢
```
CPL: $3.04 USD 🟢
Leads: 4
Gasto: $12.14 USD
Clicks: 42
CTR: 1.71%
CPC: $0.29 USD
CPM: $4.96 USD
Impresiones: 2,449
Reach: 1,932
```
**Status:** ACTIVE — Presupuesto del único ad set activo ("Urgencia"): $15.00 (gasto = 80.9% del presupuesto)
**Insight:** Mejora fuerte de $5.60 (09-23) a $3.04 (-45.7%), su mejor CPL confirmado del período, con más leads (3→4) y menos gasto (-27.7%). Primera vez en varios días que el ad set "Urgencia" cierra por debajo de su presupuesto configurado, en vez de sobregastar.

### 2. [[Pyme Colombia]] (COL) — Retrocede levemente pero corrige su sobregasto 🟡
```
CPL: $5.03 USD 🟢
Leads: 1
Gasto: $5.03 USD
Clicks: 16
CTR: 2.83%
CPC: $0.31 USD
CPM: $8.90 USD
Impresiones: 565
Reach: 424
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 67.1% del presupuesto)
**Insight:** Baja de 2 leads ($4.31 CPL, 09-23) a 1 lead ($5.03 CPL) — sigue dentro de meta pero con menos volumen. Por primera vez en varios días gasta por debajo de su presupuesto diario (67.1%), rompiendo la racha de 3 días consecutivos de sobregasto documentada ayer.

### 3. [[Pyme El salvador]] (SV) — Rompe su racha de dos cierres consecutivos en cero 🟢
```
CPL: $5.12 USD 🟢
Leads: 2
Gasto: $10.23 USD
Clicks: 29
CTR: 1.60%
CPC: $0.35 USD
CPM: $5.63 USD
Impresiones: 1,818
Reach: 1,388
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 81.8% del presupuesto)
**Insight:** Rompe su racha de **dos cierres confirmados consecutivos en cero leads** (09-22 y 09-23) con 2 leads a $5.12 CPL, dentro de meta. El problema flagueado como potencialmente sostenido (fatiga de creativo o tracking) no se repite hoy — sugiere que fue variance de bajo volumen/atribución, aunque conviene confirmar con 1-2 cierres más.

### 4. [[Odoo Test]] (GT) — Se recupera del cierre en cero, sigue levemente sobre presupuesto 🟢
```
CPL: $5.34 USD 🟢
Leads: 1
Gasto: $5.34 USD
Clicks: 12
CTR: 1.38%
CPC: $0.45 USD
CPM: $6.14 USD
Impresiones: 869
Reach: 697
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 108.3% del presupuesto)
**Insight:** Se recupera de su cierre confirmado en cero (09-23) con 1 lead a $5.34 CPL, dentro de meta. Sigue siendo la única campaña con presupuesto fijo por encima de su límite configurado (108.3%), patrón recurrente sin corregir.

### 5. [[Beco]] (GT) — Rompe su racha de ceros, pero sigue siendo la única fuera de meta 🟡
```
CPL: $9.46 USD 🔴
Leads: 1
Gasto: $9.46 USD
Clicks: 25
CTR: 1.67%
CPC: $0.38 USD
CPM: $6.32 USD
Impresiones: 1,497
Reach: 1,152
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 94.6% del presupuesto)
**Insight:** Genera lead por primera vez en varios cierres, rompiendo su patrón crónico de ceros intermitentes, pero su CPL ($9.46) sigue siendo el único de la cuenta fuera de la meta $6-7. Dentro de presupuesto (94.6%), a diferencia de días anteriores.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🧪 A/B Test — "Toma El control de tu pyme" (GT)

| Ad Set | Status | Presupuesto/día | Gasto | % del presupuesto | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-------|--------------------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $12.14 | 80.9% | 42 | 1.71% | 4 | $3.04 |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | - | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | - | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | - | 0 | - | - | - |

**Nota:** "Urgencia" cierra por primera vez en varios días por debajo de su presupuesto (80.9% vs. 111.9% el 09-23) y su CPL mejora de $5.60 a $3.04 (-45.7%), su mejor cierre confirmado del período.

## 💡 Insights Clave

- **El CPL de cuenta cae a $4.69 (-57.3% vs. 09-23), el mejor cierre confirmado documentado en el proyecto** — por debajo de la meta $6-7 y del histórico $9.29 de agosto que motivó el A/B test de copys documentado en [[CLAUDE.md]].
- **Los leads suben de 5 a 9 (+80.0%) mientras el gasto baja -23.2%** ($54.97→$42.20) — la combinación exacta opuesta a la de ayer, y la causa directa de la mejora en CPL.
- **Las 5 campañas activas cierran confirmadas con al menos 1 lead — ninguna en cero**, revirtiendo por completo el cierre de ayer (3 de 5 en cero). No hubo intervención manual registrada en el activity log, lo que sugiere que los ceros de ayer fueron más variance de bajo volumen/atribución que un problema estructural.
- **Pyme El Salvador y Odoo Test se recuperan de sus cierres en cero** documentados ayer, ambos dentro de meta hoy ($5.12 y $5.34 CPL respectivamente).
- **Toma El control de tu pyme (GT) es el mejor cierre confirmado del período**: $3.04 CPL con el mayor volumen de leads (4), y por primera vez en varios días su ad set "Urgencia" cierra dentro de presupuesto.
- **Beco es el único punto débil de la cuenta**: sí genera lead (rompiendo su racha de ceros) pero su CPL ($9.46) sigue siendo el único fuera de la meta $6-7 entre las campañas con resultados.
- **El sobregasto sistemático mejora en 3 de 4 campañas con presupuesto fijo** (Pyme Colombia 67.1%, Pyme El Salvador 81.8%, Beco 94.6%) — solo Odoo Test sigue levemente sobre presupuesto (108.3%).

## ✅ Recomendaciones Accionables

- [ ] **Evaluar subir presupuesto a "Toma El control de tu pyme" (GT):** mejor CPL confirmado del período ($3.04) con el mayor volumen de leads, y cerró por debajo de su presupuesto configurado — buena candidata a escalar si se sostiene 1-2 días más.
- [ ] **Investigar el CPL de Beco ($9.46):** única campaña fuera de meta pese a romper su racha de ceros — revisar si el problema de conversión post-click reportado en cierres anteriores persiste.
- [ ] **Confirmar la recuperación de Pyme El Salvador y Odoo Test** en el próximo cierre, para descartar del todo que sus rachas de cero fueran un problema estructural latente (tracking, fatiga de creativo).
- [ ] **Ajustar el `daily_budget` de Odoo Test:** sigue siendo la única campaña con presupuesto fijo por encima de su límite (108.3%), patrón recurrente sin corregir.
- [ ] Retomar el A/B testing pendiente de los 5 nuevos copys en "Toma El control de tu pyme" (GT), documentado en el proyecto pero aún sin iniciar en esta cuenta.
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue disparándose a las 23:50 GT en vez de después de medianoche — 14ª ocurrencia consecutiva documentada, causando que sus notas en `Daily notes/` queden mal etiquetadas con los datos del día anterior. Solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ; ningún agente automatizado tiene permiso para editarlo (rechazado explícitamente por el sistema en sesiones anteriores).

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-24 - Resumen del Dia]] - Nota del día (corregida con el cierre confirmado; antes contenía por error datos casi-finales de 09-23)
- [[Daily notes/2026-09-25 - Resumen del Dia]] - Lectura casi-final registrada hoy por la otra rutina automatizada, consistente con este cierre confirmado (sin leads adicionales rescatados por la ventana de atribución)
- [[Reports/2026-09-23 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7; este cierre es el mejor documentado del proyecto
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-24
Tags: #daily-note #performance #meta-ads #octopus
