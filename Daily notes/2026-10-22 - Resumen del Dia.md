---
date: 2026-10-22
aliases: [resumen-2026-10-22]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-10-22

> [!warning] 41ª vez consecutiva que la rutina se dispara antes de medianoche Guatemala
> Al momento del pull (2026-10-22 05:51 UTC = **2026-10-21 23:51 hora de Guatemala, GMT-6**), el día calendario 2026-10-22 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-10-21** (a ~9 min de su cierre real). Esta nota documenta esa lectura casi-final de 2026-10-21. Se confirmó vía `get_trigger` que el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde su creación el 2026-08-28 — **41ª ocurrencia consecutiva documentada** (`next_run_at` ya programado para 2026-10-23T05:50:00Z, mismo patrón). Solo el usuario puede corregirlo desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ.

> [!danger] Expansión repentina a Colombia y El Salvador: 4 campañas nuevas, gasto del día casi se triplica
> Entre las 14:05 y 14:15 GT, **Sebas Tenjo** clonó la plantilla "Advantage+ Sugerencias" (estrenada en GT el 10-19) y lanzó **4 campañas nuevas** en dos mercados sin antecedentes recientes en esta cuenta: "SLV \| Odoo \| CP \| Servicios", "SLV \| Beco \| CP \| Conjuntos", "COL \| Odoo \| CP \| Servicios" y "COL \| Beco \| CP \| Conjuntos" (una de ellas, la de Beco en SLV, se creó literalmente como copia con el sufijo "- Copia" y fue renombrada al instante). Esto añade **$64/día de presupuesto nuevo comprometido** (7 ad sets a $8/día) y el gasto total de cuenta del día salta a **~$86.50**, el más alto documentado en esta serie (vs. $25-32 en días previos). Ver detalle en [[#✏️ Cambios Realizados]].

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-10-21** (a ~9 minutos del cierre real, horario de cuenta GMT-6):

| Campaña | Status | Gasto (parcial) | Leads | CPL | CTR | Emoji |
|---------|--------|------------------|-------|-----|-----|-------|
| GT \| Odoo \| CP \| Servicios | ACTIVE | $22.93 | 4 | $5.73 🟢 | 1.26% 🔴 | 🟢🔴 |
| GT \| Beco \| CP \| Conjuntos | ACTIVE | $9.60 | 1 | $9.60 🔴 | 2.21% 🟡 | 🔴🟡 |
| 🆕 COL \| Odoo \| CP \| Servicios (nueva, 14:12) | ACTIVE | $20.12 | 2 | $10.06 🔴 | 1.44% 🟡 | 🆕🔴 |
| 🆕 SLV \| Odoo \| CP \| Servicios (nueva, 14:05) | ACTIVE | $15.12 | 1 | $15.12 🔴 | 0.92% 🔴 | 🆕🔴 |
| 🆕 COL \| Beco \| CP \| Conjuntos (nueva, 14:15) | ACTIVE | $7.14 | 0 (en este pull) | N/A 🟡 | 2.13% 🟡 | 🆕🟡 |
| 🆕 SLV \| Beco \| CP \| Conjuntos (nueva, 14:08) | ACTIVE | $5.53 | 0 (en este pull) | N/A 🟡 | 2.67% 🟢 | 🆕🟡 |
| Evento: Odoo en Acción (boost relanzado, $20 lifetime) | ACTIVE | $6.06 | 57 RSVP (ver nota) | $0.11/RSVP 🟢 | 2.58% 🟢 | 🟢 |
| Evento: Odoo en Acción (boost original, 10-13→10-15) | COMPLETED, sin cambios | $0.00 | - | - | - | 🏁 |
| Beco (GT, campaña original) | PAUSED, sin cambios (pausada 10-19) | $0.00 | - | - | - | ⏸️ |
| Toma El control de tu pyme (GT) | PAUSED, sin cambios (pausada 10-19) | $0.00 | - | - | - | ⏸️ |
| Pyme El Salvador (SV, campaña legacy no relacionada) | PAUSED, sin cambios | $0.00 | - | - | - | ⏸️ |
| Odoo Test (GT) | PAUSED, sin cambios (pausada 10-19) | $0.00 | - | - | - | ⏸️ |
| Pyme Colombia (COL, campaña legacy no relacionada) | PAUSED, sin cambios (varios días) | $0.00 | - | - | - | ⏸️ |
| Toma El control de tu pyme (USA) | PAUSED, sin cambios | $0.00 | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED, sin cambios | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX / PY | PAUSED, sin cambios | $0.00 | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED, sin cambios | $0.00 | - | - | - | ⏸️ |

**Nota importante:** todos los cambios documentados hoy fueron realizados directamente en Meta Ads Manager (Power Editor) por el equipo — ninguno fue ejecutado por esta rutina automatizada, que solo lee métricas y activity log.

### 🆕🔴 Expansión a Colombia y El Salvador: misma plantilla, 4 campañas, 7 ad sets

A las 14:05, 14:08, 14:12 y 14:15 GT, Sebas Tenjo creó en rápida sucesión (10 minutos totales) las 4 campañas nuevas listadas arriba vía Power Editor. Cada una replica exactamente la estructura "CP | Advantage + Sugerencias" estrenada en GT:
- **"SLV | Odoo | CP | Servicios"** y **"COL | Odoo | CP | Servicios"**: 3 ad sets cada una ("Odoo Ecom", "Odoo Clínica", "Odoo Para Todos"), mismos públicos de interés que la versión GT (triangulación de envíos/e-commerce; odontología/clínicas; público general), $8/día por ad set, objetivo "Conversion leads", puja "Automatically bid for actions", Advantage+ audience activado. Targeting geográfico: El Salvador (país completo) y Colombia (ciudades de 1-3M+ habitantes) respectivamente.
- **"SLV | Beco | CP | Conjuntos"** y **"COL | Beco | CP | Conjuntos"**: 1 ad set cada una ("CP | Advantage + Sugerencias | Beco"), mismo público inmobiliario que la versión GT, $8/día, mismo objetivo y puja.
- La campaña de Beco en SLV se creó literalmente como copia (nombre inicial "SLV | Beco | CP | Conjuntos - Copia") y fue renombrada al instante — evidencia de que el equipo duplicó plantillas existentes en vez de construir desde cero.

En sus primeras ~9-10 horas: COL Odoo ya registra 2 leads (CPL $10.06), SLV Odoo 1 lead (CPL $15.12); ninguna de las dos campañas de Beco (COL/SLV) muestra leads confirmados todavía en este pull cercano al cierre — podría ser rezago de atribución de formularios, como ya se vio en lanzamientos anteriores (ver [[#📊 Análisis e Insights]]).

### 🔴 "GT | Beco | CP | Conjuntos" y las nuevas campañas de Beco (COL/SLV) muestran el CPL más alto de la cuenta

Beco GT cierra con CPL $9.60 (1 lead) y las dos campañas nuevas de Beco todavía no confirman leads — en conjunto, la línea de producto "Beco/Conjuntos" sigue siendo la más débil de la expansión del día, frente a "Odoo/Servicios" que ya tiene leads confirmados en los 3 mercados activos (GT, COL, SLV).

### 🟢 "GT | Odoo | CP | Servicios" mantiene el mejor CPL de lead-gen de la cuenta

$5.73 CPL (4 leads, $22.93 de gasto) — dentro/cerca de la meta de $6-7 fijada en [[CLAUDE.md]], y el único resultado de lead-gen con status 🟢 hoy, aunque el CTR (1.26%) sigue por debajo de la meta de 3-4%.

### ⏸️ Ciclo de pausa/reactivación en GT a primera hora del día (antes de la expansión)

A las 00:15 GT, el actor **Juan Tamayo** puso en "Pending Process" los 4 ad sets activos de GT (Beco, Odoo Clínica, Odoo Ecom, Odoo Para Todos) y amplió su targeting geográfico de "Guatemala: All Cities" a "Guatemala" (sin restricción de ciudad). A las 7:16-7:17 AM, **Sebas Tenjo** los reactivó, conservando el cambio de targeting. Ningún otro ajuste de presupuesto o creativo acompañó este ciclo. No hay evidencia de impacto negativo visible en el CPL de GT Odoo Servicios tras la reactivación.

### 🟢 Boost "Evento: Odoo en Acción" sigue siendo el mejor performer de la cuenta — cierra mañana

$6.06 de gasto hoy, CTR 2.58%, CPC ~$0.03. El campo de resultados del pull de hoy muestra 57 RSVP con costo por resultado $0.11/RSVP — **cifra menor a los 75 RSVP acumulados reportados en el cierre confirmado de 10-20**, lo que sugiere que el `results` de este pull podría estar reflejando solo una ventana parcial en vez del acumulado lifetime; **no tratar como una caída real de RSVPs sin confirmar con el reporte formal de mañana**. El boost cierra su presupuesto lifetime ($20) el 2026-10-22 a las 11:24 AM hora de cuenta.

---

## 📊 Análisis e Insights

- **Expansión geográfica no documentada previamente en [[CLAUDE.md]]**: el proyecto solo listaba la cuenta GT como activa; hoy el equipo comprometió $64/día adicionales en Colombia y El Salvador sin que este repositorio reflejara ese plan. Vale la pena confirmar con el equipo si esta expansión es intencional y sostenida, o una prueba de corta duración.
- **Patrón de clonado rápido**: las 4 campañas nuevas se crearon en 10 minutos reutilizando la estructura "Advantage+ Sugerencias" de GT (mismos ad sets, públicos, presupuesto por ad set y objetivo) — el equipo ya trata esta plantilla como su playbook estándar para abrir nuevos mercados, confirmando la tendencia apuntada en la nota del 10-21.
- **"Odoo/Servicios" funciona mejor que "Beco/Conjuntos" en todos los mercados activos hoy**: Odoo ya tiene leads confirmados en GT, COL y SLV; Beco solo los tiene en GT. Es consistente con el historial de la cuenta, donde Beco ha mostrado más episodios de "pico y reversión" que Odoo.
- **0 leads confirmados en las 2 campañas nuevas de Beco (COL, SLV)**: dado que son el día de lanzamiento y el pull es casi al cierre, es pronto para alarmarse — mismo patrón que se vio con "GT | Beco | CP | Conjuntos" en su primer día parcial (10-20), donde tampoco había leads en el pull nocturno pero sí terminó con 1 lead confirmado.
- **Posible discrepancia en el contador de RSVP del boost de evento** (57 en este pull vs. 75 acumulados reportados el 10-20) — pendiente de confirmar si es un artefacto del pull parcial o un cambio real en cómo se está reportando el acumulado lifetime.
- **Ciclo de pausa/reactivación de madrugada (Juan Tamayo → Sebas Tenjo) en GT** no parece haber afectado negativamente el CPL de Odoo Servicios, que de hecho mejora levemente vs. el día anterior.
- **Comparación vs. 2026-10-20 (cierre confirmado)**: gasto de lead-gen sube de $25.00 a $80.44 (+222%), impulsado casi en su totalidad por las 4 campañas nuevas; CTR blendeado de lead-gen prácticamente plano (1.34% hoy vs. 1.38% el 10-20 confirmado).

---

## ✏️ Cambios Realizados

**Todos los cambios siguientes se identificaron en el activity log de la cuenta (ventana 2026-10-21 00:00–23:51 hora GT) — fueron ejecutados por el equipo directamente en Meta Ads Manager (Power Editor), no por esta sesión automatizada:**

- **00:15 GT — Juan Tamayo** puso en pausa ("Pending Process") los 4 ad sets activos de GT (Beco, Odoo Clínica, Odoo Ecom, Odoo Para Todos) y amplió su targeting de "Guatemala: All Cities" a "Guatemala".
- **7:16-7:17 AM GT — Sebas Tenjo** reactivó ("Active") los mismos 4 ad sets de GT, conservando el targeting ampliado.
- **14:05 GT — Sebas Tenjo** creó la campaña **"SLV | Odoo | CP | Servicios"** con 3 ad sets ("Odoo Ecom", "Odoo Clínica", "Odoo Para Todos"), targeting El Salvador, $8/día cada uno, objetivo Conversion leads.
- **14:08 GT — Sebas Tenjo** creó la campaña **"SLV | Beco | CP | Conjuntos"** (inicialmente nombrada "- Copia" y renombrada en el acto) con el ad set "CP | Advantage + Sugerencias | Beco", targeting El Salvador, $8/día.
- **14:12 GT — Sebas Tenjo** creó la campaña **"COL | Odoo | CP | Servicios"** con 3 ad sets equivalentes, targeting Colombia (ciudades 1-3M+ hab.), $8/día cada uno.
- **14:15 GT — Sebas Tenjo** creó la campaña **"COL | Beco | CP | Conjuntos"** con el ad set "CP | Advantage + Sugerencias | Beco", targeting Colombia, $8/día.
- **14:05-14:15 GT — Sebas Tenjo** creó ~30 anuncios nuevos repartidos entre los 7 ad sets nuevos (variaciones de "Odoo | Negocio", "Odoo | Clínica", "Odoo | Para todos" y "Beco | Inmobiliario").

---

## 🔬 Investigación Realizada

- Se revisaron las 17 campañas de la cuenta a nivel campaña con `date_preset=today` (equivalente a 2026-10-21 en horario de cuenta), incluyendo gasto, leads, CPL, CTR, CPC, CPM, impresiones, clicks, reach y estado.
- Se revisó el activity log completo de la cuenta para la ventana 2026-10-21 00:00–23:51 GT (dos llamadas: 00:00-17:58 y 17:58-23:51, ~250+ eventos combinados), filtrando por categoría `campaign` y `ad_set` para aislar los cambios reales de los ~150 eventos de ruido tipo "Ad delivered"/"Ad status updated" generados automáticamente por Meta durante el rollout de los anuncios nuevos.
- Se confirmó el estado del trigger automatizado "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`) vía `get_trigger`: sigue en `50 5 * * *` UTC sin cambios desde su creación el 2026-08-28 — 41ª ocurrencia consecutiva del bug de zona horaria.
- Se identificaron los actores de cada cambio (Sebas Tenjo para toda la expansión y creación de campañas/anuncios; Juan Tamayo para el ciclo de pausa de madrugada en GT) vía `actor_name` del activity log.
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## 📊 Datos Clave del Día

| Métrica | 2026-10-21 (casi-final, parcial por rezago de atribución) | 2026-10-20 (cierre confirmado, [[Reports/2026-10-20 - Reporte Performance]]) | Variación |
|---------|-------------------------------------------------------------|-------------------------------------------------------------------------------|-----------|
| Gasto lead-gen (6 campañas activas: GT, COL, SLV x2) | $80.44 | $25.00 | 🔴 +222% |
| Leads confirmados (en el pull) | 8 (GT Odoo 4, GT Beco 1, COL Odoo 2, SLV Odoo 1) | 0 | 🟢 +8 (pendiente confirmar cierre) |
| CPL Promedio (blendeado, solo campañas con leads) | $10.06 | N/A (0 leads) | — |
| CTR Promedio (lead-gen, blendeado) | 1.34% | 1.38% | 🔴 -2.9% |
| Gasto boost evento | $6.06 | $7.16 | 🟢 -15.4% |
| RSVPs del boost evento (cifra del pull, ver nota de ambigüedad) | 57 | 75 (acumulado reportado) | — (posible artefacto del pull) |
| Gasto total de cuenta (incl. boost) | ~$86.50 | $32.16 | 🔴 +169% |
| Campañas nuevas del día | 4 (SLV Odoo, SLV Beco, COL Odoo, COL Beco) | 1 (GT Beco Conjuntos) | — |
| Mejor señal del día | GT Odoo Servicios: CPL $5.73, dentro de meta | GT Odoo Servicios: CPL N/A (0 leads) | 🟢 |
| Peor señal del día | COL Beco y SLV Beco: 0 leads confirmados en el pull, $12.67 combinados | Cuenta completa: 0 leads, $25.00 de gasto | Pendiente de confirmar si es rezago o real |

**Nota:** estas cifras de leads y RSVP son la lectura más incierta del día — a diferencia de un cierre confirmado, no hay certeza de si reflejan el resultado final o un rezago de atribución/reporte parcial. Confirmar con el Reporte Performance formal de hoy (~7 AM GT) antes de tratar estas cifras como definitivas, especialmente el gasto total de cuenta y el conteo de RSVP del boost de evento.

---

## 📋 Próximas Acciones

- [ ] **Confirmar con el equipo (Gabriel Calderón / Sebas Tenjo) si la expansión a Colombia y El Salvador es una decisión estratégica sostenida** o una prueba de corta duración — y actualizar [[CLAUDE.md]] con la nueva estructura de cuentas/mercados si es permanente.
- [ ] **Confirmar con el Reporte Performance formal de hoy (~7 AM GT) el cierre real de 2026-10-21**, en particular si "COL | Beco | CP | Conjuntos" y "SLV | Beco | CP | Conjuntos" terminaron el día en 0 leads o fue rezago de atribución.
- [ ] **Monitorear de cerca el CPL de las 4 campañas nuevas durante sus primeros 3-5 días** (meta: $6-7) antes de decidir si se mantienen, se ajustan o se pausan — especialmente Beco en ambos mercados nuevos, que no muestra leads todavía.
- [ ] **Aclarar la discrepancia del contador de RSVP del boost de evento** (57 vs. 75 acumulados) con el próximo pull antes de reportarlo como una caída real.
- [ ] **Investigar el ciclo de pausa/reactivación de madrugada en GT (Juan Tamayo → Sebas Tenjo)** — confirmar si fue una prueba intencional de ampliar el targeting de ciudad o un ajuste accidental.
- [ ] **Decidir el futuro de las campañas legacy pausadas** (Toma El control GT/USA, Beco original, Pyme El Salvador legacy, Odoo Test, Pyme Colombia legacy): varias llevan semanas sin actividad ni decisión, y ahora coexisten con campañas nuevas de nombre similar en los mismos mercados (Beco/Colombia, Beco/El Salvador).
- [ ] **Lanzar el A/B testing de los 5 copys** documentado en [[CLAUDE.md]] (pendiente desde 2026-08-24).
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` sigue disparándose a las 23:50 GT en vez de después de medianoche (41ª ocurrencia consecutiva) — solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ.

---

## 🔗 Enlaces

- [[Reports/2026-10-20 - Reporte Performance]] — último reporte de cierre confirmado disponible (el de 2026-10-21 se genera hoy ~7 AM GT)
- [[Daily notes/2026-10-21 - Resumen del Dia]] — resumen del día anterior
- Tags: #daily-note #summary #meta-ads #octopus
