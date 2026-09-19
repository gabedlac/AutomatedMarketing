---
date: 2026-09-18
aliases: [reporte-2026-09-18, performance-18-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-18

> [!info] Datos de cierre confirmados
> Pull realizado 2026-09-19 (07:05 hora de Guatemala) con `date_preset=yesterday`, día ya cerrado completamente en horario de Guatemala (GMT-6). Este reporte reemplaza y confirma la lectura parcial (~10 min antes del cierre) documentada en [[Daily notes/2026-09-18 - Resumen del Dia]].

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $5.03 USD | $6-7 | 🟢 Por debajo de la meta |
| **Gasto Total** | $40.27 USD | - | 🔻 -8.9% vs. 09-17 ($44.22) |
| **Leads Totales** | 8 | 4-5/día | 🟢 Supera la meta (+60%); primera vez con atribución completa en las 4 campañas activas |
| **CTR Promedio** | 1.52% | 3-4% | 🔴 Sigue por debajo de meta, retrocede -13.6% vs. 09-17 (1.76%) |
| **CPC Promedio** | $0.42 USD | - | 🔺 +23.5% vs. 09-17 ($0.34) |
| **CPM Promedio** | $6.42 USD | - | 🔺 +6.5% vs. 09-17 ($6.03) |
| **Impresiones** | 6,269 | - | 🔻 -14.5% vs. 09-17 |
| **Clicks** | 95 | - | 🔻 -26.4% vs. 09-17 |
| **Alcance (Reach)** | 4,593 | - | 🔻 -15.6% vs. 09-17 |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** por primera vez en varios cierres, las 4 campañas activas muestran `results` disponibles (sin `Not available`) — el gasto de las 4 campañas ($40.27) cuadra exactamente con el gasto total de cuenta.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Odoo Test]] — Mejor CPL del día, atribución resuelta 🟢
```
CPL: $2.08 USD 🟢
Leads: 3
Gasto: $6.25 USD
Clicks: 14
CTR: 1.90%
CPC: $0.45 USD
CPM: $8.47 USD
Impresiones: 738
Reach: 529
```
**Status:** ACTIVE
**Insight:** Primera vez con leads confirmados tras mostrar `results: Not available` en los cierres de 09-15 y 09-17 (problema de atribución señalado en el reporte anterior). Pasa de ser la campaña con el problema de tracking más persistente a la de mejor CPL de la cuenta en un solo cierre.

### 2. [[Pyme El salvador]] (SV) — Tercera mejora consecutiva, dentro de meta por primera vez 🟢
```
CPL: $5.19 USD 🟢
Leads: 2
Gasto: $10.37 USD
Clicks: 34
CTR: 1.88%
CPC: $0.31 USD
CPM: $5.74 USD
Impresiones: 1,806
Reach: 1,357
```
**Status:** ACTIVE
**Insight:** Mejora sostenida: $10.83 → $7.18 → **$5.19**. Primer cierre confirmado dentro del rango meta de cuenta ($6-7), de hecho por debajo. Tres días consecutivos de mejora.

### 3. [[Toma El control de tu pyme]] (GT) — Revierte su racha de mínimos históricos 🟡
```
CPL: $7.41 USD 🟡
Leads: 2
Gasto: $14.82 USD
Clicks: 31
CTR: 1.31%
CPC: $0.48 USD
CPM: $6.26 USD
Impresiones: 2,368
Reach: 1,840
```
**Status:** ACTIVE
**Insight:** Tras dos cierres consecutivos con CPL récord ($2.92 el 09-16, $2.98 el 09-17), el cierre confirmado de hoy sube a **$7.41** — de vuelta cerca del problema original de [[CLAUDE.md]] ($9.29). El CTR también cae de ~2.2% a 1.31%. Con solo 31 clicks, la muestra es pequeña; el ad set "Urgencia" gastó $14.82, la primera vez en varios días que se mantiene dentro de su presupuesto de $15.00 (venía sobregastando 17-19%). Confirma la reversión ya señalada en la lectura parcial documentada en [[Daily notes/2026-09-18 - Resumen del Dia]].

### 4. [[Beco]] — Atribución resuelta, pero CPL más alto de la cuenta 🔴
```
CPL: $8.83 USD 🔴
Leads: 1
Gasto: $8.83 USD
Clicks: 16
CTR: 1.18%
CPC: $0.55 USD
CPM: $6.51 USD
Impresiones: 1,357
Reach: 1,068
```
**Status:** ACTIVE
**Insight:** También recupera atribución tras `results: Not available` en 09-15 y 09-17, pero con solo 1 lead a partir de 16 clicks, queda como el CPL más alto de la cuenta hoy y por encima de la meta ($6-7).

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🧪 A/B Test — "Toma El control de tu pyme" (GT)

| Ad Set | Status | Presupuesto/día | Gasto | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $14.82 (dentro del presupuesto) | 31 | 1.31% | 2 | **$7.41** |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | 0 | - | - | - |

**Cambios de cuenta durante la ventana 09-18 (según activity log):** ninguno manual. Solo eventos automáticos de Meta: creación de 4 audiencias personalizadas (`asa_auto_custom_audience`) a las 4:10 AM. No hubo ajustes de presupuesto, pausas ni cambios de nombre por parte de Gabriel Calderon.

## 💡 Insights Clave

- **Se resuelve (al menos por un día) el problema de atribución de Beco y Odoo Test**: ambas campañas mostraron `results: Not available` en los cierres confirmados de 09-15 y 09-17, y hoy las dos reportan leads normalmente. Odoo Test incluso termina con el mejor CPL de la cuenta ($2.08). Recomendado seguir monitoreando 1-2 cierres más antes de dar el problema por resuelto definitivamente.
- **"Toma El control de tu pyme" (GT) revierte su racha de mínimos históricos**: de $2.92-$2.98 CPL en los dos cierres anteriores a **$7.41** hoy, con el CTR cayendo de ~2.2% a 1.31%. Es el primer cierre confirmado en varios días en que el ad set "Urgencia" no sobregasta su presupuesto diario ($14.82 de $15.00) — posible relación entre menor entrega/alcance y el CPL más alto. Con una muestra de solo 31 clicks / 2 leads, conviene confirmar si es variación normal o una tendencia real antes de tocar el A/B test.
- **Pyme El Salvador entra en meta por primera vez**: tercer cierre consecutivo de mejora ($10.83 → $7.18 → $5.19), ya claramente por debajo del rango meta de cuenta ($6-7).
- El gasto total de cuenta baja -8.9% vs. 09-17 ($40.27 vs $44.22), en línea con el CTR y clicks más bajos del día (-26.4% clicks).
- El CTR promedio de cuenta retrocede a 1.52% (-13.6% vs. 09-17), alejándose más de la meta de 3-4%.
- Sin cambios manuales de presupuesto, pausas ni nomenclatura durante el 09-18 — la configuración vigente sigue siendo la decidida en el A/B test (Urgencia activo, Excel pausado).

## ✅ Recomendaciones Accionables

- [ ] **Confirmar si el problema de atribución de Beco y Odoo Test quedó resuelto** o si vuelve a aparecer `results: Not available` en los próximos cierres — un solo día de datos normales no es concluyente.
- [ ] **Monitorear si la reversión de CPL de "Toma El control" (Urgencia) a $7.41 se sostiene** en el próximo cierre antes de considerar cambios al A/B test; la muestra de hoy es pequeña (31 clicks).
- [ ] **Aprovechar el momentum de Odoo Test** ($2.08 CPL, mejor de la cuenta) — evaluar si amerita más presupuesto si se confirma que la atribución quedó resuelta.
- [ ] **Mantener el seguimiento de Pyme El Salvador** — primer cierre confirmado dentro de meta, validar que se sostiene.
- [ ] Seguir sin resolver: aclarar el origen y plan de uso de los ad sets pausados "TestA/B Productividad", "TestA/B Excel" y "GT + QTZ".

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-18 - Resumen del Dia]] - Nota del día (actualizada con el cierre confirmado)
- [[Reports/2026-09-17 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Tarea de A/B testing de copys; reversión del CPL a confirmar en próximos cierres
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-18
Tags: #daily-note #performance #meta-ads #octopus
