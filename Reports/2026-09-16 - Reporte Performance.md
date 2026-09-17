---
date: 2026-09-16
aliases: [reporte-2026-09-16, performance-16-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-16

> [!info] Datos de cierre confirmados
> Pull realizado 2026-09-17 con `date_preset=yesterday`, día ya cerrado completamente en horario de Guatemala (GMT-6). Las 4 campañas activas muestran leads confirmados — a diferencia del cierre anterior (09-15), que seguía con 3 de 4 campañas pendientes de atribución al momento de su reporte.

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $4.93 USD | $6-7 | 🟢 Por debajo de la meta — mejor cierre en semanas |
| **Gasto Total** | $39.45 USD | - | 🔻 -9.2% vs. 09-15 ($43.47*) |
| **Leads Totales** | 8 | 4-5/día | 🟢 Supera la meta (+60%) |
| **CTR Promedio** | 1.36% | 3-4% | 🔴 Sigue por debajo de meta, mejora +13% vs. 09-15 (1.20%*) |
| **CPC Promedio** | $0.42 USD | - | 🟢 Estable/leve mejora |
| **CPM Promedio** | $5.78 USD | - | 🟢 Leve mejora vs. 09-15 |
| **Impresiones** | 6,829 | - | 🔻 -6.9% vs. 09-15 |
| **Clicks** | 93 | - | 🟢 +5.7% vs. 09-15 |
| **Alcance (Reach)** | 5,356 | - | 🔻 -8.9% vs. 09-15 |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

\* Cifras de 09-15 son parciales: 3 de 4 campañas activas siguen mostrando `results: Not available` incluso en este pull (2 días después de su cierre) — ver advertencia en Insights.

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Toma El control de tu pyme]] (GT) — Mejor CPL de la cuenta 🟢
```
CPL: $3.56 USD 🟢
Leads: 4
Gasto: $14.24 USD
Clicks: 36
CTR: 1.80%
CPC: $0.40 USD
CPM: $7.11 USD
Impresiones: 2,003
Reach: 1,550
```
**Status:** ACTIVE
**Insight:** Cae a $3.56 CPL, el mejor cierre confirmado en semanas y muy por debajo de la meta ($6-7), tras la volatilidad reciente ($8.32 el 09-15, $5.36 el 09-14). Leads suben a 4, el volumen más alto documentado para esta campaña. Coincide con el inicio del A/B test de copys pendiente desde 2026-08-24 (ver Cambios de Cuenta abajo) — aunque el test se activó en los últimos ~15 minutos del día, así que este resultado refleja mayormente el copy y setup previos al test, no su efecto.

### 2. [[Beco]] (antes "Beco GT" — renombrada el 09-16)
```
CPL: $4.79 USD 🟢
Leads: 2
Gasto: $9.57 USD
Clicks: 26
CTR: 1.24%
CPC: $0.37 USD
CPM: $4.56 USD
Impresiones: 2,097
Reach: 1,664
```
**Status:** ACTIVE
**Insight:** Cierra con 2 leads confirmados a $4.79, por debajo de la meta. Recupera actividad de leads tras cerrar en 0 el 09-14; su cierre de 09-15 sigue sin dato disponible (ver advertencia).

### 3. [[Odoo Test]]
```
CPL: $4.81 USD 🟢
Leads: 1
Gasto: $4.81 USD
Clicks: 16
CTR: 1.87% (el más alto de la cuenta)
CPC: $0.30 USD
CPM: $5.62 USD
Impresiones: 856
Reach: 668
```
**Status:** ACTIVE
**Insight:** CTR más alto de la cuenta (1.87%), CPL saludable por debajo de meta. Campaña de bajo volumen pero consistente.

### 4. [[Pyme El salvador]] (SV) — Única campaña sobre meta 🔴
```
CPL: $10.83 USD 🔴
Leads: 1
Gasto: $10.83 USD
Clicks: 15
CTR: 0.80% (el más bajo de la cuenta)
CPC: $0.72 USD (el más alto de la cuenta)
CPM: $5.78 USD
Impresiones: 1,873
Reach: 1,474
```
**Status:** ACTIVE
**Insight:** Único CPL sobre la meta $6-7 y el CTR más bajo de la cuenta por segundo día consecutivo (0.78% el 09-15, 0.80% hoy). Candidata prioritaria a revisión de copy/creativo — patrón similar al problema histórico que motivó el rediseño de copys de "Toma El control de tu pyme" en 08-24.

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 💡 Insights Clave

- **CPL de cuenta baja a $4.93, dentro/mejor que la meta ($6-7) por primera vez en varios cierres**, con 8 leads totales — 60% por encima de la meta de 4-5/día. Es el mejor cierre confirmado desde que se documenta en este vault.
- **⚠️ Posible problema de tracking de leads en 3 de 4 campañas para el cierre de 2026-09-15**: al re-consultar hoy (09-17, ~2 días después de ese cierre) para calcular la comparación día a día, Odoo Test, Beco y Pyme El Salvador **siguen mostrando `results: Not available`** para 09-15, mientras que sus datos de gasto/clicks/impresiones sí están cerrados. Esto ya se había señalado como anómalo en el reporte de 09-15 (a solo ~13h del cierre) y **no se ha resuelto tras ~2 días**, superando el umbral de 24-48h que ese mismo reporte marcó como punto de escalación. Recomendación: verificar la integración de formularios de lead / CAPI para estas 3 campañas — ya no parece demora normal de atribución.
- **"Toma El control de tu pyme" (GT) lidera con $3.56 CPL y 4 leads**, su mejor cierre documentado, justo el día en que se decidió duplicar presupuesto al ad set "TestA/B Urgencia" y pausar "TestA/B Excel" (cambio aplicado ~15 min antes de medianoche, por lo que su efecto se verá reflejado recién en el cierre de 09-17).
- **"Pyme El Salvador" es la única campaña activa por encima de la meta de CPL** y tiene el CTR más bajo de la cuenta dos días seguidos — necesita atención de copy/creativo similar a la que recibió "Toma El control" en agosto.
- El CTR promedio de cuenta mejora a 1.36% (+13% vs. 09-15) pero sigue muy por debajo de la meta de 3-4%.
- **Cambios de nomenclatura aplicados el 09-16** (11:45 PM GT, por Gabriel Calderon): "Beco GT" → "Beco"; "Pyme El salvador" corrigió su etiqueta de [GT] a [SV] (la campaña es para El Salvador).
- **A/B test de copys iniciado** (pendiente desde 2026-08-24 según [[CLAUDE.md]]): dentro de "Toma El control de tu pyme", el ad set "TestA/B Urgencia" recibió presupuesto duplicado ($7.50 → $15.00/día) y "TestA/B Excel" fue pausado, ambos cambios a las 11:47 PM GT del 09-16.

## ✅ Recomendaciones Accionables

- [ ] **Investigar el tracking de leads de Odoo Test, Beco y Pyme El Salvador para el cierre de 2026-09-15** — sigue sin datos ~2 días después, superando el umbral de escalación ya señalado en el reporte anterior. Revisar la integración de formularios de lead / CAPI antes de asumir demora normal de atribución.
- [ ] **Confirmar si duplicar presupuesto en "TestA/B Urgencia" y pausar "TestA/B Excel" fue la decisión correcta** — dar seguimiento 3-5 días, dado que la lectura parcial previa a la decisión mostraba a Excel con mejor CTR y CPL.
- [ ] **Priorizar revisión de copy/creativo para "Pyme El Salvador"** — único CPL sobre meta y CTR más bajo de la cuenta por segundo día consecutivo.
- [ ] **Mantener el monitoreo diario del CPL de "Toma El control de tu pyme"** tras este cierre de $3.56 — tiene historial de alta volatilidad día a día.
- [ ] **Seguir trabajando el CTR promedio de cuenta**, que aunque mejora sigue muy por debajo de la meta de 3-4%.
- [ ] Documentar en [[campaigns/Adjustments]] el resultado del A/B test una vez haya 3-5 días de datos con el nuevo split de presupuesto.

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-16 - Resumen del Dia]] - Nota del día
- [[Reports/2026-09-15 - Reporte Performance]] - Reporte del día anterior
- [[campaigns/Adjustments/2026-09-17 - Guatemala & El Salvador Updates]] - Detalle de los cambios de cuenta del 09-16
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-16
Tags: #daily-note #performance #meta-ads #octopus
