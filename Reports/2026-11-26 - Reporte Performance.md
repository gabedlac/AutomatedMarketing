---
date: 2026-11-26
report-type: Daily
period: 2026-11-26
campaign: GT | Octopus Innovations (act_2530001557366648)
tags: [daily-note, performance, meta-ads, octopus]
---

# 📊 Reporte Performance - 2026-11-26

## 📋 Resumen Ejecutivo

**Cuenta:** GT | Octopus Innovations (`act_2530001557366648`)
**Período:** 2026-11-26 (día completo, zona horaria de la cuenta — America/Guatemala)
**Generado:** 2026-11-27, 07:07 hora local de la cuenta — día ya cerrado, datos finales

> **Nota sobre esta rutina:** a partir de hoy el disparador se ejecuta correctamente a las ~07:07 hora local de la cuenta (America/Guatemala), ya avanzada la mañana y no a los pocos minutos de la medianoche como ocurría en rutinas anteriores (ver advertencias de zona horaria en reportes y notas previas del 23 al 27 de noviembre). Por eso, este es el primer reporte en que `date_preset=yesterday` resuelve de forma limpia al día completo y cerrado (2026-11-26) en una sola consulta.

### 🎯 Métricas Clave (blendeado, 6 campañas lead-gen activas + 1 de evento con actividad)

| Métrica | Valor | Meta | Status |
|---|---|---|---|
| CPL (Costo por Lead) | **$9.55** | $6-7 | 🔴 -14.4% vs. ayer ($11.16) — mejor cifra del período reciente, aunque sigue ~36% sobre el límite superior de la meta |
| CTR | 2.24% | 3-4% | 🔴 +0.10pp vs. ayer (2.14%), sigue bajo meta |
| Leads Totales | 7 | 4-5/día | 🟢 Sobre meta, aunque -12.5% vs. ayer (8) |
| Gasto Total | $66.85 | — | 🟢 -25.1% vs. ayer ($89.28) |
| ROAS | No aplica | — | — (campañas de Leads/Evento, sin valor de conversión asignado) |
| Impresiones | 11,135 | — | 🔴 -49.0% vs. ayer (21,846) |
| Clicks | 249 | — | 🔴 -46.7% vs. ayer (467) |

> **Nota sobre ROAS:** no aplica porque todas las campañas activas tienen objetivo `OUTCOME_LEADS` (generación de leads) o `EVENT_RESPONSES` (campañas de evento), sin pixel de valor de compra asociado.

> ⚠️ **Alerta principal del día:** el CPL mejora a **$9.55** (-14.4% vs. ayer), la mejor cifra del período reciente, pero viene acompañado de una caída generalizada de actividad: gasto -25.1%, impresiones -49.0% y clicks -46.7%. La mayor parte de esa caída la explica la campaña de evento **"Cotiza en segundos y cierra ventas desde el celular"**, cuyo gasto colapsó -75.3% ($6.59 → $1.63) e impresiones -73.7% (9,628 → 2,527) de un día a otro, sin que `ads_insights_anomaly_signal` ni `ads_get_errors` detectaran anomalías o errores de entrega — conviene confirmar en Ads Manager si el evento promocionado ya pasó o si cambió su calendario/presupuesto.

---

## 📈 Performance por Campaña (ranked por CPL)

| # | Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|---|
| 1 | 🟢 COL \| Odoo \| CP \| Servicios | ACTIVE | $7.05 | 669 | 20 | 2.99% | 2 | **$3.53** |
| 2 | 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $6.79 | 1,066 | 23 | 2.16% | 1 | $6.79 (dentro de meta $6-7) |
| 3 | 🟡 PY \| Beco \| CP \| Conjuntos | ACTIVE | $7.99 | 962 | 27 | 2.81% | 1 | $7.99 |
| 4 | 🔴 GT \| Odoo \| CP \| Servicios | ACTIVE | $24.48 | 3,393 | 80 | 2.36% | 2 | $12.24 |
| 5 | 🔴 GT \| Beco \| CP \| Conjuntos | ACTIVE | $13.08 | 1,710 | 33 | 1.93% | 1 | $13.08 |
| 6 | 🔴 PY \| Odoo \| CP \| Servicios | ACTIVE | $5.83 | 808 | 17 | 2.10% | 0 | — (sin leads) |
| 7 | ⚫ SLV \| Beco \| CP \| Conjuntos | **PAUSADA todo el día** (desde 25-nov, 14:24h, Sebas Tenjo) | $0.00 | 0 | 0 | — | 0 | — (pausada) |
| — | ⚪ Evento: Cotiza en segundos y cierra ventas desde el celular (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $1.63 | 2,527 | 49 | 1.94% | n/a (15 RSVP) | n/a |
| — | ⚪ Evento: El futuro de la gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |

**Resto de la cuenta:** ~14 campañas PAUSED sin gasto ni actividad (sin cambios: COL \| Beco \| CP \| Conjuntos, COL \| Odoo \| CP \| Servicios versión de prueba anterior, 2x boosts de "Evento: Odoo en Acción", Pyme Colombia, Toma El control de tu pyme GT/USA, Accurate Partners - Loyalti, Odoo Test GT, Beco GT histórica, Pyme El Salvador, Conversión Clientes Potenciales MX/PY, 🟡 Conversión - Clientes Potenciales).

---

## 💡 Insights Clave y Análisis

1. **Caída generalizada de actividad, liderada por la campaña de evento:** el colapso de gasto/impresiones en "Cotiza en segundos" (-75.3% / -73.7%) explica la mayor parte de la baja de -49.0% en impresiones y -46.7% en clicks a nivel cuenta — sin anomalías ni errores detectados, apunta a que el evento promocionado ya ocurrió o a un cambio de calendario/presupuesto, no a un problema de entrega.
2. **El CPL blendeado mejora a $9.55 (-14.4% vs. $11.16 de ayer), la mejor cifra del período reciente**, aunque sigue ~36% sobre el límite superior de la meta ($6-7) y el gasto también bajó (-25.1%), por lo que la mejora no viene acompañada de más leads.
3. **SLV \| Odoo entra por primera vez dentro del rango objetivo de CPL** ($6.79, dentro de $6-7), aunque con menos volumen que ayer (3 → 1 lead).
4. **COL \| Odoo es la mejor campaña del día** (CPL $3.53, 2 leads), mejorando fuerte vs. $7.77/1 lead de ayer.
5. **GT \| Odoo sigue deteriorado:** CPL $10.42 → **$12.24** (+17.5%), con menos leads (3→2, -33%) y menos gasto ($31.27→$24.48, -21.7%) — la campaña de mayor gasto de la cuenta no recupera su nivel histórico (~$5 CPL).
6. **GT \| Beco recupera 1 lead** (0 ayer → 1 hoy) pero sigue siendo, junto con GT \| Odoo, la campaña más cara en CPL ($13.08).
7. **PY \| Odoo cae a cero leads** (1 ayer → 0 hoy) con gasto similar ($8.40→$5.83, -30.6%).
8. **PY \| Beco se mantiene estable:** 1 lead igual que ayer, CPL $8.70 → $7.99 (-8.2%).
9. **SLV \| Beco permanece pausada todo el día** (desde la pausa manual de Sebas Tenjo el 25-nov a las 14:24 hora local) — sin reactivación ni reemplazo.
10. **CTR blendeado mejora levemente a 2.24%** (vs. 2.14% ayer, +0.10pp) pero sigue bajo la meta 3-4%.
11. **Sin anomalías ni errores de entrega detectados:** `ads_insights_anomaly_signal` no encontró solapamiento de subasta, fatiga de creativo ni audiencia estrecha; `ads_get_errors` no devolvió errores bloqueantes de publicación o entrega.
12. **Actividad de cuenta (`ads_account_get_activity_logs`, 26-nov 06:00 – 27-nov 06:00 UTC):** una sola entrada, un evento de sistema rutinario ("Ad delivered" / inicio de entrega de un anuncio) — sin cambios manuales de presupuesto, estado o targeting por parte del equipo.
13. **Verificación contra la nota provisional del mismo día:** la nota provisional publicada ~9 minutos antes del cierre de cuenta ([[Daily notes/2026-11-27 - Resumen del Dia]]) reportó gasto blendeado $66.27 con la misma distribución de 7 leads; los datos finales de este reporte (gasto $66.85) confirman un drift marginal de atribución tardía (~+0.9%), sin cambios en el conteo de leads — consistente con el patrón de días anteriores, y esta vez sin el desajuste de zona horaria que afectaba a esas notas provisionales.
14. **Evento "El futuro de la gestión de nómina"** sigue sin gasto/impresiones por ~18º día consecutivo.
15. **Corrección de archivo:** el archivo `Daily notes/2026-11-26 - Resumen del Dia.md` documentaba hasta hoy, de forma provisional, el día 2026-11-25 (por el desajuste de zona horaria de rutinas anteriores). Esos datos ya están finalizados y publicados en [[Reports/2026-11-25 - Reporte Performance]]. Con el disparador corregido, ese archivo se actualiza en esta misma rutina para documentar su propio día (2026-11-26), alineando de nuevo nombre de archivo y contenido.

---

## 🎬 Recomendaciones Accionables

### Inmediatas
- [ ] **Confirmar en Ads Manager** si el colapso de gasto/impresiones del evento "Cotiza en segundos" (-75.3% / -73.7%) se debe a que el evento promocionado ya ocurrió o está por ocurrir, o a un cambio de presupuesto/calendario.
- [ ] Investigar por qué **PY \| Odoo** cayó a cero leads (1→0) con gasto similar al día anterior.
- [ ] Confirmar que **SLV \| Odoo** sostiene su CPL dentro de meta ($6.79) y evaluar si se puede escalar el presupuesto sin perder ese nivel de costo.

### Corto plazo
- [ ] Seguir monitoreando a **GT \| Odoo** (CPL $12.24, +17.5% vs. ayer) — la campaña de mayor gasto de la cuenta, que no logra recuperar su CPL histórico (~$5).
- [ ] Decidir el futuro de **SLV \| Beco** (pausada desde el 25-nov) — reactivar, reemplazar por una versión nueva, o mantener pausada.
- [ ] Continuar la investigación pendiente del formulario instantáneo/integración CRM/pixel para las campañas con leads intermitentes (PY \| Beco, GT \| Beco, PY \| Odoo).

### Mediano plazo
- [ ] Verificar en Ads Manager por qué la campaña de evento **"El futuro de la gestión de nómina (Odoo)"** sigue sin reportar gasto ni impresiones tras ~18 días consecutivos.
- [ ] Seguir trabajando el CTR blendeado (2.24% vs. meta 3-4%) con pruebas A/B de creativo, evaluando primero por CTR y luego por CPL, según los principios de la bóveda.
- [ ] Decidir el futuro de las ~14 campañas históricas pausadas.

---

## 📌 Notas y Observaciones

- Datos obtenidos vía `ads_get_ad_entities` (`date_preset=yesterday` relativo al 2026-11-27, resolviendo de forma limpia a 2026-11-26) sobre `act_2530001557366648`, día completo y cerrado en la zona horaria de la cuenta (America/Guatemala; rutina ejecutada a las ~07:07 hora local).
- ROAS no se reporta porque las campañas activas de la cuenta son 100% de generación de leads (`OUTCOME_LEADS`) o de respuesta a evento (`EVENT_RESPONSES`), sin valor de conversión de compra asociado.
- Ver insight 15 arriba sobre la corrección del archivo `Daily notes/2026-11-26 - Resumen del Dia.md`.

---

## 🔗 Enlaces

- [[Daily notes/2026-11-26 - Resumen del Dia]] — nota diaria de este mismo día (corregida en esta rutina para reflejar los datos finales de este reporte; ver insight 15).
- [[Daily notes/2026-11-27 - Resumen del Dia]] — nota que documentaba de forma provisional los datos de este mismo día 26-nov antes del cierre de la cuenta (confirmados aquí con drift marginal).
- [[Reports/2026-11-25 - Reporte Performance]] — reporte final del día anterior, usado como base de comparación.

---

**Generado por:** Claude (rutina automática "Daily Meta Ads Performance Report - 7 AM Guatemala")
**Período cubierto:** 2026-11-26
**Próxima revisión:** 2026-11-28
