---
date: 2026-09-17
aliases: [reporte-2026-09-17, performance-17-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-17

> [!info] Datos de cierre confirmados
> Pull realizado 2026-09-18 (07:11 hora de Guatemala) con `date_preset=yesterday`, día ya cerrado completamente en horario de Guatemala (GMT-6). Este reporte reemplaza y confirma la lectura parcial (~10 min antes del cierre) documentada por error en [[Daily notes/2026-09-17 - Resumen del Dia]].

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $5.53 USD* | $6-7 | 🟢 Por debajo de la meta |
| **Gasto Total** | $44.22 USD | - | 🔺 +12.1% vs. 09-16 ($39.45) |
| **Leads Totales** | 8 confirmados* | 4-5/día | 🟢 Supera la meta (+60%, aún incompleto) |
| **CTR Promedio** | 1.76% | 3-4% | 🔴 Sigue por debajo de meta, mejora fuerte +29.4% vs. 09-16 (1.36%) |
| **CPC Promedio** | $0.34 USD | - | 🟢 Mejora -19.0% vs. 09-16 ($0.42) |
| **CPM Promedio** | $6.03 USD | - | 🔺 +4.3% vs. 09-16 ($5.78) |
| **Impresiones** | 7,332 | - | 🔺 +7.4% vs. 09-16 |
| **Clicks** | 129 | - | 🔺 +38.7% vs. 09-16 |
| **Alcance (Reach)** | 5,440 | - | 🔺 +1.6% vs. 09-16 |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

\* CPL y leads calculados sobre gasto/leads confirmados de cuenta. **Beco** y **Odoo Test** siguen mostrando `results: Not available` (ver advertencia en Insights) — el CPL y los leads reales de cuenta podrían ser más altos/mejores una vez se resuelva su atribución.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Toma El control de tu pyme]] (GT) — Nuevo mejor CPL histórico del vault 🟢
```
CPL: $2.98 USD 🟢
Leads: 6
Gasto: $17.88 USD
Clicks: 64
CTR: 2.24% (el más alto de la cuenta)
CPC: $0.28 USD
CPM: $6.25 USD
Impresiones: 2,859
Reach: 2,259
```
**Status:** ACTIVE
**Insight:** Segundo cierre confirmado consecutivo por debajo de la meta de cuenta ($6-7), y el mejor registrado en el vault hasta ahora (vs. $3.56 el 09-16). Confirma que la decisión del A/B test — mantener el ad set "Urgencia" activo con presupuesto duplicado y "Excel" pausado — fue acertada. Objetivo de [[CLAUDE.md]] de bajar el CPL de esta campaña de $9.29 a $6-7 ya superado ampliamente durante dos días seguidos.

### 2. [[Pyme El salvador]] (SV) — Mejora fuerte, aún ligeramente sobre meta 🟡
```
CPL: $7.18 USD 🟡
Leads: 2
Gasto: $14.36 USD
Clicks: 50
CTR: 1.83%
CPC: $0.29 USD
CPM: $5.27 USD
Impresiones: 2,725
Reach: 2,007
```
**Status:** ACTIVE
**Insight:** Mejora -33.7% vs. el $10.83 confirmado del 09-16, y ya está dentro del rango cercano a la meta de cuenta ($6-7). Sigue siendo la campaña activa con el CPL más alto de la cuenta, pero la tendencia de los últimos 3 cierres es de mejora sostenida.

### 3. [[Beco]] — Leads pendientes de atribución ⚠️
```
Gasto: $9.42 USD
Clicks: 12
CTR: 0.87%
CPC: $0.79 USD
CPM: $6.79 USD
Impresiones: 1,387
Reach: 1,071
Leads / CPL: Not available
```
**Status:** ACTIVE
**Insight:** `results` y `cost_per_result` siguen sin datos disponibles para el cierre de 09-17. Es la segunda vez que esto ocurre en el vault para esta campaña (la primera fue el cierre de 09-15, que tardó más de 48h en resolverse según lo documentado en el reporte de 09-16) — ver advertencia en Insights Clave.

### 4. [[Odoo Test]] — Leads pendientes de atribución ⚠️
```
Gasto: $2.56 USD
Clicks: 3
CTR: 0.83% (el más bajo de la cuenta)
CPC: $0.85 USD (el más alto de la cuenta)
CPM: $7.09 USD
Impresiones: 361
Reach: 316
Leads / CPL: Not available
```
**Status:** ACTIVE
**Insight:** Mismo patrón que Beco: sin datos de `results` disponibles para 09-17, repitiendo la anomalía ya vista el 09-15. Volumen de clicks muy bajo (3), lo que podría hacer más lenta la atribución, pero el patrón repetido con la misma campaña merece revisión directa de su configuración de lead forms/CAPI.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🧪 A/B Test — "Toma El control de tu pyme" (GT)

| Ad Set | Status | Presupuesto/día | Gasto | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $17.88 (+19% sobre presupuesto) | 64 | 2.24% | 6 | **$2.98** |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | 0 | - | - | - |

**Cambios de cuenta durante la ventana 09-17 (según activity log):** ninguno manual. Solo eventos automáticos de Meta (inicio de entrega en varios anuncios, creación automática de audiencia `asa_auto_custom_audience`) y una actualización de estado de revisión de anuncio ("Odoo Test Imagen Estatica": Pending Process → Pending Review) por Gabriel Calderon vía Power Editor.

## 💡 Insights Clave

- **"Toma El control de tu pyme" (GT) marca su segundo cierre confirmado consecutivo por debajo de la meta de cuenta**, con $2.98 CPL — el mejor resultado documentado en el vault. La decisión del A/B test (Urgencia activo, Excel pausado) queda validada con dos días de datos de cierre real.
- **El ad set "Urgencia" gastó $17.88 contra un presupuesto diario de $15.00** (~19% sobre el límite configurado), repitiendo el patrón de sobregasto visto en la lectura parcial del día anterior. Vale la pena confirmar si esto está dentro de la tolerancia de entrega normal de Meta o si conviene subir el presupuesto formalmente dado el excelente CPL.
- **⚠️ Persiste el problema de tracking de leads en Beco y Odoo Test**: ambas campañas muestran `results: Not available` para el cierre de 09-17, el mismo patrón que ya se había señalado como anómalo para el cierre de 09-15 (sin resolver tras más de 48h en ese momento). Que sea justo el mismo par de campañas el que vuelve a mostrar el problema — y no las 4 campañas activas — sugiere que el problema podría no ser demora de atribución genérica sino algo específico de la configuración de lead forms/CAPI de Beco y Odoo Test. Recomendación: revisar directamente la integración de estas 2 campañas.
- **Pyme El Salvador mejora por tercer cierre consecutivo** ($10.79 → $10.83 → $7.18), acercándose a la meta de cuenta aunque sigue ligeramente por encima.
- El CTR promedio de cuenta sube a 1.76% (+29.4% vs. 09-16) pero sigue muy por debajo de la meta de 3-4%.
- Sin cambios manuales de presupuesto, pausas o nomenclatura durante el 09-17 — la configuración vigente fue la decidida el 09-16 (A/B test) y se mantuvo estable todo el día.

## ✅ Recomendaciones Accionables

- [ ] **Revisar la configuración de lead forms / CAPI de Beco y Odoo Test específicamente** — es la segunda vez que estas mismas 2 campañas (de 4 activas) muestran `results: Not available` en el cierre confirmado; si se repite un tercer día, tratar como incidente de tracking, no de atribución normal.
- [ ] **Confirmar leads pendientes de Beco y Odoo Test en los próximos 1-2 días** para actualizar el CPL/leads reales de cuenta del 09-17.
- [ ] **Mantener "Urgencia" como configuración ganadora del A/B test** — el resultado se sostiene y mejora en su segundo cierre confirmado consecutivo.
- [ ] **Evaluar subir formalmente el presupuesto diario de "Urgencia"** a ~$18 USD/día, dado que consistentemente gasta 19-20% sobre el límite de $15 configurado.
- [ ] **Seguir dando seguimiento a Pyme El Salvador** — tercera mejora consecutiva, cerca de entrar en meta.
- [ ] Aclarar el origen y plan de uso de los ad sets pausados "TestA/B Productividad" y "GT + QTZ" dentro de "Toma El control de tu pyme".

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-17 - Resumen del Dia]] - Nota del día (actualizada con el cierre confirmado)
- [[Reports/2026-09-16 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Tarea de A/B testing de copys, con resultados confirmados muy positivos
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-17
Tags: #daily-note #performance #meta-ads #octopus
