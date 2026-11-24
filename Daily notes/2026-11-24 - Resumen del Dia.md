---
date: 2026-11-24
aliases: [resumen-2026-11-24]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-11-24

> [!warning] Nota sobre la fecha y los datos (mismo desajuste de zona horaria de rutinas anteriores)
> Esta rutina se ejecutó a las **~05:51 UTC del 24-nov** (≈ 23:51 del 2026-11-23 en `America/Guatemala`, zona horaria de la cuenta `act_2530001557366648`). A esa hora el día local de la cuenta **todavía no cambiaba a 2026-11-24**: `date_preset=today` resolvió a **2026-11-23** (provisional, faltan ~9 minutos de cierre) y `date_preset=yesterday` resolvió a **2026-11-22** (final, ya publicado en [[Reports/2026-11-22 - Reporte Performance]]). Por lo tanto, los datos de "hoy" en esta nota corresponden en realidad al día **2026-11-23** (provisional) y la comparación es contra **2026-11-22** (final). Se mantiene el nombre de archivo `2026-11-24` siguiendo el mismo patrón de rutinas anteriores (fecha del sistema al momento de ejecutarse) — mismo desajuste ya documentado en las notas del 18 al 23-nov.
>
> **Verificación de drift de atribución tardía contra el reporte final del 22-nov:** al re-consultar `date_preset=yesterday` (2026-11-22) hoy, el gasto total sumó **$107.30** vs. $107.13 final reportado (+$0.17), impresiones 14,740 vs. 14,687 (+53); leads (22) y clicks (297) no cambiaron. Ajuste marginal (+0.16%), consistente con el patrón de días anteriores; no se corrige el reporte ya publicado del 22-nov.
>
> **Higiene de repositorio:** `git status` al iniciar mostró `main` limpio y sincronizado con `origin/main` (sin HEAD detached) — a diferencia de rutinas anteriores (20 al 23-nov), hoy no fue necesario corregir nada.

---

## 🎯 Campañas Revisadas

Se revisaron las 7 campañas activas de lead-gen + 2 de evento vía `ads_get_ad_entities` (nivel campaña, `date_preset=today` → día real 2026-11-23, provisional):

| Campaña | Status | Gasto | Impresiones | Clicks | CTR | Leads | CPL |
|---|---|---|---|---|---|---|---|
| 🔴 COL \| Odoo \| CP \| Servicios | ACTIVE | $9.88 | 944 | 26 | 2.75% | 0 | — (sin leads) |
| 🔴 PY \| Beco \| CP \| Conjuntos | ACTIVE | $7.62 | 1,297 | 18 | 1.39% | 0 | — (sin leads) |
| 🔴 PY \| Odoo \| CP \| Servicios | ACTIVE | $8.89 | 1,203 | 25 | 2.08% | 0 | — (sin leads) |
| 🔴 SLV \| Beco \| CP \| Conjuntos | ACTIVE | $8.05 | 1,335 | 29 | 2.17% | 0 | — (sin leads) |
| 🟢 SLV \| Odoo \| CP \| Servicios | ACTIVE | $9.18 | 1,280 | 37 | 2.89% | 2 | **$4.59** |
| 🔴 GT \| Beco \| CP \| Conjuntos | ACTIVE | $16.31 | 2,036 | 42 | 2.06% | 1 | $16.31 |
| 🟡 GT \| Odoo \| CP \| Servicios | ACTIVE | $34.15 | 4,633 | 95 | 2.05% | 4 | $8.54 |
| ⚪ Evento: El futuro de la gestión de nómina (Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $0.00 | 0 | 0 | — | n/a | n/a |
| 🆕 Evento: Cotiza en segundos y cierra ventas desde el celular (3 trucos en Odoo) | ACTIVE (EVENT_RESPONSES, no lead-gen) | $4.58 | 6,624 | 162 | 2.45% | n/a | n/a |

**Resto de la cuenta — todo PAUSED** (14 campañas, sin cambios desde días anteriores): COL \| Beco \| CP \| Conjuntos, COL \| Odoo \| CP \| Servicios (versión de prueba anterior), 2x boosts de "Evento: Odoo en Acción", "[2026-08][Lead Generation][Odoo][COL] - Pyme Colombia", "...[USA] - Toma El control de tu pyme", "...[GT] - Toma El control de tu pyme", Accurate Partners - Loyalti, "...[GT] - Odoo Test", "...[GT] - Beco", Conversión Clientes Potenciales MX/PY, "...[SV] - Pyme El Salvador", 🟡 Conversión - Clientes Potenciales.

**Acción manual detectada (fuera de esta rutina):** `ads_account_get_activity_logs` (rango 2026-11-23 06:00 – 2026-11-24 06:00 UTC) muestra que **Gabriel Calderon creó hoy a las 9:34–9:36 AM (hora de la cuenta), vía la app "Boosted Page" (boost de página/evento desde el móvil o Ads Manager), una nueva campaña-boost de evento**: "Evento: Cotiza en segundos y cierra ventas desde el celular: 3 trucos en Odoo para vender..." — segmentación Guatemala, 18+, Advantage+ audience activado, presupuesto total (lifetime budget) **$20.00 USD**, objetivo "Event response". El anuncio empezó a entregar a las 10:30 AM y ya acumuló $4.58 de gasto / 6,624 impresiones / 162 clicks / 2.45% CTR en su primer día — no es parte del set de lead-gen y no se compara contra la meta de CPL.

---

## 📊 Análisis e Insights

1. **Reversión fuerte del día: 4 de 7 campañas lead-gen caen a cero leads simultáneamente** (COL \| Odoo, PY \| Beco, PY \| Odoo, SLV \| Beco), subiendo de solo 1 campaña en cero (SLV \| Beco) en los dos días previos a 4 — y abarcando 3 países distintos (COL, PY, SLV) y ambas marcas (Odoo y Beco). Que el corte sea simultáneo y cruce países/marcas, no un patrón aislado de una sola campaña, apunta más a una causa compartida (formulario de leads, integración con CRM/webhook, tracking) que a problemas independientes de audiencia o puja en cada una.
2. **Leads totales se desploman a 7** (vs. 22 finales del 21-nov anterior/22-nov), -68.2%, el peor día del período registrado desde que se empezó a documentar mejora sostenida (18 al 22-nov). **CPL blendeado sube a ~$13.44** (vs. $4.87 final de ayer, +176%), muy por encima de la meta $6-7.
3. **El tráfico (impresiones, clicks, CTR) solo cae moderadamente, y el CTR incluso mejora:** impresiones 12,728 (-13.3% vs. 14,687), clicks 272 (-8.4% vs. 297), CTR blendeado ~2.14% (+5.9% vs. 2.02% final de ayer). Esto es clave: la caída está concentrada en la conversión a lead, no en la entrega ni en el interés del anuncio (el CTR sigue siendo de los mejores del período) — refuerza la hipótesis de un problema técnico de captura de leads (formulario, CRM, pixel) más que de fatiga de audiencia o creativo.
4. **Las recuperaciones reportadas el 21/22-nov no se sostuvieron:** PY \| Odoo (que había llegado a 5 leads/$2.08 CPL) y PY \| Beco (1 lead/$9.90 CPL) vuelven ambas a cero hoy; COL \| Odoo (2 leads/$5.19 ayer) también cae a cero. Solo SLV \| Beco mantiene su racha de cero (ya 5-6 días consecutivos).
5. **SLV \| Odoo es la única campaña que se mantiene estable y saludable:** 2 leads a **$4.59 CPL**, por debajo de la meta, mejor CPL del día — contrasta con el resto de la cuenta y sugiere que no es un problema de infraestructura 100% generalizado (si lo fuera, también afectaría a esta campaña), aunque sí reduce su volumen de leads (2 vs. 4 ayer).
6. **GT \| Odoo y GT \| Beco (las dos campañas de mayor gasto) absorben casi todos los leads del día (4 y 1) pero a CPL sobre meta:** GT \| Odoo $8.54 (vs. $5.47 final de ayer, +56%) y GT \| Beco **$16.31** (vs. $6.34 final de ayer, +157%, el peor CPL individual del período para esta campaña).
7. **`ads_insights_anomaly_signal` no detectó anomalías** (solapamiento de subasta, fatiga de creativo o audiencia estrecha) y `ads_get_errors` no devolvió errores de entrega/publicación bloqueantes — es decir, Meta no ve un problema de delivery, consistente con que el tráfico (impresiones/clicks/CTR) está en línea con días anteriores. Esto refuerza que, si hay un problema, está río abajo de Meta (formulario instantáneo, integración con CRM, confirmación de leads), fuera del alcance de estas herramientas de diagnóstico.
8. **Nueva campaña-boost de evento creada manualmente hoy** ("Cotiza en segundos...", ver sección de Campañas Revisadas) — es una acción del usuario fuera de esta rutina, no relacionada con la caída de leads de las campañas de Odoo/Beco.
9. **Campaña de evento "El futuro de la gestión de nómina" sigue sin datos** por ~14º día consecutivo (sin gasto/impresiones/clicks), sin errores de entrega bloqueantes detectados — pendiente de revisión manual directa, ahora con más urgencia dado el tiempo acumulado.
10. No hubo otra sesión de Claude Code activa en la cuenta hoy aparte de esta rutina, y no se realizó investigación externa de competencia o tendencias de mercado.
11. **Dato pendiente de cierre:** como se explica en la nota de advertencia arriba, los números de esta nota son provisionales (faltan ~9 minutos de cierre del día de la cuenta); se espera que una rutina posterior confirme estas cifras con los datos finales — dado lo marcado de la caída, es poco probable que el drift normal (+0.1-0.5%) cambie la conclusión.

---

## ✏️ Cambios Realizados

**Ninguno desde esta rutina** en las campañas lead-gen (solo lectura/análisis: `ads_get_ad_accounts`, `ads_get_ad_entities` con `date_preset=today` y `date_preset=yesterday`, `ads_account_get_activity_logs`, `ads_insights_anomaly_signal`, `ads_get_errors`); no se modificó presupuesto, targeting, copy ni creativo de ninguna campaña de lead-gen.

**Cambio detectado, realizado directamente en Meta por el usuario (no por esta rutina):** creación de la nueva campaña-boost de evento "Evento: Cotiza en segundos y cierra ventas desde el celular: 3 trucos en Odoo para vender..." (ver detalle arriba) — campaña, ad set y anuncio creados y activados entre las 9:34 AM y 10:30 AM de hoy vía la app "Boosted Page", presupuesto total $20.00 USD, ya entregando.

**Repositorio:** sin cambios de higiene necesarios hoy (rama `main` ya sincronizada con `origin/main` al iniciar).

---

## 🔬 Investigación Realizada

- Se consultó `ads_get_ad_accounts` para confirmar la cuenta activa de la plantilla (`act_2530001557366648`, "GT | Octopus Innovations") entre las 10 cuentas visibles para este usuario.
- Se consultó `ads_get_ad_entities` (nivel cuenta) para verificar la zona horaria real de la cuenta (`timezone_name=America/Guatemala`) junto con `date -u` / `TZ='America/Guatemala' date` del sistema, confirmando que "hoy" de la cuenta = 2026-11-23 (provisional, ~9 min de cierre).
- Se consultó `ads_get_ad_entities` (nivel campaña) con `date_preset=today` (→ 23-nov, provisional) y `date_preset=yesterday` (→ 22-nov) para las 7 campañas lead-gen activas más las 2 de evento.
- Se comparó `date_preset=yesterday` (22-nov) contra las cifras finales ya publicadas en [[Reports/2026-11-22 - Reporte Performance]] para detectar drift de atribución tardía (+$0.17 gasto, +53 impresiones, sin cambio en leads/clicks).
- Se consultó `ads_account_get_activity_logs` para el rango 2026-11-23 06:00 – 2026-11-24 06:00 UTC: se detectó la creación manual de la nueva campaña-boost de evento (ver arriba); sin otros cambios de presupuesto, targeting ni estado en las campañas de lead-gen.
- Se ejecutó `ads_insights_anomaly_signal` sobre la cuenta: sin anomalías de solapamiento de subasta, fatiga de creativo o audiencia estrecha, a pesar de la fuerte caída de leads observada.
- Se ejecutó `ads_get_errors` sobre la cuenta: sin errores bloqueantes de publicación o entrega.
- Se auditó `git status`: repo limpio y ya sincronizado con `origin/main`, sin necesidad de corrección.
- No se realizó investigación externa de competencia ni tendencias de mercado.

---

## 📊 Datos Clave del Día

| Métrica (blendeada, 7 campañas lead-gen) | 2026-11-23 (provisional, ~9 min de cierre) | 2026-11-22 (final, verificado) | Meta | Status |
|---|---|---|---|---|
| CPL Promedio | **$13.44** | $4.87 | $6-7 | 🔴 Empeora fuertemente (+176%), peor del período registrado |
| Gasto Total (lead-gen) | $94.08 | $107.13 | - | 🟡 -12.2%, menos gasto pero muchos menos leads |
| Leads Totales | **7** | 22 | 4-5/día | 🔴 -68.2%, peor día del período, aunque sigue dentro del rango histórico amplio |
| CTR Promedio | 2.14% | 2.02% | 3-4% | 🟢 Mejora (+5.9%), sigue bajo meta pero el tráfico no es el problema |
| Impresiones (lead-gen) | 12,728 | 14,687 | - | — |
| Clicks (lead-gen) | 272 | 297 | - | — |
| Campañas activas sin ningún lead | 4 (COL Odoo, PY Beco, PY Odoo, SLV Beco) | 1 (SLV Beco) | - | 🔴 Empeora fuertemente (de 1 a 4) |
| Mejor campaña del día | SLV Odoo ($4.59 CPL, 2 leads) | PY Odoo ($2.08 CPL, 5 leads) | - | — |
| Cambios de campaña lead-gen ejecutados hoy | 0 | 0 | - | — |
| Nuevas campañas creadas (fuera de lead-gen) | 1 (boost de evento, manual) | 0 | - | — |

---

## 📋 Proximas Acciones

- [ ] **Prioridad urgente:** investigar causa técnica compartida de la caída simultánea a cero leads en 4 campañas de 3 países distintos (COL \| Odoo, PY \| Beco, PY \| Odoo, SLV \| Beco) — revisar en Ads Manager / Meta Business Suite el estado del formulario instantáneo (Instant Forms), la integración con CRM/webhook y el pixel de leads, ya que el tráfico (CTR, clicks, impresiones) se mantuvo normal, lo que descarta un problema de entrega o fatiga de audiencia.
- [ ] Confirmar al cierre formal del 2026-11-23 si el CPL ($13.44) y el conteo de leads (7) se mantienen con los números finales, o si hay atribución tardía significativa — generar `Reports/2026-11-23 - Reporte Performance.md` una vez cierre el día.
- [ ] Revisar por qué **SLV \| Beco** sigue en cero leads (ya 5-6 días consecutivos, el más persistente de la cuenta) — evaluar audiencia, puja, horario de entrega u oferta frente a SLV \| Odoo (mismo país, única que sí convierte hoy).
- [ ] Verificar si la caída de **GT \| Beco** a $16.31 CPL (1 lead) es puntual o el inicio de una tendencia, dado que es el peor CPL individual del período para esta campaña.
- [ ] Confirmar con el usuario el objetivo y seguimiento de la nueva campaña-boost de evento "Cotiza en segundos..." (creada hoy manualmente, $20 USD lifetime budget) — no requiere acción de esta rutina, pero conviene documentarla en Campaigns/ si se espera que continúe.
- [ ] Verificar en Ads Manager por qué "Evento: El futuro de la gestión de nómina (Odoo)" sigue sin reportar gasto ni métricas (~14 días) — confirmar `start_time`, presupuesto o calendario.
- [ ] Seguir trabajando el CTR blendeado (2.14% vs meta 3-4%) con pruebas A/B de creativo, aunque hoy no es la causa principal del mal resultado.
- [ ] Pendiente heredado: decidir el futuro de las ~14 campañas históricas pausadas (Toma El control de tu pyme, Pyme Colombia, Pyme El Salvador, etc.) — reactivar, reemplazar formalmente o archivar.

---

## 🔗 Enlaces

- [[Reports/2026-11-22 - Reporte Performance]] — reporte final y verificado del día usado como base de comparación en esta nota.
- [[Daily notes/2026-11-23 - Resumen del Dia]] — nota del día anterior.
- [[Reports/2026-11-21 - Reporte Performance]] — reporte final de dos días atrás, para contexto adicional de tendencia.
- Tags: #daily-note #summary #meta-ads #octopus
