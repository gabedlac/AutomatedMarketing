---
date: 2026-10-12
aliases: [reporte-2026-10-12, performance-12-oct]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-10-12

> [!info] Fuente de datos
> Generado por la rutina "Daily Meta Ads Performance Report - 7 AM Guatemala" el 2026-10-13, con `date_preset=yesterday` sobre la cuenta GT | Octopus Innovations (2530001557366648), día 2026-10-12 ya cerrado en horario de cuenta (GMT-6). El total a nivel cuenta (gasto $36.36, impresiones 6,582, clicks 100, leads 3) cuadra exactamente con la suma de las 4 campañas activas con gasto (Pyme Colombia tuvo $0.00). Se validó el activity log de la cuenta para la ventana 2026-10-12 06:00–2026-10-13 06:30 UTC: **cero eventos registrados** (ni ajustes de presupuesto, targeting, copy ni estado de campaña), por lo que la caída de leads no se explica por ningún cambio manual detectado.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio (blendeado)** | $12.12 USD | $6-7 | 🔴 73-100% por encima del rango meta; +83.1% vs. 10-11 ($6.62) |
| **Gasto Total** | $36.36 USD | - | 🔻 -31.4% vs. 10-11 ($52.98) |
| **Leads Totales** | 3 | 4-5/día | 🔴 Muy por debajo de la meta diaria; -62.5% vs. 10-11 (8) |
| **CTR Promedio** | 1.52% | 3-4% | 🔴 Por debajo de meta, pero mejora; +8.6% vs. 10-11 (1.40%) |
| **CPC Promedio** | $0.36 USD | - | 🟢 -14.3% vs. 10-11 ($0.42) |
| **CPM Promedio** | $5.52 USD | - | 🟢 -6.6% vs. 10-11 ($5.91) |
| **Impresiones** | 6,582 | - | 🔻 -26.6% vs. 10-11 (8,970) |
| **Clicks** | 100 | - | 🔻 -20.6% vs. 10-11 (126) |
| **Alcance (Reach)** | 4,944 | - | 🔻 -26.3% vs. 10-11 (6,710) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota clave:** El CPL blendeado sube +83.1% a $12.12, revirtiendo de golpe la mejora documentada el 10-11 (cuando por primera vez había entrado en el rango meta $6-7) y volviendo a un nivel comparable al peor cierre reciente (10-10: $12.87). Los leads caen -62.5% (de 8 a 3) mientras el gasto baja solo -31.4%, señal de que el problema es de **conversión**, no de presupuesto ni de calidad de tráfico: el CTR mejora (+8.6%), el CPC baja (-14.3%) y el CPM baja (-6.6%). Tres de las cuatro campañas con gasto activo (Beco, Pyme El Salvador y Odoo Test parcialmente) cerraron sin generar los leads que habían aportado el día anterior.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. Odoo Test (GT) — Único performer dentro de rango meta 🟢
```
CPL: $4.70 USD 🟢
Leads: 1
Gasto: $4.70 USD (95.3% del presupuesto diario de $4.93)
Clicks: 17
Impresiones: 677
CTR: 2.51% 🟡 (el más alto del día)
CPC: $0.28 USD
CPM: $6.94 USD
Alcance: 550
Status: ACTIVE
```

### 2. Toma El control de tu pyme (GT) — Campaña ancla, sigue convirtiendo pero con CPL más alto 🟡
```
CPL: $6.13 USD 🟡 (ligeramente por encima del rango meta)
Leads: 2
Gasto: $12.26 USD (81.7% del presupuesto de ad set de $15.00; N/D a nivel campaña — presupuesto ABO)
Clicks: 32
Impresiones: 1,922
CTR: 1.66% 🔴
CPC: $0.38 USD
CPM: $6.38 USD
Alcance: 1,591
Status: ACTIVE
```

### 3. Beco (GT) — Cero leads, revierte su mejor día documentado 🔴
```
CPL: N/A (0 leads) 🔴
Leads: 0
Gasto: $9.31 USD (93.1% del presupuesto diario de $10.00)
Clicks: 28
Impresiones: 2,152
CTR: 1.30% 🔴
CPC: $0.33 USD
CPM: $4.33 USD
Alcance: 1,730
Status: ACTIVE
```
> [!warning] Caída abrupta
> Beco había cerrado el 10-11 con el mejor CPL de la cuenta ($4.15, 3 leads). Hoy gasta 93.1% de su presupuesto diario sin generar ningún lead, pese a CTR/CPC/CPM estables o mejores que ayer.

### 4. Pyme El Salvador (SV) — Cero leads, segundo día consecutivo en rojo 🔴
```
CPL: N/A (0 leads) 🔴
Leads: 0
Gasto: $10.09 USD (80.7% del presupuesto diario de $12.50)
Clicks: 23
Impresiones: 1,831
CTR: 1.26% 🔴 (el más bajo del día)
CPC: $0.44 USD
CPM: $5.51 USD
Alcance: 1,426
Status: ACTIVE
```

### 5. Pyme Colombia (COL) — Tercer día consecutivo sin ninguna entrega ⚠️🔴
```
CPL: N/A (0 leads, $0 gasto) 🔴
Leads: 0
Gasto: $0.00 USD (0.0% del presupuesto diario de $7.50)
Clicks: 0
Impresiones: 0
CTR: N/A
CPC: N/A
CPM: N/A
Alcance: 0
Status: ACTIVE (campaña), pero delivery = "completed" (sub-status: all_ad_sets_completed)
```
> [!warning] Mismo problema reportado el 10-10 y el 10-11, aún sin resolver — 3er día consecutivo
> El ad set de esta campaña sigue en `delivery: completed` (`all_ad_sets_completed`) y con `budget_remaining` igual a su presupuesto diario completo ($7.50). Sin extender su `end_time` o asignarle presupuesto nuevo, esta campaña continuará en $0.00 de gasto y 0 leads indefinidamente.

### Campañas pausadas (sin gasto, $0.00) ⏸️
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 💡 Insights Clave

1. **El CPL blendeado sube +83.1% a $12.12**, revirtiendo por completo la mejora del 10-11 y acercándose al peor cierre reciente documentado (10-10: $12.87). Queda 73-100% por encima del rango meta $6-7.
2. **Los leads caen -62.5% a 3** (vs. 8 el 10-11) con un gasto que solo baja -31.4% — la caída de leads es casi el doble de pronunciada que la caída de gasto, confirmando un problema de **conversión clic→lead**, no de presupuesto.
3. **La conversión clic→lead colapsa de 6.35% a 3.00%** (3 leads / 100 clicks vs. 8 leads / 126 clicks el 10-11) — el motor principal de la subida de CPL.
4. **El tráfico no es la causa**: CTR sube +8.6% (1.52% vs. 1.40%), CPC baja -14.3% ($0.36 vs. $0.42) y CPM baja -6.6% ($5.52 vs. $5.91). El tráfico llegó más barato y con mejor CTR que ayer, pero convirtió mucho menos.
5. **Beco (GT) y Pyme El Salvador (SV) cierran en cero leads hoy**, tras haber aportado juntas 4 de los 8 leads del 10-11 (Beco 3, El Salvador 1) — una reversión abrupta y sin cambios de configuración detectados en el activity log que la explique.
6. **Pyme Colombia acumula su 3er día consecutivo sin ninguna entrega** ($0.00 de gasto, 0 impresiones, delivery "completed"), el mismo problema diagnosticado el 10-10 (ad set vencido), aún sin intervención.
7. **Odoo Test (GT) es hoy el único performer dentro del rango meta** ($4.70 CPL, 1 lead), tras cerrar en cero leads el día anterior — confirma el patrón intermitente ya documentado en reportes previos.
8. **"Toma El control de tu pyme" (GT) sigue convirtiendo pero con CPL más alto** ($6.13 vs. $4.46 el 10-11), aún dentro de un margen aceptable cerca del rango meta.
9. **Sin cambios manuales ni automáticos detectados**: el activity log de la ventana 2026-10-12 06:00–2026-10-13 06:30 UTC no registra ningún evento, descartando que un ajuste humano o de Meta explique la caída.

## ✅ Recomendaciones Accionables

- [ ] **Urgente — investigar por qué Beco y Pyme El Salvador cerraron en cero leads** tras haber convertido bien el día anterior, pese a CTR/CPC/CPM estables o mejores: revisar el funcionamiento del formulario de leads, el pixel/tracking y posible fatiga de audiencia o creativo antes de mover presupuesto.
- [ ] **Urgente — sigue sin resolver "Pyme Colombia"** (3er día consecutivo en $0.00 de gasto, delivery "completed"): extender el `end_time` del ad set y/o asignar presupuesto nuevo.
- [ ] **Monitorear si la caída de hoy es puntual o el inicio de una tendencia**: comparar con el cierre de 10-13 antes de reasignar presupuesto entre campañas, dado que el CPL ya mostró alta variabilidad día a día en la serie reciente (10-10: $12.87 → 10-11: $6.62 → 10-12: $12.12).
- [ ] **Aprovechar que "Toma El control de tu pyme" sigue siendo la campaña más estable**: lanzar por fin el A/B testing de los 5 copys documentado en [[CLAUDE.md]] (pendiente desde el 2026-08-24, ~50 días) para reducir la dependencia de Beco y El Salvador mientras se investiga su caída.
- [ ] **Dar seguimiento a Odoo Test**: confirmó 1 lead hoy tras cero ayer — seguir monitoreando el patrón intermitente antes de decidir si pausar o mantener activa.

## 🔗 Seguimiento

Ver registro del día en [[Daily notes/2026-10-12 - Resumen del Día]].

#daily-note #performance #meta-ads #octopus
