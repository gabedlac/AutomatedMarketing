---
date: 2026-11-26
aliases: [resumen-2026-11-26]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-26

> [!warning] Corrección de contenido (este archivo documentaba antes el día 2026-11-25)
> Hasta hoy, este archivo documentaba de forma **provisional** el día **2026-11-25** (casi final, ~8 minutos antes del cierre de cuenta), por el desajuste de zona horaria que afectaba al disparador de rutinas anteriores (fecha de archivo = fecha de ejecución, un día después del período real reportado). Esos datos del 25-nov ya están **finalizados y publicados** en [[Reports/2026-11-25 - Reporte Performance]] — nada se pierde, solo se corrige dónde vive la nota provisional.
>
> **A partir de esta rutina, el disparador se ejecuta correctamente a las ~07:07 hora local de la cuenta (America/Guatemala)**, bien entrada la mañana y no a los pocos minutos de la medianoche. Por eso, este archivo se reescribe para documentar **su propio día, 2026-11-26** (día completo y cerrado, datos finales), alineando de nuevo el nombre del archivo con su contenido. El reporte detallado y verificado de este mismo día está en [[Reports/2026-11-26 - Reporte Performance]].

---

## 🎯 Resumen Ejecutivo del Día

El 2026-11-26 cerró con **$66.85 de gasto total** (-25.1% vs. el 25-nov), **7 leads** (-12.5%) y un **CPL blendeado de $9.55** — la mejor cifra de CPL del período reciente (-14.4% vs. $11.16 de ayer), aunque sigue ~36% sobre el límite superior de la meta ($6-7). La caída de actividad (impresiones -49.0%, clicks -46.7%) la explica en su mayoría el colapso de gasto/impresiones en la campaña de evento "Cotiza en segundos" (-75.3% / -73.7%), sin anomalías ni errores de entrega detectados.

---

## 🔄 Cambios Principales vs. Día Anterior (2026-11-25)

| Campaña | Status | Leads hoy | Leads ayer | CPL hoy | CPL ayer |
|---|---|---|---|---|---|
| 🟢 COL \| Odoo \| CP \| Servicios | **Arriba** | 2 | 1 | $3.53 | $7.77 |
| 🟡 SLV \| Odoo \| CP \| Servicios | Abajo en volumen, estable en costo | 1 | 3 | $6.79 (dentro de meta) | $2.77 |
| 🟡 PY \| Beco \| CP \| Conjuntos | Estable | 1 | 0 | $7.99 | — (sin leads) |
| 🔴 GT \| Odoo \| CP \| Servicios | Abajo | 2 | 3 | $12.24 | $10.42 |
| 🟢 GT \| Beco \| CP \| Conjuntos | Arriba | 1 | 0 | $13.08 | — (sin leads) |
| 🔴 PY \| Odoo \| CP \| Servicios | Abajo | 0 | 1 | — (sin leads) | $8.40 |
| ⚫ SLV \| Beco \| CP \| Conjuntos | Pausada todo el día (sin cambios) | 0 | 0 (parcial) | — | — |
| ⚪ Evento: Cotiza en segundos (Odoo) | Abajo fuerte (gasto -75.3%) | n/a (15 RSVP) | n/a | n/a | n/a |

**Resto de la cuenta:** ~14 campañas históricas PAUSED, sin cambios.

**Actividad en Meta (vía `ads_account_get_activity_logs`, 26-nov 06:00 – 27-nov 06:00 UTC):** solo 1 entrada, un evento de sistema rutinario ("Ad delivered"), sin cambios manuales de presupuesto, estado o targeting por parte del equipo. `ads_insights_anomaly_signal` y `ads_get_errors` no detectaron anomalías ni errores bloqueantes.

---

## 📋 Próximas Acciones

- [ ] Confirmar en Ads Manager si el colapso de gasto/impresiones del evento "Cotiza en segundos" se debe a que el evento ya ocurrió/está por ocurrir o a un cambio de presupuesto/calendario.
- [ ] Investigar por qué **PY \| Odoo** cayó a cero leads (1→0) con gasto similar.
- [ ] Confirmar que **SLV \| Odoo** sostiene su CPL dentro de meta ($6.79) y evaluar escalar su presupuesto.
- [ ] Seguir monitoreando a **GT \| Odoo** (CPL $12.24, +17.5% vs. ayer), la campaña de mayor gasto de la cuenta.
- [ ] Decidir el futuro de **SLV \| Beco** (pausada desde el 25-nov).
- [ ] Verificar por qué "Evento: El futuro de la gestión de nómina" sigue sin actividad (~18 días).
- [ ] Ver recomendaciones completas en [[Reports/2026-11-26 - Reporte Performance]].

---

## 🔗 Enlaces

- [[Reports/2026-11-26 - Reporte Performance]] — reporte detallado y verificado de este mismo día.
- [[Reports/2026-11-25 - Reporte Performance]] — reporte final del día anterior (donde viven los datos que esta nota documentaba antes de la corrección de hoy).
- [[Daily notes/2026-11-27 - Resumen del Dia]] — nota del día siguiente.
- Tags: #daily-note #summary
