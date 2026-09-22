---
date: 2026-09-21
aliases: [reporte-2026-09-21, performance-21-sep]
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-09-21

> [!info] Datos de cierre confirmados
> Pull realizado 2026-09-22 con `date_preset=yesterday`, día ya cerrado completamente en horario de Guatemala (GMT-6). Este reporte reemplaza y confirma la lectura casi-final (~9 min antes del cierre) documentada en [[Daily notes/2026-09-21 - Resumen del Dia]].

## 📋 Resumen Ejecutivo

| Métrica | Valor | Meta | Status |
|---------|-------|------|--------|
| **CPL Promedio** | $8.49 USD | $6-7 | 🔴 Por encima de la meta (+21-41%) |
| **Gasto Total** | $42.43 USD | - | 🔻 -19.1% vs. 09-20 ($52.47) |
| **Leads Totales** | 5 | 4-5/día | 🟢 En el límite inferior de la meta |
| **CTR Promedio** | 1.49% | 3-4% | 🔴 Por debajo de meta, retrocede -10.8% vs. 09-20 (1.67%) |
| **CPC Promedio** | $0.39 USD | - | 🔻 +14.7% vs. 09-20 ($0.34) |
| **CPM Promedio** | $5.75 USD | - | 🔻 +2.1% vs. 09-20 ($5.63) |
| **Impresiones** | 7,385 | - | 🔻 -20.7% vs. 09-20 |
| **Clicks** | 110 | - | 🔻 -29.5% vs. 09-20 |
| **Alcance (Reach)** | 5,844 | - | 🔻 -20.4% vs. 09-20 |
| **ROAS** | No aplica | - | Campañas Lead Gen sin tracking de valor de conversión |

**Nota:** Las 4 campañas activas históricas caen a la mitad de leads (10 → 5) con menos gasto (-19.1%), lo que empuja el CPL promedio por encima de la meta de $6-7 por primera vez desde el 09-18. Pyme Colombia, lanzada anoche, no registra gasto confirmado en la ventana del 09-21 (ver insight abajo).

## 🎯 Performance por Campaña (Ranked por CPL)

### 1. [[Odoo Test]] (GT) — Mejor CPL de la cuenta hoy 🟢
```
CPL: $4.00 USD 🟢
Leads: 1
Gasto: $4.00 USD
Clicks: 12
CTR: 2.39%
CPC: $0.33 USD
CPM: $7.95 USD
Impresiones: 503
Reach: 384
```
**Status:** ACTIVE
**Insight:** Baja de $6.41 (09-20) a $4.00, el mejor CPL de la cuenta hoy, aunque sobre una muestra muy pequeña (1 lead / 12 clicks) que sigue moviéndose fuerte día a día.

### 2. [[Pyme El salvador]] (SV) — Dentro de meta, pierde el liderazgo de eficiencia 🟢
```
CPL: $6.13 USD 🟢
Leads: 2
Gasto: $12.25 USD
Clicks: 33
CTR: 1.47%
CPC: $0.37 USD
CPM: $5.47 USD
Impresiones: 2,239
Reach: 1,700
```
**Status:** ACTIVE
**Insight:** Sube de $3.94 (09-20) a $6.13 (+55.6%), su primer cierre fuera del mejor puesto de la cuenta en varios días, pero se mantiene justo dentro de la meta de $6-7. El gasto baja -22.2% y los leads caen de 4 a 2, señal de menor volumen más que de una pérdida de eficiencia aislada.

### 3. [[Beco]] (GT) — Repite peor patrón, fuera de meta 🔴
```
CPL: $10.49 USD 🔴
Leads: 1
Gasto: $10.49 USD
Clicks: 23
CTR: 1.25%
CPC: $0.46 USD
CPM: $5.70 USD
Impresiones: 1,841
Reach: 1,495
```
**Status:** ACTIVE
**Insight:** Sube ligeramente de $9.99 (09-20) a $10.49, confirmando atribución de leads por tercera vez en los últimos 7 cierres, siempre con 1 solo lead y siempre fuera de la meta de $6-7. El patrón intermitente de atribución sigue sin resolverse.

### 4. [[Toma El control de tu pyme]] (GT) — Peor CPL de la cuenta, fuera de meta 🔴
```
CPL: $15.69 USD 🔴
Leads: 1
Gasto: $15.69 USD
Clicks: 42
CTR: 1.50%
CPC: $0.37 USD
CPM: $5.60 USD
Impresiones: 2,802
Reach: 2,265
```
**Status:** ACTIVE
**Insight:** Salta de $5.08 (09-20) a $15.69 (+208.9%), su peor cierre confirmado del período reciente ($2.43–$9.91 en los 6 cierres previos). El volumen de clicks (42) baja frente a los ~57-58 de días anteriores, así que el salto de CPL combina menos tráfico con una conversión click→lead mucho más débil (solo 1 lead sobre 42 clicks).

### 5. [[Pyme Colombia]] (COL) — Campaña nueva, sin gasto confirmado en la ventana del 09-21 🆕
```
CPL: N/D
Leads: N/D
Gasto confirmado: $0.00 USD
Clicks: 0
Impresiones: 0
```
**Status:** ACTIVE (lanzada 09-21 ~22:59 PM hora Guatemala)
**Insight:** La nota casi-final de anoche estimó ~$7.19 gastados en la primera hora, basado en una lectura de `budget_remaining` tomada minutos después del lanzamiento. La API confirma ahora **$0.00 de gasto atribuido al día calendario 09-21** — la campaña arrancó a las 22:59 PM GT y su actividad medible (impresiones/clicks) no llegó a acumularse antes del corte de medianoche. El gasto real ya se está acumulando en el día 09-22 (verificado: $2.90 de $7.50 gastados a media mañana de hoy). Tratar la estimación de anoche como no confiable; el primer cierre real de Colombia se confirmará en el reporte de mañana (09-22).

### Campañas sin actividad (PAUSED, $0 gasto)
- Toma El control de tu pyme (USA)
- Accurate Partners - Loyalti - Nuevas Obligaciones - JUN 2026
- Conversión Clientes Potenciales - MX
- Conversión Clientes Potenciales - PY
- 🟡 CONVERSIÓN - CLIENTES POTENCIALES

## 🧪 A/B Test — "Toma El control de tu pyme" (GT)

| Ad Set | Status | Presupuesto/día | Gasto | Clicks | CTR | Leads | CPL |
|--------|--------|------------------|-------|--------|-----|-------|-----|
| TestA/B Urgencia | ACTIVE 🟢 | $15.00 | $15.69 (104.6% del presupuesto) | 42 | 1.50% | 1 | $15.69 |
| TestA/B Excel | PAUSED ⏸️ | $7.50 | $0.00 | 0 | - | - | - |
| TestA/B Productividad | PAUSED ⏸️ | $5.00 | $0.00 | 0 | - | - | - |
| GT + QTZ | PAUSED ⏸️ | $20.00 | $0.00 | 0 | - | - | - |

**Nota:** El sobregasto de "Urgencia" se reduce drásticamente vs. los cierres anteriores (135.5% el 09-20, 134.8% el 09-19-casi-final) a solo 104.6% hoy — el más cercano al presupuesto exacto documentado en el período reciente. A la vez, el volumen de clicks cae de 58 a 42 (-27.6%) y solo se registró 1 lead, el peor resultado de conversión de "Urgencia" en varios cierres.

## 🌎 Nueva Campaña — Pyme Colombia

- Creada y activada manualmente por Gabriel Calderon vía Power Editor el 09-21 entre 22:45 PM y 23:02 PM (hora Guatemala): 3 imágenes nuevas subidas, campaña `[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia` creada con objetivo Leads, presupuesto corregido de $12.50/día a $7.50/día, ad set con targeting Medellín/Bogotá (28-50 años, decision makers de pyme) y Advantage+ audience activado.
- Confirmado hoy: sin gasto atribuido al 09-21; el ritmo de gasto real comienza a verse en el día 09-22 ($2.90 de $7.50 a media mañana). Se dará seguimiento a su primer cierre completo en el reporte de mañana.

## 💡 Insights Clave

- **El CPL promedio de cuenta sube a $8.49 (+61.7% vs. 09-20) y queda por primera vez desde el 09-18 fuera de la meta de $6-7**, impulsado por una caída de leads a la mitad (10 → 5) que no viene acompañada de una caída proporcional de gasto (-19.1%).
- **"Toma El control de tu pyme" (GT) registra su peor cierre confirmado del período reciente** ($15.69, +208.9% vs. 09-20), rompiendo el rango de volatilidad habitual ($2.43-$9.91) por primera vez hacia arriba. El volumen de clicks también cae, así que el problema no es solo de conversión sino también de tráfico.
- **El sobregasto de "Urgencia" se normaliza a 104.6% del presupuesto**, su lectura más cercana al límite exacto en el período reciente, aunque coincide con su peor resultado de conversión (1 lead sobre 42 clicks).
- **Beco confirma atribución por tercera vez en 7 cierres, siempre fuera de meta** ($10.49 hoy) — el patrón de "1 lead a CPL alto" cuando sí reporta datos se mantiene consistente; sigue ameritando tratamiento como problema recurrente de tracking.
- **Pyme El Salvador pierde el liderazgo de eficiencia de la cuenta por primera vez en varios días**, aunque se mantiene justo dentro de la meta ($6.13); Odoo Test toma el mejor puesto con $4.00 sobre un volumen muy bajo.
- **La estimación de gasto de Pyme Colombia de la nota casi-final de anoche (~$7.19) no se confirma**: el cierre real del 09-21 registra $0.00, y el gasto verificado ya está corriendo en el día 09-22. Tratar las lecturas casi-finales de campañas recién lanzadas con cautela adicional hasta su primer cierre completo.
- **El CTR de cuenta retrocede a 1.49% (-10.8% vs. 09-20)**, alejándose más de la meta de 3-4% y marcando su segundo retroceso consecutivo.

## ✅ Recomendaciones Accionables

- [ ] **Investigar la caída de conversión en "Toma El control" (GT)**: 1 solo lead sobre 42 clicks es la peor tasa de conversión click→lead documentada para esta campaña en el período reciente — revisar el copy/landing del ad set "Urgencia" antes de escalar presupuesto de nuevo.
- [ ] **Confirmar el primer cierre completo de Pyme Colombia mañana (09-22)** y descartar la estimación de gasto de anoche, que no se sostuvo con datos de cierre.
- [ ] **Escalar formalmente el problema de atribución intermitente de Beco** como posible falla de tracking/pixel — tercera confirmación en 7 cierres, siempre con 1 lead y siempre fuera de meta.
- [ ] Dar seguimiento a si Pyme El Salvador retoma su rango de mejor eficiencia de la cuenta o si $6.13 se convierte en su nuevo nivel base.
- [ ] Seguir sin resolver: aclarar el origen y plan de uso de los ad sets pausados "TestA/B Productividad", "TestA/B Excel" y "GT + QTZ".

## 🔗 Enlaces Relacionados

- [[Daily notes/2026-09-21 - Resumen del Dia]] - Nota del día (actualizada con el cierre confirmado)
- [[Reports/2026-09-20 - Reporte Performance]] - Reporte del día anterior
- [[CLAUDE.md]] - Tarea de A/B testing de copys; caída de conversión en "Toma El control" y primer cierre de Pyme Colombia a seguir confirmando
- [[cloud.md]] - Dashboard principal

---
Generado por: Claude Code (Reporte Automatizado) + Meta Ads API
Cuenta: GT | Octopus Innovations (2530001557366648)
Fecha: 2026-09-21
Tags: #daily-note #performance #meta-ads #octopus
