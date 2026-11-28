---
date: 2026-11-28
aliases: [resumen-2026-11-28]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-28

> [!warning] Nota sobre la fecha y los datos (mismo desajuste de zona horaria de rutinas anteriores)
> Esta rutina se ejecutó a las **~05:51 UTC del 28-nov** (≈ 23:51 del 2026-11-27 en `America/Guatemala`, zona horaria de la cuenta `act_2530001557366648`). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-28**: `date_preset=today` resolvió a **2026-11-27** (casi final, faltan ~9 minutos de cierre) y `date_preset=yesterday` resolvió a **2026-11-26** (final, ya publicado en [[Reports/2026-11-26 - Reporte Performance]]). Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-27** (casi final) y la comparación es contra **2026-11-26** (final). Se mantiene el nombre de archivo `2026-11-28` siguiendo el mismo patrón de rutinas anteriores (fecha del sistema al momento de ejecutarse).
>
> **Verificación contra el reporte final del 26-nov:** al re-consultar `date_preset=yesterday` (2026-11-26) hoy, las cifras coinciden con el reporte final publicado con drift marginal esperado (gasto blendeado $67.11 hoy vs. $66.85 publicado; CPL $9.59 vs. $9.55); leads idénticos (7) en todas las campañas. Consistente con el patrón de drift de días anteriores; no se corrige el reporte ya publicado.
>
> **Higiene de repositorio:** `git status` al iniciar mostró `HEAD` **detached** en un commit antiguo (`c7e0402`, "Add Daily Performance Report - 2026-11-22"), con la rama local `main` 8 commits por detrás de `origin/main`. Se corrigió con `git checkout main && git fetch && git merge --ff-only origin/main` — fast-forward limpio hasta `7efa59a`, sin pérdida de datos ni divergencia real con `origin`. Este problema se repite rutina tras rutina desde el 20-nov; sigue pendiente investigar la causa raíz.

---

## 🎯 Campañas Revisadas

Se revisaron las 6 campañas lead-gen activas + 2 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today` → día real 2026-11-27, casi final, ~9 min de cierre restantes):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 PY \| Odoo \| CP \| Servicios | ACTIVE | $6.71 | 1,093 | 21 | 1.92% | 2 | **$3.36** |
| 🟢 GT \| Beco \| CP \| Conjuntos | ACTIVE | $13.23 | 1,753 | 26 | 1.48% | 2 | $6.62 |
| 🟡 SLV \| Odoo \| CP \| Servicios | ACTIVE | $7.11 | 1,002 | 29 | 2.89% | 1 | $7.11 |
| 🟡 PY \| Beco \| CP \| Conjuntos | ACTIVE | $6.48 | 993 | 11 | 1.11% | 1 | $6.48 |
| 🔴 GT \| Odoo \| CP \| Servicios | ACTIVE | $25.15 | 3,180 | 73 | 2.30% | 2 | $12.58 |
| 🔴 COL \| Odoo \| CP \| Servicios | ACTIVE | $7.16 | 475 | 10 | 2.11% | 0 | — (sin leads) |
| ⚫ SLV \| Beco \| CP \| Conjuntos | **PAUSADA** (desde 25-nov, 14:24h, Sebas Tenjo) | $0.00 | 0 | 0 | — | 0 | — (pausada, 3er día consecutivo) |
| ⚪ Evento: Cotiza en segundos y cierra ventas desde el celular (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |
| ⚪ Evento: El futuro de la gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED** (~14 campañas históricas, sin cambios desde días anteriores).

**🔔 Actividad detectada hoy en Meta (vía `ads_account_get_activity_logs`, rango 2026-11-27 06:00 – 2026-11-28 06:00 UTC):** **0 entradas** — ni cambios manuales ni eventos de sistema registrados. Es una diferencia notable vs. días anteriores, que siempre mostraban al menos 1 entrada de sistema ("Ad delivered"). SLV \| Beco sigue pausada tal como quedó el 25-nov — no se reactivó ni se reemplazó.

---

## 📊 Análisis e Insights

1. **El CPL blendeado mejora a $8.23 (-14.2%), y por primera vez en varios días la mejora viene acompañada de más leads, no de menos:** 8 leads hoy vs. 7 ayer (+14.3%), con gasto casi plano (-1.9%). Rompe el patrón reciente donde el CPL mejoraba solo porque caía el gasto/tráfico.
2. **La caída de tráfico continúa, aunque más moderada que el salto del 26-nov:** impresiones -23.8% (8,496 vs. 11,149) y clicks -31.7% (170 vs. 249) vs. el día final anterior. `ads_insights_anomaly_signal` sigue sin detectar solapamiento de subasta, fatiga de creativo ni audiencia estrecha, y `ads_get_errors` no devolvió errores de entrega/publicación — la causa de fondo sigue sin identificarse.
3. **El evento "Cotiza en segundos" deja de recibir gasto por completo** (de $6.63 el 25-nov, a $1.63 el 26-nov, a **$0.00** hoy) — tercer día consecutivo de caída y ahora inactivo del todo; posible fin de calendario/presupuesto del evento, pendiente de confirmar en Ads Manager.
4. **GT \| Odoo encadena su cuarto día consecutivo de deterioro de CPL:** $5.06 (24-nov) → $10.42 (25-nov) → $12.25 (26-nov, final) → **$12.58** (hoy) — sigue siendo la campaña de mayor gasto de la cuenta ($25.15 hoy) sin revertir la tendencia.
5. **GT \| Beco tiene su mejor día del período reciente:** 1 → 2 leads, CPL $13.09 → **$6.62** (-49.4%) — pasa de ser la campaña más cara de la cuenta a quedar dentro del rango meta $6-7.
6. **PY \| Odoo se recupera con fuerza:** 0 → 2 leads, revirtiendo el cero de ayer, con el **mejor CPL del día ($3.36)**, muy por debajo de la meta.
7. **COL \| Odoo rompe su racha de recuperación:** 2 leads (ayer) → **0 leads** (hoy), tras dos días consecutivos de mejora — revierte por completo su buen desempeño reciente.
8. **PY \| Beco mejora dentro de meta:** CPL $8.01 → $6.48 (-19.1%), manteniendo 1 lead.
9. **SLV \| Odoo se mantiene prácticamente estable:** 1 lead ambos días, CPL $6.81 → $7.11 (+4.4%), cerca del límite superior de la meta.
10. **El CTR blendeado retrocede:** 2.00% vs. 2.23% ayer (-0.23pp), alejándose aún más de la meta 3-4%.
11. **SLV \| Beco sigue pausada sin novedad** (3er día consecutivo desde que Sebas Tenjo la pausó el 25-nov).
12. **Evento "El futuro de la gestión de nómina"** sigue sin gasto/impresiones por ~19º día consecutivo.
13. **Actividad en Meta en cero:** a diferencia de todos los días anteriores revisados (que mostraban al menos 1 evento de sistema), hoy el activity log no registró ninguna entrada — ni manual ni automática — en todo el rango de 24h de la cuenta.
14. No hubo otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.
15. **Dato pendiente de cierre:** como se explica en la nota de advertencia arriba, los números de "hoy" (2026-11-27) están casi finales (~9 minutos de cierre restantes); se espera que la rutina de reporte final confirme estas cifras con una variación marginal.

---

## ✏️ Cambios Realizados

**Por esta rutina (Claude Code):** ninguno en las campañas lead-gen — rutina de solo lectura/análisis (`ads_get_ad_accounts`, `ads_get_ad_entities` con `date_preset=today`/`yesterday`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña.

**Cambios manuales en Meta:** ninguno detectado hoy — el activity log del día completo de la cuenta no registró ninguna entrada (ni de sistema ni de un miembro del equipo).

**Repositorio:** se corrigió un desajuste de `HEAD`/`main` local (fast-forward de 8 commits hasta `origin/main`, sin pérdida de datos) — ver nota de advertencia arriba. Problema recurrente desde el 20-nov, causa raíz aún sin investigar.

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_accounts` para confirmar que `act_2530001557366648` (GT | Octopus Innovations) sigue activa y consultable.
- Se consultó `ads_get_ad_entities` (nivel cuenta) para confirmar la zona horaria real de la cuenta (`timezone_name=America/Guatemala`) junto con `date -u` del sistema, confirmando que "hoy" de la cuenta = 2026-11-27 (casi final, ~9 min de cierre).
- Se consultó `ads_get_ad_entities` (nivel campaña) con `date_preset=today` (→ 27-nov) y `date_preset=yesterday` (→ 26-nov) para las 6 campañas lead-gen activas más las 2 de evento, y se listó el resto de la cuenta (~14 campañas históricas, todas PAUSED, sin cambios).
- Se comparó `date_preset=yesterday` (26-nov) contra las cifras ya publicadas en [[Reports/2026-11-26 - Reporte Performance]], confirmando consistencia (leads idénticos, gasto/CPL con drift marginal esperado).
- Se consultó `ads_account_get_activity_logs` para el rango 2026-11-27 06:00 – 2026-11-28 06:00 UTC (día completo de la cuenta): 0 entradas, sin cambios manuales ni eventos de sistema — notable por ser el primer día sin ninguna entrada.
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha (no explica la caída de tráfico observada — ver Análisis e Insights #2).
- Se ejecutó `ads_get_errors` sobre la cuenta: sin errores bloqueantes de publicación o entrega.
- Se auditó `git status`/`git log`: se detectó `HEAD` detached y `main` local 8 commits por detrás de `origin/main`; se corrigió con fast-forward, sin divergencia real ni pérdida de datos.
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 6 campañas lead-gen + 2 de evento) | 2026-11-27 (casi final, ~9 min de cierre) | 2026-11-26 (final, verificado) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$8.23** | $9.59 | $6-7 | 🟡 Mejora (-14.2%), sigue sobre meta |
| Gasto Total (incl. eventos) | $65.84 | $67.11 | - | 🟢 -1.9% |
| Leads Totales | 8 | 7 | 4-5/día | 🟢 +14.3%, por encima de meta |
| CTR Promedio (incl. eventos) | 2.00% | 2.23% | 3-4% | 🔴 -0.23pp, se aleja de la meta |
| Impresiones (incl. eventos) | 8,496 | 11,149 | - | 🔴 -23.8% (caída moderada, sin causa identificada) |
| Clicks (incl. eventos) | 170 | 249 | - | 🔴 -31.7% (caída moderada, sin causa identificada) |
| Campañas activas sin ningún lead | 1 (COL Odoo) | 1 (PY Odoo) | - | — Igual, cambia cuál |
| Mejor campaña del día | PY Odoo ($3.36 CPL, 2 leads) | COL Odoo ($3.62 CPL, 2 leads) | - | — |
| Cambios de campaña ejecutados hoy | 0 | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] **Confirmar en Ads Manager por qué el evento "Cotiza en segundos" cayó a $0.00 de gasto** (desde $6.63 el 25-nov) — verificar si el evento ya finalizó, se agotó el presupuesto, o hay un problema de calendario.
- [ ] **Seguir escalando/replicando lo que funcionó en GT \| Beco** (CPL $13.09 → $6.62, su mejor día reciente) y confirmar que no es un pico aislado.
- [ ] **Confirmar que PY \| Odoo sostiene su recuperación** (0 → 2 leads, CPL $3.36, el mejor del día) tras su racha de ceros.
- [ ] **Investigar por qué COL \| Odoo cayó a cero leads hoy**, revirtiendo dos días consecutivos de recuperación.
- [ ] **Confirmar/actuar sobre GT \| Odoo**, que encadena 4 días consecutivos de deterioro de CPL ($5.06→$10.42→$12.25→$12.58) siendo la campaña con mayor gasto de la cuenta.
- [ ] Seguir investigando la caída sostenida de tráfico (impresiones y clicks a la baja 3 días seguidos) pese a que no hay anomalías ni errores detectados.
- [ ] Dar seguimiento a si **SLV \| Beco**, pausada por Sebas Tenjo desde el 25-nov (ya 3 días), se reactiva, se reemplaza por una versión nueva, o permanece pausada — y documentar la decisión/razón cuando se conozca.
- [ ] Confirmar al cierre formal del 2026-11-27 si el CPL ($8.23) y el conteo de leads (8) se mantienen, o si hay atribución tardía — generar `Reports/2026-11-27 - Reporte Performance.md` una vez cierre el día.
- [ ] Seguir trabajando el CTR blendeado (2.00% vs meta 3-4%, retrocediendo) con pruebas A/B de creativo.
- [ ] Verificar en Ads Manager por qué "Evento: El futuro de la gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas (~19 días) — confirmar `start_time`, presupuesto o calendario.
- [ ] Pendiente heredado: decidir el futuro de las ~14 campañas históricas pausadas.
- [ ] Pendiente heredado (recurrente desde el 20-nov): investigar la causa raíz de por qué cada rutina encuentra `HEAD`/`main` local desincronizado de `origin/main` al iniciar.

---

## 🔗 Enlaces

- [[Reports/2026-11-26 - Reporte Performance]] — reporte final y verificado del día anterior, usado como base de comparación en esta nota.
- [[Daily notes/2026-11-27 - Resumen del Dia]] — nota del día anterior.
- Tags: #daily-note #summary #meta-ads #octopus
