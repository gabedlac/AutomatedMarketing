---
date: 2026-11-17
aliases: [resumen-2026-11-17]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-17

> [!warning] Corrección de datos
> Esta nota reemplaza una versión anterior del mismo archivo, generada a las 05:53 UTC del propio 17-nov, que documentaba cifras **provisionales** porque el día aún no había cerrado en la zona horaria de la cuenta (`America/Guatemala`). Los datos de abajo fueron obtenidos y verificados hoy (18-nov) con `date_preset=yesterday` sobre `act_2530001557366648`, día ya cerrado. También se detectó que `Daily notes/2026-11-18 - Resumen del Dia.md` (generada por una rutina a las 05:54 UTC del 18-nov, antes de la medianoche de la cuenta) documenta en realidad este mismo 17-nov, no el 18-nov; se agregó una advertencia en ese archivo señalándolo.

---

## 📋 Resumen Ejecutivo del Día

La cuenta GT | Octopus Innovations tuvo un muy buen día el 17-nov: el gasto blendeado bajó a **$85.79** (-6.0% vs. el día anterior) y los leads subieron a **15** (+25%), el nivel más alto reportado hasta ahora en la bóveda. El CPL blendeado mejoró con fuerza a **$5.72** (-24.7%), cayendo por primera vez en varios días por debajo de la meta $6-7. El CTR, en cambio, empeoró a 1.67% (vs 2.16% el día anterior), alejándose más de la meta 3-4%. La historia del día es un cambio de roles: SLV | Odoo recuperó la cima como mejor campaña, mientras que GT | Odoo —la de mayor volumen y mejor campaña del día anterior— retrocedió con fuerza.

---

## 🔄 Cambios Principales vs. Día Anterior (2026-11-16)

| Métrica | 2026-11-17 | 2026-11-16 | Cambio |
|---|---|---|---|
| CPL blendeado | $5.72 | $7.60 | 🟢 -24.7% |
| Leads totales | 15 | 12 | 🟢 +25.0% |
| Gasto total | $85.79 | $91.25 | 🟢 -6.0% |
| CTR blendeado | 1.67% | 2.16% | 🔴 -0.49pp (empeora) |
| Impresiones | 11,882 | 11,887 | ➡️ -0.04% (estable) |
| Clicks | 198 | 257 | 🔴 -23.0% |

---

## 🚦 Status de Campañas (vs. día anterior)

| Campaña | Status |
|---|---|
| 🟢 SLV \| Odoo \| CP \| Servicios | **Arriba** — leads suben de 1 a 4 y el CPL cae de $8.41 a $2.20 (-74%), recupera la cima como mejor campaña de la cuenta. |
| 🟢 GT \| Beco \| CP \| Conjuntos | **Arriba** — leads suben de 1 a 2 y el CPL cae de $16.91 a $6.93 (-59%), vuelve a estar dentro de meta. |
| 🟢 COL \| Odoo \| CP \| Servicios | **Arriba** — rompe su racha en cero: de 0 a 2 leads, CPL $4.02. |
| 🟡 PY \| Odoo \| CP \| Servicios | **Mixto** — mismo 2 leads (vs 1 el día anterior; gasto similar), CPL mejora levemente a $4.48 desde $8.20. |
| 🔴 GT \| Odoo \| CP \| Servicios | **Abajo** — cae de 9 a 4 leads, CPL sube de $3.56 a $7.82 (+119.7%); pierde su condición de mejor campaña del día anterior. |
| 🔴 SLV \| Beco \| CP \| Conjuntos | **Mixto** — rompe su racha en cero con 1 lead (CPL $7.51), pero sigue fuera de meta. |
| 🔴 PY \| Beco \| CP \| Conjuntos | **Sin cambios** — segundo día consecutivo sin ningún lead, gasto estable (~$7.33). |
| ⚪ Evento: gestión de nómina (Odoo) | **Sin cambios** — sigue sin gasto ni impresiones (~5 días consecutivos). |

Resto de la cuenta (~11 campañas históricas): **PAUSED, sin cambios** (confirmado por `ads_account_get_activity_logs`: solo un evento automático de Meta, "Account billed" por $720.00 USD a las 7:39am del 17-nov, sin cambios manuales de presupuesto, targeting ni creativo).

---

## 📋 Próximas Acciones

- [ ] Revisar creativo/audiencia de PY | Beco — 2do día consecutivo sin leads, evaluar pausar si no mejora.
- [ ] Monitorear GT | Odoo tras su fuerte retroceso (9→4 leads, CPL +119.7%) — mayor volumen de la cuenta; vigilar fatiga de audiencia/creativo pese a que `ads_insights_anomaly_signal` no detectó anomalías.
- [ ] Confirmar si la mejora de SLV | Beco y GT | Beco (ambas rompiendo rachas negativas) es sostenida o ruido de un día.
- [ ] Investigar la caída de CTR blendeado (2.16%→1.67%) a pesar de la mejora en CPL/leads — revisar creativo y frecuencia.
- [ ] Verificar en Ads Manager por qué "Evento: gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas tras ~5 días, aunque sin errores de entrega — confirmar `start_time`, presupuesto o calendario.
- [ ] Pendiente heredado: decidir el futuro de las campañas históricas pausadas (Toma El control de tu pyme, Pyme Colombia, Pyme El Salvador, etc.) — reactivar, reemplazar formalmente o archivar.

---

## 🔗 Enlaces

- [[Reports/2026-11-17 - Reporte Performance]] — reporte completo de performance del día.
- [[Daily notes/2026-11-16 - Resumen del Dia]] — resumen del día anterior.

Tags: #daily-note #summary #meta-ads #octopus
