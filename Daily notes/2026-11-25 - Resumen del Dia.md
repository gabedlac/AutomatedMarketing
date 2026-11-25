---
date: 2026-11-25
aliases: [resumen-2026-11-25]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-25

> [!warning] Nota sobre la fecha y los datos (mismo desajuste de zona horaria de rutinas anteriores, 18 al 24-nov)
> Esta rutina se ejecutó a las **~05:51 UTC del 25-nov** (≈ 23:51 del 2026-11-24 en `America/Guatemala`, zona horaria de la cuenta `act_2530001557366648`). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-25**: `date_preset=today` resolvió a **2026-11-24** (provisional, faltan ~9 minutos de cierre) y `date_preset=yesterday` resolvió a **2026-11-23** (final). Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-24** (provisional) y la comparación es contra **2026-11-23** (final, ya publicado en [[Reports/2026-11-23 - Reporte Performance]]). Se mantiene el nombre de archivo `2026-11-25` siguiendo el mismo patrón de rutinas anteriores (fecha del sistema al momento de ejecutarse).
>
> **Verificación contra el reporte final del 23-nov:** al re-consultar `date_preset=yesterday` (2026-11-23) hoy, el gasto lead-gen (7 campañas) sumó **$95.49** vs. el valor usado en el reporte final publicado; leads (7) coinciden exactamente. Consistente con el patrón de drift marginal de días anteriores; no se corrige el reporte ya publicado.
>
> **Higiene de repositorio (hallazgo de hoy):** `git status` al iniciar mostró `HEAD` **detached**, 2 commits por detrás de `main`/`origin/main` (`118c36d` "Add Daily Summary - 2026-11-24" y `6a203d0` "Add Daily Performance Report - 2026-11-23"). Se verificó la cadena de commits: ambos eran continuación lineal (fast-forward limpio) del `main` local, y `git push` confirmó que **`origin/main` ya tenía ambos commits** ("Everything up-to-date") — es decir, **no hubo pérdida de datos**, solo la rama local `main` y `HEAD` habían quedado desincronizados de una rutina anterior. Se corrigió con `git checkout main && git merge --ff-only origin/main` (fast-forward) antes de generar esta nota. Este problema se repite rutina tras rutina desde el 20-nov (ver nota 10 en [[Reports/2026-11-23 - Reporte Performance]]); sigue sin resolverse la causa raíz.

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 2 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today` → día real 2026-11-24, provisional, ~9 min de cierre restantes):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🔴 COL \| Odoo \| CP \| Servicios | ACTIVE | $7.59 | 615 | 10 | 1.63% | 0 | — (sin leads) |
| 🔴 PY \| Beco \| CP \| Conjuntos | ACTIVE | $8.55 | 1,408 | 19 | 1.35% | 0 | — (sin leads) |
| 🟡 PY \| Odoo \| CP \| Servicios | ACTIVE | $8.06 | 1,312 | 18 | 1.37% | 1 | $8.06 |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $7.10 | 1,091 | 14 | 1.28% | 0 | — (sin leads) |
| 🔴 SLV \| Odoo \| CP \| Servicios | ACTIVE | $6.40 | 823 | 17 | 2.07% | 0 | — (sin leads) |
| 🔴 GT \| Beco \| CP \| Conjuntos | ACTIVE | $13.54 | 1,715 | 42 | 2.45% | 1 | $13.54 |
| 🟢 GT \| Odoo \| CP \| Servicios | ACTIVE | $24.89 | 3,436 | 85 | 2.47% | 4 | **$6.22** |
| ⚪ Evento: Cotiza en segundos y cierra ventas desde el celular (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $6.85 | 9,849 | 227 | 2.30% | n/a | n/a |
| ⚪ Evento: El futuro de la gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |

**Resto de la cuenta — todo PAUSED** (14 campañas, sin cambios desde días anteriores).

**Cambios manuales en Meta hoy:** ninguno detectado — `ads_account_get_activity_logs` (rango 2026-11-24 06:00 – 2026-11-25 06:00 UTC, día completo de la cuenta) devolvió un array vacío, sin cambios de presupuesto, targeting, estado ni nuevas campañas.

---

## 📊 Análisis e Insights

1. **SLV \| Odoo, la campaña más estable y saludable de los últimos días, cae a cero leads hoy** — con ella, ya son **4 de 7 campañas lead-gen en cero simultáneamente** (COL Odoo, PY Beco, SLV Beco, SLV Odoo), igual que ayer pero con una composición distinta y más preocupante: la única campaña que venía sosteniéndose dentro de meta deja de convertir.
2. **GT \| Odoo es hoy la única campaña dentro de la meta de CPL ($6-7)**: $6.22 CPL con 4 de los 6 leads totales del día (66.7%) — la cuenta depende casi por completo de esta sola campaña.
3. **PY \| Odoo se recupera parcialmente** (0 leads ayer → 1 lead hoy, $8.06 CPL) — sigue sobre meta pero rompe su racha de ceros.
4. **El CPL blendeado mejora levemente vs. ayer** ($12.69 vs. $13.64, -7.0%) pero sigue muy por encima de la meta $6-7 — la mejora viene de menor gasto (-20.3%) y una caída de leads algo más suave (-14.3%), no de una recuperación real en conversión.
5. **El tráfico se contrae de forma generalizada:** impresiones -19.4% (10,400 vs. 12,906), clicks -24.6% (205 vs. 272), CTR -6.6% (1.97% vs. 2.11%) — a diferencia del 23-nov, donde el CTR se mantenía fuerte mientras los leads caían, hoy también se suaviza la entrega, aunque dentro del rango reciente y todavía lejos de la meta 3-4%.
6. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) y `ads_get_errors` no devolvió errores de entrega/publicación bloqueantes — igual que ayer, lo que sigue apuntando a una causa río abajo de Meta (formulario, CRM/webhook, pixel) y no a un problema de delivery, consistente con la acción urgente pendiente desde el 24-nov.
7. **SLV \| Beco completa una racha extendida en cero leads** (~6-7 días consecutivos), la más persistente de la cuenta.
8. **Evento "El futuro de la gestión de nómina"** sigue sin gasto/impresiones por ~15º día consecutivo.
9. No hubo otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.
10. **Dato pendiente de cierre:** como se explica en la nota de advertencia arriba, los números de "hoy" (2026-11-24) son provisionales (faltan ~9 minutos de cierre del día de la cuenta); se espera que la rutina de reporte final confirme estas cifras.

---

## ✏️ Cambios Realizados

**Ninguno desde esta rutina** en las campañas lead-gen (solo lectura/análisis: `ads_get_ad_entities` con `date_preset=today` y `date_preset=yesterday`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña.

**Ningún cambio manual detectado en Meta hoy** (ver sección de Campañas Revisadas).

**Repositorio:** se corrigió un desajuste de `HEAD`/`main` local heredado de una rutina anterior (ver nota de advertencia arriba) — `git checkout main && git merge --ff-only origin/main`, sin pérdida de datos ya que `origin/main` tenía los commits correctos.

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_entities` (nivel cuenta) para confirmar la zona horaria real de la cuenta (`timezone_name=America/Guatemala`) junto con `date -u` del sistema, confirmando que "hoy" de la cuenta = 2026-11-24 (provisional, ~9 min de cierre).
- Se consultó `ads_get_ad_entities` (nivel campaña) con `date_preset=today` (→ 24-nov, provisional) y `date_preset=yesterday` (→ 23-nov, final) para las 7 campañas lead-gen activas más las 2 de evento.
- Se comparó `date_preset=yesterday` (23-nov) contra las cifras ya publicadas en [[Reports/2026-11-23 - Reporte Performance]], confirmando consistencia (leads idénticos, gasto con drift marginal esperado).
- Se consultó `ads_account_get_activity_logs` para el rango 2026-11-24 06:00 – 2026-11-25 06:00 UTC (día completo de la cuenta): sin resultados, ningún cambio manual.
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha.
- Se ejecutó `ads_get_errors` sobre la cuenta: sin errores bloqueantes de publicación o entrega.
- Se auditó `git status`/`git log`: se detectó `HEAD` detached y `main` local desincronizado; se verificó la cadena de commits y se corrigió con fast-forward (ver nota de advertencia e insight 6 arriba).
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen) | 2026-11-24 (provisional, ~9 min de cierre) | 2026-11-23 (final, verificado) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$12.69** | $13.64 | $6-7 | 🟡 Mejora (-7.0%) pero sigue muy sobre meta |
| Gasto Total (lead-gen) | $76.13 | $95.49 | - | 🟡 -20.3% |
| Leads Totales | 6 | 7 | 4-5/día | 🟡 -14.3%, dentro del rango histórico amplio |
| CTR Promedio | 1.97% | 2.11% | 3-4% | 🔴 Empeora (-6.6%), sigue bajo meta |
| Impresiones (lead-gen) | 10,400 | 12,906 | - | — |
| Clicks (lead-gen) | 205 | 272 | - | — |
| Campañas activas sin ningún lead | 4 (COL Odoo, PY Beco, SLV Beco, SLV Odoo) | 4 (COL Odoo, PY Beco, PY Odoo, SLV Beco) | - | 🟡 Igual cantidad, pero SLV Odoo cae y PY Odoo se recupera |
| Mejor campaña del día | GT Odoo ($6.22 CPL, 4 leads) | SLV Odoo ($4.62 CPL, 2 leads) | - | — |
| Cambios de campaña ejecutados hoy | 0 | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] **Prioridad urgente (heredada del 24-nov, sigue sin resolver):** investigar la causa técnica compartida de la caída a cero leads que ya afecta a 4 campañas en días consecutivos — revisar formulario instantáneo (Instant Forms), integración CRM/webhook y pixel de leads, dado que Meta no reporta errores de delivery ni anomalías.
- [ ] Monitorear si **SLV \| Odoo** (hoy en cero por primera vez en el período reciente) recupera leads mañana o se suma de forma sostenida a la lista de campañas en cero.
- [ ] Confirmar al cierre formal del 2026-11-24 si el CPL ($12.69) y el conteo de leads (6) se mantienen, o si hay atribución tardía significativa — generar `Reports/2026-11-24 - Reporte Performance.md` una vez cierre el día.
- [ ] Revisar por qué **SLV \| Beco** sigue en cero leads (~6-7 días consecutivos, el más persistente de la cuenta).
- [ ] Verificar en Ads Manager por qué "Evento: El futuro de la gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas (~15 días) — confirmar `start_time`, presupuesto o calendario.
- [ ] Seguir trabajando el CTR blendeado (1.97% vs meta 3-4%) con pruebas A/B de creativo.
- [ ] Pendiente heredado: decidir el futuro de las ~14 campañas históricas pausadas.
- [ ] **Investigar y resolver de raíz** por qué la rama local `main`/`HEAD` queda desincronizada entre rutinas (se repite desde el 20-nov) — considerar que cada rutina empiece siempre con `git fetch && git checkout main && git merge --ff-only origin/main` antes de crear archivos, para evitar que vuelva a quedar un commit huérfano sin verificar contra `origin`.

---

## 🔗 Enlaces

- [[Reports/2026-11-23 - Reporte Performance]] — reporte final y verificado del día anterior, usado como base de comparación en esta nota.
- [[Daily notes/2026-11-24 - Resumen del Dia]] — nota del día anterior.
- Tags: #daily-note #summary #meta-ads #octopus
