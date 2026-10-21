---
date: 2026-10-21
aliases: [resumen-2026-10-21]
tags: [daily-note, summary, meta-ads, octopus]
---

# Resumen del Dia - 2026-10-21

> [!warning] 40ª vez consecutiva que la rutina se dispara antes de medianoche Guatemala
> Al momento del pull (2026-10-21 05:52 UTC = **2026-10-20 23:52 hora de Guatemala, GMT-6**), el día calendario 2026-10-21 **todavía no ha comenzado** en la zona horaria de la cuenta Meta Ads. La métrica `date_preset=today` de la API corresponde en realidad a **2026-10-20** (a ~8 min de su cierre real). Esta nota documenta esa lectura casi-final de 2026-10-20. Se confirmó vía `get_trigger` que el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` ("Daily Summary - 11:50 PM Guatemala") sigue en `50 5 * * *` UTC (23:50 GT), sin cambios desde su creación el 2026-08-28 — **40ª ocurrencia consecutiva documentada** (`next_run_at` ya programado para 2026-10-22T05:50:00Z, mismo patrón). Solo el usuario puede corregirlo desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ.

> [!info] Sebas Tenjo sigue escalando la reestructuración del 10-19: 3ª audiencia en Odoo y relanzamiento de Beco
> Tras el giro positivo del 10-19 (pausa de 4 campañas en crisis + lanzamiento de "GT \| Odoo \| CP \| Servicios"), hoy **Sebas Tenjo** amplió esa misma campaña con una tercera audiencia ("Odoo Para Todos") y 2 anuncios adicionales, y **relanzó Beco** bajo una campaña nueva con audiencia distinta ("Conjuntos" en vez de "Administradores e Inmobiliarias"). El gasto combinado de ambas campañas de lead-gen activas hoy ($24.78) **no muestra leads confirmados** en este pull cercano al cierre — a diferencia de ayer, cuando un pull similar sí reportó leads. Ver detalle en [[#✏️ Cambios Realizados]] y [[#📊 Análisis e Insights]].

---

## 🎯 Campañas Revisadas

Lectura casi-final de **2026-10-20** (a ~8 minutos del cierre real, horario de cuenta GMT-6):

| Campaña | Status | Gasto (parcial) | Leads/Resultados | CPL/Costo por resultado | CTR | Emoji |
|---------|--------|------------------|-------------------|--------------------------|-----|-------|
| 🆕 GT \| Beco \| CP \| Conjuntos (nueva, creada hoy 14:55) | ACTIVE | $3.58 | 0 (en este pull) | N/A 🟡 | 2.19% 🟡 | 🆕🟡 |
| GT \| Odoo \| CP \| Servicios (ampliada hoy, 3ª audiencia) | ACTIVE | $21.20 | 0 (en este pull) | N/A 🟡 | 1.17% 🔴 | ⬆️🟡 |
| Evento: Odoo en Acción (boost relanzado 10-19, $20 lifetime) | ACTIVE | $7.11 | 75 RSVP acumulados (+26 hoy) | $0.09/RSVP 🟢 | 2.71% 🟢 | 🟢 |
| Beco (GT, campaña original "Administradores e Inmobiliarias") | PAUSED, sin cambios (pausada 10-19 15:44) | $0.00 | - | - | - | ⏸️ |
| Toma El control de tu pyme (GT) | PAUSED, sin cambios (pausada 10-19 15:45) | $0.00 | - | - | - | ⏸️ |
| Pyme El Salvador (SV) | PAUSED, sin cambios (pausada 10-19 15:44) | $0.00 | - | - | - | ⏸️ |
| Odoo Test (GT) | PAUSED, sin cambios (pausada 10-19 15:45) | $0.00 | - | - | - | ⏸️ |
| Evento: Odoo en Acción (boost original, 10-13→10-15) | COMPLETED, sin cambios | $0.00 | - | - | - | 🏁 |
| Pyme Colombia (COL) | PAUSED, sin cambios (7º día pausada) | $0.00 | - | - | - | ⏸️ |
| Toma El control de tu pyme (USA) | PAUSED, sin cambios | $0.00 | - | - | - | ⏸️ |
| Accurate Partners - Loyalti | PAUSED, sin cambios | $0.00 | - | - | - | ⏸️ |
| Conversión Clientes Potenciales - MX / PY | PAUSED, sin cambios | $0.00 | - | - | - | ⏸️ |
| 🟡 CONVERSIÓN - CLIENTES POTENCIALES | PAUSED, sin cambios | $0.00 | - | - | - | ⏸️ |

**Esta sesión solo leyó métricas y el activity log** — todos los cambios listados abajo fueron realizados directamente en Meta Ads Manager por el equipo, no por esta rutina automatizada.

### 🆕🟡 Campaña nueva "GT | Beco | CP | Conjuntos" relanza Beco con audiencia distinta

Creada por Sebas Tenjo a las 14:55, con el ad set "CP | Advantage + Sugerencias | Beco" (targeting "Conjuntos" / condominios residenciales, en vez del "Administradores e Inmobiliarias" de la campaña original pausada ayer) y el anuncio "Beco | Inmobiliario #1". En sus primeras ~9 horas de actividad: $3.58 de gasto, 593 impresiones, CTR 2.19%, sin leads confirmados todavía en este pull.

### ⬆️🟡 "GT | Odoo | CP | Servicios" gana una 3ª audiencia y 2 anuncios nuevos, pero el CTR cae y no hay leads en el pull

Sebas Tenjo expandió la campaña lanzada ayer (Clínica + Ecom) con un tercer ad set, "CP | Advantage + Sugerencias | Odoo Para Todos" (audiencia general, creado 11:40), y sumó los anuncios "Odoo | Negocio #2" y "Odoo | Negocio #3" al ad set "Odoo Ecom" existente. El gasto del día salta a $21.20 (vs. $8.80 parciales del día de lanzamiento), pero el CTR blendeado baja a 1.17% (vs. 2.38% el día 1) y este pull no muestra leads confirmados — a diferencia del $4.40 CPL de su primer día.

### 🟢 Boost "Evento: Odoo en Acción" sigue sumando RSVPs a bajo costo

Sin cambios de configuración hoy. Acumula 75 RSVPs totales desde el relanzamiento del 10-19 (+26 en las últimas 24h), con $7.11 de gasto hoy, CPC $0.02 y CTR 2.71% — mantiene el mejor costo por resultado de toda la cuenta ($0.09/RSVP). Cierra el 10-22.

### ⏸️ Las 4 campañas pausadas ayer permanecen sin cambios ni decisión

"Toma El control de tu pyme" (GT), "Beco" (original), "Pyme El Salvador" y "Odoo Test" siguen pausadas, sin que el equipo haya decidido todavía si se reactivan con los 5 copys nuevos pendientes desde 2026-08-24 o se retiran definitivamente. Beco específicamente fue relanzada hoy, pero como campaña nueva con audiencia distinta, no como reactivación de la pausada.

---

## 📊 Análisis e Insights

- **El equipo consolida el patrón "Advantage+ Sugerencias" iniciado ayer**: las 2 campañas con actividad hoy (la expansión de Odoo Servicios y el relanzamiento de Beco) usan la misma estructura de ad set ("CP | Advantage + Sugerencias | ...") que se introdujo el 10-19, sugiriendo que el equipo adoptó este enfoque como plantilla estándar para las audiencias nuevas.
- **Posible dilución de nicho en Odoo Servicios**: el buen CPL del día 1 ($4.40) se atribuyó a los nichos específicos (clínicas, e-commerce). Añadir hoy una audiencia general ("Para Todos") podría diluir ese enfoque — el CTR blendeado ya bajó de 2.38% a 1.17%, aunque es pronto para separar el efecto de cada ad set individualmente sin una ruptura por ad set.
- **0 leads confirmados hoy en ambas campañas de lead-gen activas, a diferencia de ayer**: un pull igualmente cercano al cierre (10-19, ~23:51 GT) sí mostró leads reales (2 en Odoo Servicios, 1 en Beco original). Hoy, con $24.78 de gasto combinado, el campo `results` devuelve "Not available" en ambas — posible rezago de atribución de formularios (los leads pueden tardar horas en reportarse) más que una caída real a cero. **Pendiente de confirmar con el Reporte Performance formal de mañana.**
- **Fuerte actividad de creativos**: 24 imágenes nuevas subidas/editadas a la librería en 3 tandas (11:22, 11:32, 1:48-1:49 PM GT), alimentando los nuevos anuncios de Odoo (Para Todos, Negocio #2, Negocio #3) y Beco (Inmobiliario #1) — señal de que el equipo está probando creativos frescos en cada audiencia nueva, no reciclando los mismos assets.
- **Cambio automático de Meta no iniciado por el equipo**: a las 19:07 y 20:31 GT, Meta actualizó automáticamente 2 audiencias personalizadas basadas en píxel (`asa_auto_custom_audience`) para incluir un segundo píxel (ID `1455990525953150`) además del original (`935137862961572`). No hay evidencia de que el equipo haya conectado este segundo píxel manualmente hoy — vale la pena confirmar su origen (ver [[#📋 Próximas Acciones]]).
- **Pyme Colombia** acumula 7 días pausada sin ninguna decisión, un día más que ayer.

---

## ✏️ Cambios Realizados

**Todos los cambios siguientes se identificaron en el activity log de la cuenta (ventana 2026-10-20 11:22–20:31 hora GT) — fueron ejecutados por el equipo directamente en Meta Ads Manager, no por esta sesión automatizada:**

- **Sebas Tenjo subió/editó 24 imágenes nuevas** a la librería de creativos de la cuenta, en 3 tandas: 11:22 AM (8 imágenes), 11:32 AM (8 imágenes) y 1:48–1:49 PM (8 imágenes).
- **Sebas Tenjo actualizó el anuncio "Odoo | Negocio"** (ad set "Odoo Ecom", campaña "GT | Odoo | CP | Servicios") a las 11:23 GT — nombre y creativo.
- **Sebas Tenjo agregó el anuncio "Odoo | Negocio #2"** al ad set "Odoo Ecom" a las 11:28 GT, con ajuste de targeting del ad set.
- **Sebas Tenjo creó el ad set "CP | Advantage + Sugerencias | Odoo Para Todos"** a las 11:40 GT (audiencia general, con performance goal, puja, targeting y budget scheduling configurados) junto con el anuncio "Odoo | Para todos".
- **Sebas Tenjo agregó el anuncio "Odoo | Negocio #3"** al ad set "Odoo Ecom" a las 1:51 PM GT, con nuevo creativo.
- **Sebas Tenjo creó la campaña "GT | Beco | CP | Conjuntos"** a las 2:55 PM GT, con el ad set "CP | Advantage + Sugerencias | Beco" (targeting "Conjuntos", puja, performance goal y budget scheduling) y el anuncio "Beco | Inmobiliario #1".
- **Meta (sistema, automático)** expandió 2 audiencias personalizadas `asa_auto_custom_audience` para incluir un segundo píxel, a las 7:07 PM y 8:31 PM GT.

---

## 🔬 Investigación Realizada

- Se revisaron las 13 campañas de la cuenta a nivel campaña con `date_preset=today` (equivalente a 2026-10-20 en horario de cuenta), incluyendo gasto, resultados/RSVP, costo por resultado, CTR, CPC, CPM, impresiones, clicks, reach y estado.
- Se verificaron explícitamente los campos de leads (`lead`, `onsite_conversion_lead_grouped`, `results`) para las 2 campañas de lead-gen activas y el boost de evento, confirmando que el campo `results` devuelve "Not available" para ambas campañas de lead-gen (posible rezago de atribución, no necesariamente cero leads reales).
- Se revisó el activity log completo de la cuenta para la ventana 2026-10-20 00:00–2026-10-21 06:00 UTC (97 eventos) — se clasificaron por tipo y actor, y se extrajeron en detalle los eventos de campaña/ad set/ad/creativo relevantes.
- Se confirmó el estado del trigger automatizado "Daily Summary - 11:50 PM Guatemala" (`trig_01DMJfrsQXaTY5KJntXisDPQ`) vía `get_trigger`: sigue en `50 5 * * *` UTC sin cambios desde su creación el 2026-08-28 — 40ª ocurrencia consecutiva del bug de zona horaria.
- No se realizó investigación externa de competencia ni tendencias de mercado en esta sesión.

---

## 📊 Datos Clave del Día

| Métrica | 2026-10-20 (casi-final, parcial por rezago de atribución) | 2026-10-19 (confirmado en nota del día anterior) | Variación |
|---------|-------------------------------------------------------------|----------------------------------------------------|-----------|
| Gasto (lead-gen: Odoo Servicios + Beco Conjuntos) | $24.78 | $31.39 | 🟢 -21.1% |
| Leads confirmados (en el pull) | 0 | 5 | 🔴 -100% (posible rezago de atribución, no confirmado como real) |
| CPL Promedio (blendeado lead-gen) | No disponible | $6.28 | — |
| CTR Promedio (lead-gen) | 1.46% (blendeado Odoo 1.17% + Beco Conjuntos 2.19%) | 1.77% | 🔴 -17.5% |
| Gasto boost evento | $7.11 | $4.64 | 🔴 +53.2% |
| RSVPs del boost evento | +26 hoy (75 acumulados) | +49 (desde relanzamiento) | — |
| Gasto total de cuenta (incl. boost) | $31.89 | $36.03 | 🟢 -11.5% |
| Campaña nueva del día | GT \| Beco \| CP \| Conjuntos | GT \| Odoo \| CP \| Servicios | — |
| Peor señal del día | 0 leads confirmados en 2 campañas con $24.78 de gasto combinado | Odoo Test y Toma El control: 0 leads cada una (ya pausadas) | Pendiente de confirmar si es rezago o caída real |

**Nota:** esta cifra de leads en 0 es la lectura más incierta de la serie — a diferencia de días anteriores, no hay certeza de si refleja un cierre real o un rezago de atribución de formularios. Confirmar con el Reporte Performance formal de hoy (~7 AM GT) antes de tratar estas cifras como definitivas.

---

## 📋 Próximas Acciones

- [ ] **Confirmar con el Reporte Performance formal de hoy (~7 AM GT) el cierre real de 2026-10-20** — en particular si "GT \| Odoo \| CP \| Servicios" y "GT \| Beco \| CP \| Conjuntos" terminaron el día en 0 leads o si fue rezago de atribución del pull de las 23:52 GT.
- [ ] **Evaluar si la 3ª audiencia "Odoo Para Todos" diluye el enfoque de nicho** que explicó el buen CPL del día 1 (Clínica/Ecom) — pedir ruptura por ad set en el próximo reporte.
- [ ] **Decidir el futuro de las 4 campañas pausadas el 10-19** (Toma El control GT, Beco original, Pyme El Salvador, Odoo Test): ¿reactivar con los 5 copys nuevos pendientes desde el 2026-08-24, o retirarlas definitivamente? Beco ya fue reemplazada por una campaña nueva; falta resolver las otras 3.
- [ ] **Confirmar el origen del segundo píxel** agregado automáticamente a 2 audiencias `asa_auto_custom_audience` (7:07 y 8:31 PM GT) — verificar si fue una conexión intencional del equipo o requiere revisión.
- [ ] **Monitorear el boost "Evento: Odoo en Acción"** hasta su cierre el 10-22 ($20 lifetime, 75 RSVPs acumulados) — verificar si se traduce en asistencia real al evento.
- [ ] **Decidir el futuro de "Pyme Colombia"**, que sigue pausada sin acción desde el 10-14 (7 días).
- [ ] **Usuario:** el trigger `trig_01DMJfrsQXaTY5KJntXisDPQ` sigue disparándose a las 23:50 GT en vez de después de medianoche (40ª ocurrencia consecutiva) — solo se puede corregir manualmente desde https://claude.ai/code/routines/trig_01DMJfrsQXaTY5KJntXisDPQ.

---

## 🔗 Enlaces

- [[Reports/2026-10-19 - Reporte Performance]] — último reporte de cierre confirmado disponible (el de 2026-10-20 se genera hoy ~7 AM GT)
- [[Daily notes/2026-10-20 - Resumen del Dia]] — resumen del día anterior
- Tags: #daily-note #summary #meta-ads #octopus
