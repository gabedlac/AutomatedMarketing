---
date: 2026-10-10
aliases: [reporte-2026-10-10, performance-10-oct]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-10-10

> [!info] Fuente de datos
> Generado por la rutina "Daily Meta Ads Performance Report - 7 AM Guatemala" el 2026-10-11, con `date_preset=yesterday` sobre la cuenta GT | Octopus Innovations (2530001557366648), día 2026-10-10 ya cerrado en horario de cuenta (GMT-6). El total a nivel cuenta (gasto $38.62, impresiones 6,528, clicks 90, leads 3) cuadra exactamente con la suma de las 4 campañas activas con gasto (Pyme Colombia tuvo $0.00). El alcance de cuenta (5,122) es menor que la suma simple por campaña (5,204) por solapamiento normal de audiencias.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio (blendeado)** | $12.87 USD | $6-7 | 🔴 Muy por encima de la meta; peor cierre de la serie reciente, +148.9% vs. 10-09 ($5.17) |
| **Gasto Total** | $38.62 USD | - | 🟢 -17.0% vs. 10-09 ($46.54) |
| **Leads Totales** | 3 | 4-5/día | 🔴 Muy por debajo de la meta; -66.7% vs. 10-09 (9) |
| **CTR Promedio** | 1.38% | 3-4% | 🔴 Por debajo de meta; -18.3% vs. 10-09 (1.69%) |
| **CPC Promedio** | $0.43 USD | - | 🔻 +13.2% vs. 10-09 ($0.38) |
| **CPM Promedio** | $5.92 USD | - | 🟢 -8.2% vs. 10-09 ($6.45) |
| **Impresiones** | 6,528 | - | 🔻 -9.5% vs. 10-09 (7,212) |
| **Clicks** | 90 | - | 🔻 -26.2% vs. 10-09 (122) |
| **Alcance (Reach)** | 5,122 | - | 🔻 -8.0% vs. 10-09 (5,566) |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota clave:** El CPL blendeado se dispara +148.9% pese a que el gasto total baja (-17.0%). La causa es doble: los leads totales caen de 9 a 3 (-66.7%) y la conversión clic→lead se desploma de **7.38% a 3.33%** (3 leads / 90 clicks vs. 9 leads / 122 clicks el día anterior). Parte de la caída de gasto no es optimización sino la pérdida completa de una campaña: Pyme Colombia pasó de gastar normalmente a $0.00 (ver insight #2).

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. Beco (GT) — Mejor CPL de la cuenta, pero por encima del rango meta 🔴
```
CPL: $9.18 USD 🔴
Leads: 1
Gasto: $9.18 USD (91.8% del presupuesto diario de $10.00)
Clicks: 31
Impresiones: 1,866
CTR: 1.66% 🔴
CPC: $0.30 USD
CPM: $4.92 USD
Alcance: 1,480
Status: ACTIVE
```

### 2. Pyme El Salvador (SV) — Segundo mejor CPL, también fuera de rango meta 🔴
```
CPL: $11.28 USD 🔴
Leads: 1
Gasto: $11.28 USD (90.2% del presupuesto diario de $12.50)
Clicks: 17
Impresiones: 1,776
CTR: 0.96% 🔴
CPC: $0.66 USD
CPM: $6.35 USD
Alcance: 1,378
Status: ACTIVE
```

### 3. Toma El control de tu pyme (GT) — Peor CPL individual del día 🔴
```
CPL: $14.02 USD 🔴
Leads: 1
Gasto: $14.02 USD (presupuesto a nivel ad set, N/D a nivel campaña)
Clicks: 29
Impresiones: 2,218
CTR: 1.31% 🔴
CPC: $0.48 USD
CPM: $6.32 USD
Alcance: 1,775
Status: ACTIVE
```

### 4. Odoo Test (GT) — Cero leads, rompe el cierre positivo del día anterior 🔴
```
CPL: N/A (0 leads) 🔴
Leads: 0
Gasto: $4.14 USD (84.0% del presupuesto diario de $4.93)
Clicks: 13
Impresiones: 668
CTR: 1.95%
CPC: $0.32 USD
CPM: $6.20 USD
Alcance: 571
Status: ACTIVE
```

### 5. Pyme Colombia (COL) — $0.00 de gasto, cero delivery todo el día ⚠️🔴
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
> [!warning] No es un problema de rendimiento, es un problema de programación
> Se investigó la causa: el ad set de esta campaña tiene `end_time = 2026-10-10T00:00:00-06:00` y `budget_remaining = $0.00` — es decir, el ad set **terminó su programación exactamente al inicio del día reportado** y agotó su presupuesto de por vida. La campaña sigue mostrando `effective_status: ACTIVE`, pero su delivery real es `completed`. Sin intervención (extender fecha de fin o aumentar presupuesto y reactivar), esta campaña no generará más leads.

### Campañas pausadas (sin gasto, $0.00) ⏸️
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 💡 Insights Clave

1. **El CPL blendeado sube +148.9% a $12.87, el peor cierre de la serie reciente**, revirtiendo con fuerza la mejora del 10-09 ($5.17). La causa principal es la caída de la conversión clic→lead, que pasa de 7.38% a **3.33%**, junto con una baja en leads totales (9 → 3, -66.7%).
2. **Pyme Colombia dejó de entregar por completo ($0.00 de gasto, 0 impresiones).** La investigación confirma que no es un problema de targeting, creativo o rechazo: el ad set de la campaña alcanzó su `end_time` programado exactamente a las 00:00 GT del 2026-10-10 y agotó su presupuesto de por vida (`budget_remaining: $0`). La campaña aparece como ACTIVE pero su delivery real es `completed`.
3. **Ninguna campaña con conversión superó 1 lead hoy.** Beco, Pyme El Salvador y Toma El control (GT) cerraron exactamente con 1 lead cada una — la primera vez en la serie reciente que ninguna campaña activa alcanza 2+ leads.
4. **Odoo Test vuelve a cero leads**, rompiendo el cierre positivo del 10-09 ($2.14 CPL, 2 leads) tras solo un día de conversión.
5. **La baja de -17.0% en gasto total no refleja optimización deliberada**: Beco y Pyme El Salvador mantienen ~90%+ de su presupuesto diario normal; la caída se explica casi en su totalidad por la pérdida de gasto de Pyme Colombia.

## ✅ Recomendaciones Accionables

- [ ] **Urgente — reactivar o renovar "Pyme Colombia"**: extender el `end_time` del ad set y/o asignar presupuesto nuevo; mientras no se haga, la campaña seguirá en $0.00 de gasto pese a aparecer ACTIVE.
- [ ] **Investigar por qué ninguna campaña superó 1 lead hoy** — evaluar fatiga de creativo o de audiencia en Beco, Pyme El Salvador y "Toma El control" (GT), las tres campañas que convirtieron.
- [ ] **Dar seguimiento a Odoo Test** para confirmar si el cierre en cero de hoy es puntual o retoma el patrón intermitente de días previos.
- [ ] **Confirmar si la caída de clic→lead (7.38% → 3.33%) es puntual** antes de mover presupuesto entre campañas.
- [ ] **Lanzar por fin el A/B testing de los 5 copys** documentado en [[CLAUDE.md]] (pendiente desde el 2026-08-24) para "Toma El control de tu pyme" (GT) — hoy registra además el peor CPL individual del día ($14.02).

## 🔗 Seguimiento

Ver registro del día en [[Daily notes/2026-10-10 - Resumen del Día]].

#daily-note #performance #meta-ads #octopus
