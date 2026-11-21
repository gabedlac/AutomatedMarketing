---
date: 2026-11-21
aliases: [resumen-2026-11-21]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-21

> [!warning] Nota sobre la fecha y los datos (mismo desajuste de zona horaria de rutinas anteriores)
> Esta rutina se ejecutó a las **~05:52 UTC del 21-nov** (≈ 23:52 del 2026-11-20 en `America/Guatemala`, zona horaria de la cuenta `act_2530001557366648`). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-21** (faltaban ~8 minutos): `date_preset=today` resolvió a **2026-11-20** y `date_preset=yesterday` resolvió a **2026-11-19** (datos finales, consistentes con [[Reports/2026-11-19 - Reporte Performance]]). Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-20** (provisional, faltan ~8 minutos de cierre) y la comparación es contra **2026-11-19** (final, verificado). Se mantiene el nombre de archivo `2026-11-21` siguiendo el mismo patrón de rutinas anteriores (fecha del sistema al momento de ejecutarse) — mismo desajuste ya documentado en las notas del 18, 19 y 20-nov. Es probable que una rutina posterior corrija esta nota con los números finales una vez cierre formalmente el día.
>
> **Hallazgo de higiene de repo corregido en esta rutina:** al iniciar, `HEAD` estaba detached en el commit `a1402ea` ("Add Daily Performance Report - 2026-11-19"), con la rama local `main` 6 commits por detrás (todavía en `23360d1`, el reporte del 16-nov), aunque `origin/main` ya estaba sincronizado en `a1402ea`. Se verificó que era un fast-forward limpio (`main` ancestro directo de `HEAD`) y se corrigió: `git checkout main && git merge --ff-only a1402ea` (push resultó en "Everything up-to-date", confirmando que solo era un desajuste de la copia local, no una falta de push).

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 1 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today`, equivalente a 2026-11-20 casi cerrado en zona horaria de la cuenta):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🟢 GT \| Odoo \| CP \| Servicios | ACTIVE | $28.39 | 4,017 | 77 | 1.92% | 4 | $7.10 |
| 🟢 GT \| Beco \| CP \| Conjuntos | ACTIVE | $14.20 | 1,583 | 38 | 2.40% | 3 | **$4.73** |
| 🔴 COL \| Odoo \| CP \| Servicios | ACTIVE | $8.37 | 720 | 19 | 2.64% | 0 | — (sin leads) |
| 🔴 PY \| Odoo \| CP \| Servicios | ACTIVE | $8.23 | 1,101 | 19 | 1.73% | 0 | — (sin leads) |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $9.09 | 1,076 | 23 | 2.14% | 0 | — (sin leads) |
| 🔴 PY \| Beco \| CP \| Conjuntos | ACTIVE | $7.45 | 1,152 | 14 | 1.22% | 0 | — (sin leads) |
| 🔴 SLV \| Odoo \| CP \| Servicios | ACTIVE | $7.72 | 1,164 | 15 | 1.29% | 0 | — (sin leads) |
| ⚪ Evento: gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED** (13 campañas, sin cambios desde días anteriores): COL \| Beco \| CP \| Conjuntos, COL \| Odoo \| CP \| Servicios (versión de prueba anterior), 2x boosts de "Evento: Odoo en Acción", "[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia", "...[USA] - Toma El control de tu pyme", "...[GT] - Toma El control de tu pyme", Accurate Partners - Loyalti, "...[GT] - Odoo Test", "...[GT] - Beco", Conversión Clientes Potenciales MX/PY, "...[SV] - Pyme El Salvador", 🟡 Conversión - Clientes Potenciales.

`ads_account_get_activity_logs` para el rango 2026-11-20 06:00 – 2026-11-21 06:00 UTC **no devolvió ningún evento** (ni cambios manuales ni el cargo automático de facturación de Meta, que todavía no ocurre porque el día local no ha cerrado). No se ejecutó ningún cambio de presupuesto, targeting ni creativo hoy.

---

## 📊 Análisis e Insights

1. **El patrón de ayer (por línea de producto) se rompe hoy — ahora parece geográfico:** el 19-nov las 4 campañas de Odoo (GT/PY/SLV/COL) tenían leads y las 3 de Beco estaban en cero, dividido limpiamente por producto. Hoy es al revés: **las dos campañas de GT (Odoo y Beco) son las únicas con leads**, mientras que **las 5 campañas de PY, SLV y COL — sin importar si son Odoo o Beco — están simultáneamente en cero**. Esto sugiere que el problema (o la ventaja) puede estar más ligado a geografía que a línea de producto; merece revisión prioritaria, ya que afecta a 5 de 7 campañas activas en 3 países distintos el mismo día.
2. **GT \| Beco es la campaña con mejor CPL del día ($4.73, 3 leads)**, su mejor resultado desde que se empezó a documentar — rompe dos días consecutivos en cero leads (18 y 19-nov) y su peor CPL histórico ($15.43 el 18-nov).
3. **GT \| Odoo mantiene su recuperación:** 4 leads por segundo día consecutivo (igual que el 19-nov), aunque el CPL sube de $5.89 (final, 19-nov) a $7.10 hoy (+20.5%), posiblemente por el mayor gasto en la misma campaña ($23.55 → $28.39).
4. **Las 5 campañas restantes (COL \| Odoo, PY \| Odoo, SLV \| Beco, PY \| Beco, SLV \| Odoo) están todas en cero leads hoy**, el mayor número de campañas en cero visto hasta ahora en esta cuenta (vs. 3 el 19-nov, todas Beco). De estas, **SLV \| Beco es la que más gasta sin ningún lead ($9.09)**, seguida de COL \| Odoo ($8.37) y PY \| Odoo ($8.23).
5. **CPL blendeado empeora con fuerza:** 7 leads con $83.45 de gasto (provisional, faltan ~8 min de cierre) → CPL blendeado **$11.92**, +22.1% vs. los $9.76 (final) del 19-nov — revierte la mejora de los dos días anteriores y es el peor CPL blendeado desde el 18-nov ($11.24).
6. **Leads totales se mantienen en 7**, igual que ayer, pero mucho más concentrados: ayer repartidos entre 4 campañas, hoy concentrados en solo **2 campañas (ambas de GT)** — máxima concentración de riesgo geográfico vista hasta ahora.
7. **CTR blendeado retrocede a 1.90%** (provisional; vs. 2.03% final de ayer, -6.4%), aunque dentro del rango de variación diaria típica; sigue por debajo de la meta 3-4%. A nivel de campaña individual, COL \| Odoo (2.64%) y GT \| Beco (2.40%) tuvieron el mejor CTR del día pese a que COL \| Odoo no generó leads.
8. **Gasto total sube a $83.45** (provisional), +22.2% vs. los $68.30 finales de ayer, con casi todo el incremento concentrado en GT \| Odoo (+$4.84) y GT \| Beco (+$2.15 vs. su propio gasto de ayer).
9. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) en los ad sets analizados — la caída simultánea de PY/SLV/COL no tiene, por ahora, una causa técnica identificada por la herramienta.
10. **Campaña de evento sigue sin datos** ("Evento: gestión de nómina (Odoo)" ACTIVE, sin gasto/impresiones/clicks reportados por ~9º día consecutivo). `ads_get_errors` no devolvió ningún error de entrega bloqueante.
11. No hubo ninguna otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.
12. **Dato pendiente de cierre:** como se explica en la nota de advertencia arriba, los números de esta nota son provisionales (faltan ~8 minutos de cierre del día de la cuenta); se espera que una rutina posterior confirme o ajuste estas cifras con los datos finales, como ha ocurrido en días anteriores.

---

## ✏️ Cambios Realizados

Ninguno en Meta Ads. Solo se hizo lectura/análisis (`ads_get_ad_entities`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña desde esta rutina ni se detectaron cambios manuales en Ads Manager (sin eventos registrados en el log de actividad del día).

**Cambio técnico/de repositorio:** se corrigió el `HEAD` detached descrito en la nota de advertencia (fast-forward de `main` local a `a1402ea`, ya sincronizado con `origin/main`), dejando el repositorio alineado antes de crear esta nota.

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_entities` (nivel cuenta y campaña, `act_2530001557366648`) con `date_preset=today` y se verificó la zona horaria real de la cuenta (`timezone_name=America/Guatemala`) para confirmar a qué día calendario corresponde el dato.
- Se consultó el campo `lead` / `onsite_conversion_lead_grouped` directamente por campaña para confirmar que las 5 campañas sin leads reportan **cero leads reales** (campo ausente = 0), no un error o dato faltante de la API.
- Se consultó `ads_account_get_activity_logs` para el rango 2026-11-20 06:00 – 2026-11-21 06:00 UTC: sin resultados (ni cambios manuales ni facturación automática, consistente con que el día local aún no cerró).
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha.
- Se ejecutó `ads_get_errors` sobre la cuenta: sin errores bloqueantes de publicación o entrega.
- Se comparó campaña por campaña contra los datos finales verificados de [[Reports/2026-11-19 - Reporte Performance]] para identificar el cambio de patrón (producto → geografía) descrito en Insights.
- Se auditó `git status`/`git log`/`git branch -a`: se detectó y corrigió un `HEAD` detached 6 commits por detrás de `main`/`origin/main`, ya sincronizados entre sí (ver advertencia arriba); tras la corrección, repo limpio y alineado.
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen) | 2026-11-20 (provisional, ~8 min de cierre) | 2026-11-19 (final, verificado) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$11.92** | $9.76 | $6-7 | 🔴 Empeora fuerte (+22.1%), peor CPL desde el 18-nov |
| Gasto Total (lead-gen) | $83.45 | $68.30 | - | 🔴 +22.2% |
| Leads Totales | 7 | 7 | 4-5/día | 🟢 Igual que ayer, por encima de meta |
| CTR Promedio | 1.90% | 2.03% | 3-4% | 🔴 Retrocede (-6.4%), sigue bajo meta |
| Impresiones (lead-gen) | 10,813 | 9,740 | - | — |
| Clicks (lead-gen) | 205 | 198 | - | — |
| Campañas activas sin ningún lead | 5 (COL Odoo, PY Odoo, SLV Beco, PY Beco, SLV Odoo) | 3 (PY Beco, SLV Beco, GT Beco — todas Beco) | - | 🔴 Empeoró en cantidad; ahora cruza ambas líneas de producto |
| Mejor campaña del día | GT Beco ($4.73 CPL, 3 leads) | GT Odoo ($5.89 CPL, 4 leads) | - | — |
| Cambios de campaña ejecutados hoy | 0 | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] Confirmar al cierre formal del 2026-11-20 si el CPL ($11.92), el CTR (1.90%) y la concentración de leads en solo GT se mantienen con los números finales (misma verificación que rutinas anteriores: `date_preset=yesterday` + `time_range` explícito una vez cierre el día).
- [ ] **Nuevo — prioridad alta:** investigar por qué **PY, SLV y COL** quedaron simultáneamente en cero leads hoy, cruzando ambas líneas de producto (Odoo y Beco) — el patrón ya no parece ser por línea de producto (como se pensaba el 19-nov) sino geográfico; revisar si hay un factor común a esas 3 geografías (audiencia, puja, horario de entrega, o algo externo al creativo).
- [ ] Confirmar si la concentración de leads en **GT** (ambas campañas, Odoo y Beco) se sostiene mañana o fue un repunte puntual de un solo día.
- [ ] Revisar por qué el CPL de **GT \| Odoo** subió de $5.89 a $7.10 pese a mantener 4 leads — el mayor gasto ($28.39 vs $23.55) no se tradujo en más leads.
- [ ] Verificar en Ads Manager por qué "Evento: gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas (~9 días), aunque sin errores de entrega — confirmar `start_time`, presupuesto o calendario.
- [ ] Seguir trabajando el CTR blendeado (1.90% vs meta 3-4%) con pruebas A/B de creativo, priorizando evaluación por CTR antes de CPL.
- [ ] Pendiente heredado: decidir el futuro de las ~13 campañas históricas pausadas (Toma El control de tu pyme, Pyme Colombia, Pyme El Salvador, etc.) — reactivar, reemplazar formalmente o archivar.

---

## 🔗 Enlaces

- [[Daily notes/2026-11-20 - Resumen del Dia]] — nota del día anterior (documenta en realidad el 2026-11-19, final, por el mismo desajuste de zona horaria).
- [[Reports/2026-11-19 - Reporte Performance]] — reporte final y verificado del día usado como base de comparación en esta nota.
- [[Reports/2026-11-18 - Reporte Performance]] — reporte final y verificado de dos días atrás, para contexto adicional de tendencia.
- Tags: #daily-note #summary #meta-ads #octopus
