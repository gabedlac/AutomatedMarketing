---
date: 2026-11-09
aliases: [resumen-2026-11-09]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-09

> [!success] Conector Meta Ads restablecido — se actualiza este resumen con datos reales
> Esta nota se regenera el 2026-11-10 (13:10 UTC) desde la rutina "Daily Meta Ads Performance Report - 7 AM Guatemala", que esta vez sí tuvo acceso a `ads_get_ad_entities`. **Reemplaza la versión anterior de este archivo**, que había sido creada por la rutina nocturna separada documentando el bloqueo de conector (`needs_reconnect`) como decimoctavo día consecutivo sin datos. Con el conector funcionando, se recuperan las métricas reales del 2026-11-09 y se cierra la racha de 19 días sin visibilidad (10-23 a 11-10). Ver el detalle completo en [[Reports/2026-11-09 - Reporte Performance]].

---

## 🎯 Campañas Revisadas

7 campañas de lead-gen activas (más 1 de evento, no lead-gen). La cuenta ya no gira sobre la campaña única que documenta [[CLAUDE.md]] — esa campaña ("Toma El control de tu pyme" GT) está **PAUSED**, junto con todo el resto de campañas legacy.

| Campaña | Status | Gasto | Leads | CPL |
|---|---|---|---|---|
| GT \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $32.44 | 8 | $4.06 |
| GT \| Beco \| CP \| Conjuntos | 🟢 ACTIVE | $11.85 | 3 | $3.95 |
| PY \| Odoo \| CP \| Servicios | 🟢 ACTIVE | $8.50 | 3 | $2.83 |
| COL \| Odoo \| CP \| Servicios | 🟡 ACTIVE | $8.19 | 1 | $8.19 |
| SLV \| Odoo \| CP \| Servicios | 🟡 ACTIVE | $7.54 | 1 | $7.54 |
| PY \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $7.10 | 0 | — |
| SLV \| Beco \| CP \| Conjuntos | 🔴 ACTIVE | $6.85 | 0 | — |
| Evento: gestión de nómina (Odoo) | ⚪ ACTIVE (EVENT_RESPONSES) | $4.08 | n/a | n/a |

Resto de campañas (Toma El control GT/USA, Beco original, Pyme El Salvador/Colombia legacy, Odoo Test, Accurate Partners, Conversión Clientes Potenciales, boosts de evento anteriores): **PAUSED**, sin cambios.

---

## 📊 Análisis e Insights

- **El conector volvió a dar datos reales** después de 19 días calendario de bloqueo — se recupera visibilidad sobre la cuenta a partir de hoy.
- **CPL blendeado (7 campañas lead-gen): $5.15**, dentro/mejor que la meta histórica de $6-7.
- **CTR blendeado: 1.24%**, lejos de la meta de 3-4% — mismo problema de creativo que ya diagnosticaba [[CLAUDE.md]] en agosto, ahora visible en la estructura nueva de cuenta.
- **16 leads totales** repartidos en 5 de las 7 campañas; GT Odoo sigue siendo el motor principal (8 leads, 50% del total).
- **Alerta:** PY Beco y SLV Beco pasaron a 0 leads hoy pese a seguir gastando (~$7 cada una) — revisar creativo/audiencia antes de escalar presupuesto en esas dos.
- La estructura de cuenta cambió por completo frente a lo que documenta [[CLAUDE.md]] (una sola campaña GT); las tareas pendientes de A/B testing de los 5 copys probablemente necesitan reencuadrarse a las campañas activas actuales.

---

## ✏️ Cambios Realizados

Ninguno ejecutado desde esta rutina — es un reporte de solo lectura. No se modificó presupuesto, targeting ni creativo de ninguna campaña.

---

## 🔬 Investigación Realizada

- Se obtuvieron métricas reales vía `ads_get_ad_entities` (nivel campaña) para `act_2530001557366648`, rango `2026-11-09` y `2026-11-08` (comparación día anterior).
- Se confirmó el estado PAUSED de la campaña histórica de [[CLAUDE.md]] y de todo el resto de campañas legacy.
- Se corrigió el estado de git: la sesión inició en *detached HEAD* sobre `origin/main` (3 commits por delante de la rama local `main`); se hizo `git checkout -B main origin/main` para volver a trabajar sobre una rama real antes de este commit.

---

## 📊 Datos Clave del Día (comparación vs 2026-11-08)

| Métrica (blendeada, lead-gen) | 2026-11-08 | 2026-11-09 | Cambio |
|---|---|---|---|
| Gasto total | $104.38 | $82.47 | 🔽 -21% |
| Leads totales | 16 | 16 | ➡️ Igual |
| CPL blendeado | $6.52 | $5.15 | 🟢 Mejora -21% |
| Impresiones | 15,457 | 14,272 | 🔽 -7.7% |
| Clicks | 215 | 177 | 🔽 -17.7% |
| CTR blendeado | 1.39% | 1.24% | 🔴 -0.15pp |

**Por campaña, 11-08 → 11-09:** PY Odoo (0→3 leads, mejora fuerte), COL Odoo (0→1) y SLV Odoo (0→1) mejoran; GT Odoo estable (8→8); GT Beco mejora eficiencia (gasto -42%, CPL $5.07→$3.95) con solo 1 lead menos; **PY Beco (3→0) y SLV Beco (1→0) retroceden a cero leads** — foco de atención para mañana.

---

## 📋 Próximas Acciones

- [ ] Revisar creativo/audiencia de PY Beco y SLV Beco (0 leads el 11-09 pese a ~$7 de gasto cada una).
- [ ] Extender el diagnóstico de CTR bajo de [[CLAUDE.md]] (copys sin urgencia) a las 7 campañas activas actuales; el síntoma persiste con la estructura nueva de cuenta.
- [ ] Confirmar con el usuario si el A/B testing de los 5 copys (pendiente desde 2026-08-24) se reencuadra a GT Odoo/Beco o se cierra, dado que la campaña original está PAUSED.
- [ ] Actualizar [[CLAUDE.md]] con la estructura real de cuenta (7 campañas país × producto) en vez de la campaña única ya pausada.
- [ ] Mantener monitoreo diario de GT Odoo, PY Odoo y GT Beco (mejores CPL) y vigilar COL Odoo / SLV Odoo (CPL sobre meta, $7-8).

---

## 🔗 Enlaces

- [[Reports/2026-11-09 - Reporte Performance]] — reporte completo del día con ranking de campañas.
- [[Daily notes/2026-11-10 - Resumen del Dia]] — resumen del día siguiente (generado por la rutina nocturna separada, documentaba el bloqueo antes de que este cierre lo resolviera).
- [[Reports/2026-10-22 - Reporte Performance]] — último cierre confirmado antes del bloqueo de 19 días.
- Tags: #daily-note #summary #meta-ads #octopus
