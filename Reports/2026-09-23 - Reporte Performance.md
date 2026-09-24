---
date: 2026-09-23
aliases: [reporte-2026-09-23, performance-23-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-23

> [!info] Datos de cierre confirmados
> Pull realizado 2026-09-24 ~07:14 GT con `date_preset=yesterday`, día ya cerrado completamente en horario de Guatemala (GMT-6). El total de gasto y leads por campaña cuadra exactamente con el total de cuenta, confirmando que no hay atribución pendiente.

> [!note] Dos rutinas distintas escriben en `Daily notes/` con nombres que se pisan
> Esta rutina ("Daily Meta Ads Performance Report", cron `0 13 * * *` UTC = 7:00 AM GT) corre a la hora correcta y **no tiene el bug de las 23:50 GT** documentado en notas anteriores — ese bug pertenece a una rutina distinta, "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`, cron `50 5 * * *` UTC, sin cambios desde su creación el 2026-08-28, confirmado vía `list_triggers`). El problema real: ambas rutinas generan archivos en `Daily notes/YYYY-MM-DD - Resumen del Dia.md`, pero calculan la fecha de forma distinta (una usa "día anterior a la ejecución", la otra "fecha actual", que por el bug de horario termina siendo el día anterior también) y terminan **sobrescribiendo el mismo archivo con contenido de días distintos**. Concretamente: `Daily notes/2026-09-23 - Resumen del Dia.md` fue creado por la rutina de las 23:50 GT con datos casi-finales de **2026-09-22** (mal etiquetados), no de 2026-09-23. Este reporte corrige esa nota — ver sección de enlaces.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $10.99 USD | $6-7 | 🔴 Muy por encima de la meta — peor cierre confirmado documentado en el proyecto (supera incluso el $9.29 de agosto que motivó el A/B test de copys) |
| **Gasto Total** | $54.97 USD | - | 🔺 +16.7% vs. 09-22 ($47.09) |
| **Leads Totales** | 5 | 4-5/día | 🟡 Dentro del rango bajo de la meta, pero -37.5% vs. 09-22 (8) |
| **CTR Promedio** | 1.39% | 3-4% | 🔴 Muy por debajo de meta, +1.5% vs. 09-22 (1.37%) |
| **CPC Promedio** | $0.44 USD | - | 🟢 -2.2% vs. 09-22 ($0.45) |
| **CPM Promedio** | $6.14 USD | - | 🟢 -1.3% vs. 09-22 ($6.22) |
| **Impresiones** | 8,947 | - | 🔺 +18.2% vs. 09-22 |
| **Clicks** | 124 | - | 🔺 +19.2% vs. 09-22 |
| **Alcance (Reach)** | 6,488 | - | 🔺 +16.9% vs. 09-22 |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** El CPL de cuenta se dispara a $10.99 (+86.6% vs. 09-22), el peor cierre confirmado documentado en el proyecto. La causa es una combinación de más gasto (+16.7%) y menos leads (-37.5%): tres de las cinco campañas activas (Odoo Test, Beco, Pyme El Salvador) cerraron el día en cero leads confirmados, y la ventana de atribución no rescató ningún lead adicional para ninguna de las tres — esto confirma, sin cambios, lo que la lectura casi-final de ayer ya anticipaba.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Pyme Colombia]] (COL) — Mejor CPL confirmado de la cuenta 🟢
```
CPL: $4.31 USD 🟢
Leads: 2
Gasto: $8.62 USD
Clicks: 16
CTR: 1.62%
CPC: $0.54 USD
CPM: $8.73 USD
Impresiones: 987
Reach: 702
```
**Status:** ACTIVE — Presupuesto/día: $7.50 (gasto = 114.9% del presupuesto)
**Insight:** Mejora fuerte de $9.97 (09-22) a $4.31 (-56.8%), su mejor cierre confirmado hasta ahora, duplicando leads (1→2) con menos gasto (-13.5%). Sigue gastando por encima de su presupuesto diario configurado (114.9%), tercer día consecutivo con este patrón.

### 2. [[Toma El control de tu pyme]] (GT) — Leads sostenidos, CPL sube dentro de meta 🟢
```
CPL: $5.60 USD 🟢
Leads: 3
Gasto: $16.79 USD
Clicks: 53
CTR: 1.68%
CPC: $0.32 USD
CPM: $5.33 USD
Impresiones: 3,149
Reach: 2,453
```
**Status:** ACTIVE
**Insight:** Sigue siendo la campaña con mayor volumen de leads de la cuenta, pero retrocede desde su mejor cierre reciente ($3.02, 09-22): CPL +85.4%, leads -25% (4→3), gasto +39.1%. El ad set "Urgencia" (único activo) gasta $16.79 de $15.00 de presupuesto (111.9%), volviendo a sobregastar tras el único día dentro de presupuesto documentado. Se mantiene dentro de la meta $6-7, pero la tendencia es a la baja frente al cierre anterior.

### 3. [[Odoo Test]] (GT) — Caída más dramática del día, de líder de eficiencia a cero 🔴
```
CPL: N/D (sin leads)
Leads: 0
Gasto: $5.02 USD
Clicks: 5
CTR: 0.61%
CPC: $1.00 USD
CPM: $6.15 USD
Impresiones: 816
Reach: 711
```
**Status:** ACTIVE — Presupuesto/día: $4.93 (gasto = 101.8% del presupuesto)
**Insight:** Era la campaña más eficiente de la cuenta el 09-22 (CPL $2.22, CTR 1.69%) y hoy cierra confirmado en cero leads, con el CTR colapsando a 0.61% (-63.9%) pese a gastar 101.8% de su presupuesto. Es el mayor contraste día a día de toda la cuenta — amerita revisión inmediata de creativo y del paso de conversión (landing/formulario).

### 4. [[Beco]] (GT) — CTR mejora pero no convierte, cero leads confirmados 🔴
```
CPL: N/D (sin leads)
Leads: 0
Gasto: $11.47 USD
Clicks: 26
CTR: 1.45%
CPC: $0.44 USD
CPM: $6.39 USD
Impresiones: 1,794
Reach: 1,444
```
**Status:** ACTIVE — Presupuesto/día: $10.00 (gasto = 114.7% del presupuesto)
**Insight:** El CTR mejora +57.6% vs. 09-22 (0.92%→1.45%) pero no se traduce en ningún lead confirmado, frente a 1 lead el día anterior. La mejora de tráfico sin conversión apunta a un problema en el formulario o el paso posterior al click, no solo en el creativo. Sigue gastando por encima de presupuesto (114.7%).

### 5. [[Pyme El salvador]] (SV) — Segundo cierre confirmado consecutivo en cero leads 🔴
```
CPL: N/D (sin leads)
Leads: 0
Gasto: $13.07 USD
Clicks: 24
CTR: 1.09%
CPC: $0.54 USD
CPM: $5.94 USD
Impresiones: 2,201
Reach: 1,664
```
**Status:** ACTIVE — Presupuesto/día: $12.50 (gasto = 104.6% del presupuesto)
**Insight:** Encadena su **segundo cierre confirmado consecutivo sin leads** ($10.78 el 09-22 + $13.07 hoy, ambos en cero), pese a que el CTR sube +36.3% y el gasto +21.2%. Deja de ser variance de un solo día: era la campaña más consistente de la cuenta dentro de meta antes de esta racha. Requiere acción antes de un tercer día en cero (pausar, refrescar creativo, o auditar tracking/atribución).

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🧪 A/B Test — "Toma El control de tu pyme" (GT)

| Ad Set | Status | Presupuesto/día | Gasto | % del presupuesto | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-------|--------------------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $16.79 | 111.9% | 53 | 1.68% | 3 | $5.60 |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | - | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | - | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | - | 0 | - | - | - |

**Nota:** "Urgencia" vuelve a sobregastar (111.9% vs. 80.5% el 09-22, su único día dentro de presupuesto documentado) y su CPL sube de $3.02 a $5.60 (+85.4%), aunque se mantiene dentro de la meta $6-7.

## 💡 Insights Clave

- **El CPL de cuenta se dispara a $10.99 (+86.6% vs. 09-22), el peor cierre confirmado documentado en el proyecto** — supera incluso el $9.29 de agosto que motivó el esfuerzo de A/B testing de copys documentado en [[CLAUDE.md]].
- **Los leads caen de 8 a 5 (-37.5%) mientras el gasto sube +16.7%** ($47.09→$54.97) — la combinación exacta que dispara el CPL.
- **Tres de cinco campañas activas (Odoo Test, Beco, Pyme El Salvador) cierran confirmadas en cero leads simultáneamente**, y la ventana de atribución no rescató ningún lead adicional para ninguna — confirma sin cambios la lectura casi-final de ayer.
- **Pyme El Salvador encadena su segundo cierre confirmado consecutivo en cero leads** ($13.07 gastados, +21.2% vs. ayer) pese a mejorar su CTR — deja de ser variance de un día.
- **Odoo Test es la caída más dramática**: de líder de eficiencia (CPL $2.22, CTR 1.69%) a cero leads con CTR colapsando a 0.61%.
- **Beco mejora su CTR (+57.6%) pero sigue sin convertir** — el problema parece estar en el formulario/paso de conversión, no en el creativo.
- **Pyme Colombia es el único punto claramente positivo**: mejor cierre confirmado hasta ahora ($4.31 CPL, -56.8%), duplicando leads con menos gasto.
- **Las 4 campañas con presupuesto fijo volvieron a gastar por encima de su daily_budget** (101.8%-114.9%), patrón recurrente sin corregir.

## ✅ Recomendaciones Accionables

- [ ] **Acción urgente en Pyme El Salvador:** segundo cierre confirmado consecutivo en cero leads pese a gasto normal (~$11-13/día) — si el cierre de mañana también da cero, pausar la campaña mientras se investiga tracking/atribución o se refresca el creativo.
- [ ] **Investigar la caída de Odoo Test:** de $2.22 CPL a cero leads con CTR colapsando a 0.61% — revisar fatiga de creativo y el paso de conversión (landing/formulario), no solo el anuncio.
- [ ] **Revisar el formulario de Beco:** el CTR mejora (+57.6%) pero no genera leads — apunta a un problema de conversión post-click, no de creativo.
- [ ] **Escalar con cautela Pyme Colombia:** mejor cierre confirmado del período ($4.31 CPL) — buena candidata a subir presupuesto si se sostiene 1-2 días más, aunque ya gasta 114.9% de su presupuesto configurado.
- [ ] **Corregir el sobregasto sistemático:** las 4 campañas con presupuesto fijo (Pyme Colombia, Odoo Test, Beco, Pyme El Salvador) gastaron 101.8%-114.9% de su daily_budget — ajustar budget o revisar pacing.
- [ ] **Usuario:** confirmado que existen dos rutinas distintas escribiendo en `Daily notes/` con el mismo patrón de nombre de archivo y pisándose entre sí (ver nota de infraestructura arriba) — además del bug de horario ya reportado 13 veces en la rutina "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`, editable solo por el usuario en https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ).
- [ ] Retomar el A/B testing pendiente de los 5 nuevos copys en "Toma El control de tu pyme" (GT), documentado en el proyecto pero aún sin iniciar en esta cuenta.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-23 - Resumen del Dia]] - Nota del día (corregida con el cierre confirmado; antes contenía por error datos casi-finales de 09-22)
- [[Daily notes/2026-09-24 - Resumen del Dia]] - Lectura casi-final registrada ayer por la otra rutina automatizada, confirmada sin cambios por este reporte
- [[Reports/2026-09-22 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Meta de CPL $6-7; este cierre es el peor documentado del proyecto
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-23
Tags: #daily-note #performance #meta-ads #octopus
