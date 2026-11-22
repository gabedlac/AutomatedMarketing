---
date: 2026-11-21
aliases: [resumen-2026-11-21]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-21

> [!info] Corrección de etiquetado (higiene de bóveda)
> Este archivo se generó originalmente por una rutina anterior que, debido a un desajuste de zona horaria (ejecución cerca de las ~05:52 UTC, antes del cierre del día local de la cuenta en `America/Guatemala`), documentaba bajo el nombre "2026-11-21" datos que en realidad correspondían al día **2026-11-20** (esos datos ya están preservados y finalizados en [[Reports/2026-11-20 - Reporte Performance]]). Esta rutina (ejecutada el 2026-11-22, con el día 21-nov ya cerrado y verificado) reemplaza ese contenido mal etiquetado con el resumen real y final del **2026-11-21**, para que el nombre del archivo coincida con los datos que contiene. No se pierde información: los datos del 20-nov permanecen disponibles en su reporte correspondiente.

---

## 📊 Resumen Ejecutivo del Día

Las 7 campañas activas de lead-gen generaron **13 leads** con **$81.56** de gasto → CPL blendeado **$6.27**, el primer día dentro de la meta ($6-7) del período registrado. Es también el mayor número de leads de un solo día documentado hasta ahora, casi duplicando los 7 leads del 20-nov (+85.7%), y con mejor diversificación: 4 campañas distintas aportaron leads (vs. 2 el día anterior). SLV \| Odoo ($1.86 CPL) y COL \| Odoo ($2.02 CPL) rompieron dos días consecutivos en cero y marcaron los mejores CPL individuales de la historia de la cuenta. El lado débil: **GT \| Odoo** sigue subiendo de CPL por tercer día consecutivo ($5.89 → $7.15 → $7.99) pese a mantener 4 leads, con el mayor gasto absoluto de la cuenta ($31.97).

Datos verificados y finales: `date_preset=yesterday` y un `time_range` explícito (`2026-11-21`) a nivel de campaña devolvieron cifras idénticas.

---

## 📈 Cambios Principales vs. Día Anterior (2026-11-20, final)

| Métrica | 2026-11-21 (final) | 2026-11-20 (final) | Cambio |
|---|---|---|---|
| CPL Promedio | **$6.27** | $12.10 | 🟢 -48.2% |
| Gasto Total | $81.56 | $84.68 | 🟢 -3.7% |
| Leads Totales | **13** | 7 | 🟢 +85.7% |
| CTR Promedio | 1.75% | 1.90% | 🔴 -7.9% |
| Impresiones | 11,120 | 10,976 | 🟢 +1.3% |
| Clicks | 195 | 208 | 🔴 -6.3% |
| Campañas sin ningún lead | 3 (PY Beco, PY Odoo, SLV Beco) | 5 (SLV Beco, COL Odoo, PY Odoo, SLV Odoo, PY Beco) | 🟢 Mejora (2 campañas recuperan leads) |
| Mejor campaña del día | SLV Odoo ($1.86 CPL, 4 leads — mejor histórico de la cuenta) | GT Beco ($4.85 CPL, 3 leads) | — |

---

## 🚦 Status de Campañas

| Campaña | Status | Tendencia |
|---|---|---|
| SLV \| Odoo \| CP \| Servicios | 🟢 Activa, convierte | ⬆️ Arriba — de 0 leads a $1.86 CPL (mejor histórico) |
| COL \| Odoo \| CP \| Servicios | 🟢 Activa, convierte | ⬆️ Arriba — de 0 leads a $2.02 CPL |
| GT \| Beco \| CP \| Conjuntos | 🟡 Activa, convierte pero empeora | ⬇️ Abajo — de $4.85 (mejor histórico) a $7.31 |
| GT \| Odoo \| CP \| Servicios | 🟡 Activa, convierte pero empeora | ⬇️ Abajo — CPL sube 3er día consecutivo ($7.15 → $7.99) |
| PY \| Beco \| CP \| Conjuntos | 🔴 Activa, sin leads | ➡️ Estable — 3er día consecutivo en cero |
| PY \| Odoo \| CP \| Servicios | 🔴 Activa, sin leads | ➡️ Estable — 3er día consecutivo en cero |
| SLV \| Beco \| CP \| Conjuntos | 🔴 Activa, sin leads | ➡️ Estable — 3er día consecutivo en cero |
| Evento: El futuro de la gestión de nómina (Odoo) | ⚪ Activa, sin actividad | ➡️ Estable — ~12º día sin gasto ni impresiones |
| ~14 campañas históricas | ⏸️ Pausadas | ➡️ Sin cambios |

Sin cambios de configuración (presupuesto, targeting, creativo) registrados en `ads_account_get_activity_logs` para el rango 2026-11-21 06:00–2026-11-22 06:00 UTC. `ads_insights_anomaly_signal` no detectó anomalías (solapamiento de subasta, fatiga de creativo, audiencia estrecha).

---

## 🔗 Enlaces

- [[Reports/2026-11-21 - Reporte Performance]] — reporte completo y detallado de este día (análisis, insights y recomendaciones).
- [[Daily notes/2026-11-22 - Resumen del Dia]] — nota que documentaba (bajo ese nombre de archivo) los datos provisionales de este mismo día 21-nov, ahora confirmados como finales en el reporte enlazado arriba.
- [[Reports/2026-11-20 - Reporte Performance]] — reporte del día anterior, usado como base de comparación.

---

## 📋 Próximas Acciones

- [ ] Revisar por qué el CPL de **GT \| Odoo** sube por tercer día consecutivo pese a mantener 4 leads — evaluar pausar el escalado de presupuesto hasta estabilizar el CPL.
- [ ] Confirmar si **PY \| Beco, PY \| Odoo y SLV \| Beco** comparten un factor común distinto al de SLV \| Odoo y COL \| Odoo, que sí recuperaron leads.
- [ ] Confirmar si la recuperación de SLV \| Odoo y COL \| Odoo se sostiene antes de reasignar presupuesto hacia ellas.
- [ ] Verificar en Ads Manager por qué la campaña de evento sigue sin reportar actividad (~12 días).
- [ ] Seguir trabajando el CTR blendeado (1.75% vs meta 3-4%) con pruebas A/B de creativo.

#daily-note #summary #meta-ads #octopus
