---
date: 2026-11-26
aliases: [resumen-2026-11-26]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-26

> [!warning] Nota sobre la fecha y los datos (mismo desajuste de zona horaria de rutinas anteriores)
> Esta rutina se ejecutó a las **~05:52 UTC del 26-nov** (≈ 23:52 del 2026-11-25 en `America/Guatemala`, zona horaria de la cuenta `act_2530001557366648`). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-26**: `date_preset=today` resolvió a **2026-11-25** (casi final, faltan ~8 minutos de cierre) y `date_preset=yesterday` resolvió a **2026-11-24** (final, ya publicado en [[Reports/2026-11-24 - Reporte Performance]]). Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-25** (casi final) y la comparación es contra **2026-11-24** (final). Se mantiene el nombre de archivo `2026-11-26` siguiendo el mismo patrón de rutinas anteriores (fecha del sistema al momento de ejecutarse).
>
> **Verificación contra el reporte final del 24-nov:** al re-consultar `date_preset=yesterday` (2026-11-24) hoy, el gasto lead-gen (7 campañas) sumó **$77.23** vs. **$77.11** del reporte final publicado (+0.16%), impresiones y clicks con drift de unidades; leads (7, misma distribución) no cambiaron. Consistente con el patrón de drift marginal de días anteriores; no se corrige el reporte ya publicado.
>
> **Higiene de repositorio:** `git status` al iniciar mostró `HEAD` **detached** en el commit más reciente (`4e0ae94`, "Add Daily Performance Report - 2026-11-24"), con la rama local `main` 4 commits por detrás. Se verificó la cadena (fast-forward limpio) y `git checkout main && git merge --ff-only 4e0ae94` dejó `main` al día; `git push` confirmó que **`origin/main` ya tenía todos los commits** ("Everything up-to-date") — sin pérdida de datos. A diferencia de rutinas anteriores, hoy no hubo divergencia real con `origin`, solo con la copia local de `main`/`HEAD`.

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 2 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today` → día real 2026-11-25, casi final, ~8 min de cierre restantes):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $8.18 | 1,271 | 35 | 2.75% | 3 | **$2.73** |
| 🟡 COL \| Odoo \| CP \| Servicios | ACTIVE | $7.73 | 624 | 8 | 1.28% | 1 | $7.73 |
| 🟡 PY \| Odoo \| CP \| Servicios | ACTIVE | $8.32 | 1,330 | 32 | 2.41% | 1 | $8.32 |
| 🟡 GT \| Odoo \| CP \| Servicios | ACTIVE | $30.86 | 4,906 | 95 | 1.94% | 3 | $10.29 |
| 🔴 PY \| Beco \| CP \| Conjuntos | ACTIVE | $8.63 | 1,311 | 18 | 1.37% | 0 | — (sin leads) |
| 🔴 GT \| Beco \| CP \| Conjuntos | ACTIVE | $14.20 | 2,097 | 34 | 1.62% | 0 | — (sin leads) |
| ⚫ SLV \| Beco \| CP \| Conjuntos | **PAUSADA hoy (14:24 hora local)** | $3.91 (parcial) | 537 | 5 | 0.93% | 0 | — (sin leads) |
| ⚪ Evento: Cotiza en segundos y cierra ventas desde el celular (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $6.55 | 9,500 | 232 | 2.44% | n/a | n/a |
| ⚪ Evento: El futuro de la gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED** (~14 campañas, sin cambios desde días anteriores).

**🔔 Cambio manual detectado hoy en Meta (vía `ads_account_get_activity_logs`, rango 2026-11-25 06:00 – 2026-11-26 06:00 UTC):**
- **11/25/2026 2:24 PM (hora de la cuenta):** el actor **Sebas Tenjo**, vía **Power Editor**, cambió el estado de **SLV \| Beco \| CP \| Conjuntos** de `Active` a `Inactive` (pausó la campaña). Esto corta la racha de ~6-7 días consecutivos en cero leads que se venía señalando como pendiente desde días anteriores.
- 11/25/2026 6:13 AM: "Account billed" — cargo rutinario de Meta por $537.00 USD (sin relación con cambios de campaña).

---

## 📊 Análisis e Insights

1. **Primera acción manual sobre el pendiente de SLV \| Beco:** después de varios días señalando esta campaña como la racha de cero leads más persistente de la cuenta (~6-7 días), un miembro del equipo (Sebas Tenjo) la pausó manualmente hoy a las 2:24 PM — resolviendo el punto de acción pendiente, aunque solo deteniendo el gasto, no diagnosticando la causa raíz.
2. **SLV \| Odoo se recupera con fuerza y es hoy la mejor campaña de la cuenta:** pasó de 0 leads ayer a **3 leads hoy**, CPL $2.73 — el mejor costo por lead del período reciente, muy por debajo de la meta $6-7.
3. **GT \| Odoo retrocede pese a mayor gasto:** leads 5→3 (-40%), gasto $25.34→$30.86 (+21.8%), CPL $5.07→$10.29 (+103%) — la campaña que más sostenía el CPL blendeado de la cuenta se debilita justo cuando SLV \| Odoo y COL \| Odoo se recuperan.
4. **COL \| Odoo rompe su racha de ceros** (0 leads ayer → 1 lead hoy, CPL $7.73).
5. **Solo 3 de 7 campañas lead-gen cierran el día en cero leads** (PY \| Beco, GT \| Beco, y SLV \| Beco parcial antes de pausarse) — mejora frente a las 4 de ayer (COL \| Odoo, PY \| Beco, SLV \| Beco, SLV \| Odoo).
6. **El CPL blendeado (incl. eventos, misma metodología que el reporte diario) mejora a $11.05** (gasto total $88.38 / 8 leads) vs. $12.01 de ayer (-8.0%) — esta vez la mejora sí viene acompañada de más leads (7→8, +14.3%), no solo de menor gasto.
7. **GT \| Beco acumula el gasto más caro sin ningún retorno:** $14.20 sin leads, el peor ratio gasto/resultado del día.
8. **El tráfico crece de forma generalizada:** impresiones +5.1% (21,576 vs. 20,528), clicks +4.3% (459 vs. 440), CTR blendeado prácticamente estable (2.13% vs. 2.14%) — sigue bajo la meta 3-4%.
9. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) y `ads_get_errors` no devolvió errores de entrega/publicación bloqueantes — mismo patrón que días anteriores.
10. **Evento "El futuro de la gestión de nómina"** sigue sin gasto/impresiones por ~16º día consecutivo.
11. No hubo otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina (más allá de la acción manual de Sebas Tenjo en Ads Manager), y no se realizó investigación externa de competencia o tendencias de mercado.
12. **Dato pendiente de cierre:** como se explica en la nota de advertencia arriba, los números de "hoy" (2026-11-25) están casi finales (~8 minutos de cierre restantes); se espera que la rutina de reporte final confirme estas cifras con una variación marginal.

---

## ✏️ Cambios Realizados

**Por esta rutina (Claude Code):** ninguno en las campañas lead-gen — rutina de solo lectura/análisis (`ads_get_ad_accounts`, `ads_get_ad_entities` con `date_preset=today`/`yesterday`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña.

**Cambio manual en Meta (por un miembro del equipo, no por esta rutina):** **SLV \| Beco \| CP \| Conjuntos** pausada por Sebas Tenjo vía Power Editor a las 2:24 PM (hora de la cuenta) — ver detalle en la sección de Campañas Revisadas.

**Repositorio:** se corrigió un desajuste de `HEAD`/`main` local (fast-forward a `origin/main`, sin pérdida de datos) — ver nota de advertencia arriba.

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_accounts` para confirmar que `act_2530001557366648` (GT | Octopus Innovations) sigue activa y consultable.
- Se consultó `ads_get_ad_entities` (nivel cuenta) para confirmar la zona horaria real de la cuenta (`timezone_name=America/Guatemala`) junto con `date -u` del sistema, confirmando que "hoy" de la cuenta = 2026-11-25 (casi final, ~8 min de cierre).
- Se consultó `ads_get_ad_entities` (nivel campaña) con `date_preset=today` (→ 25-nov) y `date_preset=yesterday` (→ 24-nov) para las 7 campañas lead-gen activas más las 2 de evento, incluyendo una consulta puntual por `object_ids` para **SLV \| Beco** (ya no aparece en el filtro `effective_status=ACTIVE` tras ser pausada hoy) en ambos días.
- Se comparó `date_preset=yesterday` (24-nov) contra las cifras ya publicadas en [[Reports/2026-11-24 - Reporte Performance]], confirmando consistencia (leads idénticos, gasto/impresiones con drift marginal esperado).
- Se consultó `ads_account_get_activity_logs` para el rango 2026-11-25 06:00 – 2026-11-26 06:00 UTC (día completo de la cuenta): se detectó el cambio manual de SLV \| Beco y un cargo rutinario de Meta (ver Campañas Revisadas).
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha.
- Se ejecutó `ads_get_errors` sobre la cuenta: sin errores bloqueantes de publicación o entrega.
- Se auditó `git status`/`git log`: se detectó `HEAD` detached y `main` local desincronizado; se corrigió con fast-forward y se verificó que `origin/main` ya tenía todos los commits.
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen + 2 de evento) | 2026-11-25 (casi final, ~8 min de cierre) | 2026-11-24 (final, verificado) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$11.05** | $12.01 | $6-7 | 🟡 Mejora (-8.0%), sigue sobre meta |
| Gasto Total (incl. eventos) | $88.38 | $84.04 | - | 🟡 +5.2% |
| Leads Totales | 8 | 7 | 4-5/día | 🟢 +14.3%, sobre meta |
| CTR Promedio (incl. eventos) | 2.13% | 2.14% | 3-4% | 🔴 Estable, sigue bajo meta |
| Impresiones (incl. eventos) | 21,576 | 20,528 | - | 🟢 +5.1% |
| Clicks (incl. eventos) | 459 | 440 | - | 🟢 +4.3% |
| Campañas activas sin ningún lead | 3 (PY Beco, GT Beco, SLV Beco parcial) | 4 (COL Odoo, PY Beco, SLV Beco, SLV Odoo) | - | 🟢 Mejora, 1 campaña menos en cero |
| Mejor campaña del día | SLV Odoo ($2.73 CPL, 3 leads) | GT Odoo ($5.07 CPL, 5 leads) | - | — |
| Cambios de campaña ejecutados hoy | 1 (pausa manual de SLV Beco, por Sebas Tenjo) | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] **Monitorear a GT \| Odoo** (CPL $5.07 → $10.29, leads 5→3, gasto +21.8%) — confirmar si es una fluctuación de un día o el inicio de un deterioro en la campaña que más sostiene el CPL blendeado de la cuenta.
- [ ] Confirmar que **SLV \| Odoo** sostiene su recuperación ($2.73 CPL, 3 leads) y no es un pico aislado.
- [ ] Dar seguimiento a si **SLV \| Beco**, ahora pausada manualmente por Sebas Tenjo, se reactiva, se reemplaza por una versión nueva, o permanece pausada — y documentar la decisión/razón cuando se conozca.
- [ ] Revisar por qué **GT \| Beco** sigue sin generar ningún lead pese a ser, junto con GT \| Odoo, la campaña con mayor gasto del día ($14.20).
- [ ] Confirmar al cierre formal del 2026-11-25 si el CPL ($11.05) y el conteo de leads (8) se mantienen, o si hay atribución tardía — generar `Reports/2026-11-25 - Reporte Performance.md` una vez cierre el día.
- [ ] Seguir trabajando el CTR blendeado (2.13% vs meta 3-4%) con pruebas A/B de creativo.
- [ ] Verificar en Ads Manager por qué "Evento: El futuro de la gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas (~16 días) — confirmar `start_time`, presupuesto o calendario.
- [ ] Pendiente heredado: decidir el futuro de las ~14 campañas históricas pausadas.
- [ ] Pendiente heredado (menor prioridad hoy, sin divergencia real con `origin`): seguir vigilando que cada rutina empiece con `git fetch && git checkout main && git merge --ff-only origin/main` antes de crear archivos, para evitar que `HEAD`/`main` local queden desincronizados entre rutinas.

---

## 🔗 Enlaces

- [[Reports/2026-11-24 - Reporte Performance]] — reporte final y verificado del día anterior, usado como base de comparación en esta nota.
- [[Daily notes/2026-11-25 - Resumen del Dia]] — nota del día anterior.
- Tags: #daily-note #summary #meta-ads #octopus
