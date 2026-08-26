# Diseño por servicio — ficha de repaso

> Guía autocontenida para diseñar cada servicio hospitalario: clasificación **AEA 90364-7-710** (grupo de sala), instalación **eléctrica**, **gases medicinales**, **climatización** y **planta física** (m², dimensiones), según resoluciones **PNGCAM**.
>
> Formato: cada servicio abre con una **ficha compacta** (vista rápida) seguida del **criterio de diseño** (el porqué). Ordenado de mayor a menor criticidad.
>
> Fuentes: `resumenes/servicios-hospitalarios-resoluciones.md`, `instalaciones-electricas.md`, `climatizacion.md`, `gases-medicinales.md`, `estructura-hospitalaria.md`, `alimentacion-de-emergencia.md`. No inventa cifras: si un dato no está en los resúmenes, se marca como **[no en resúmenes]**.

---

## Índice

**Parte 1 — Consideraciones generales (transversales)**
- [1.1 Clasificación de salas AEA 710 (grupo 0/1/2A/2B)](#11-clasificación-de-salas-aea-710)
- [1.2 Qué implica una sala Grupo 2 (checklist)](#12-qué-implica-una-sala-grupo-2--checklist-de-diseño)
- [1.3 Macrochoque y microchoque](#13-macrochoque-y-microchoque)
- [1.4 Presiones, renovaciones y filtros de aire](#14-presiones-renovaciones-y-filtros-de-aire)
- [1.5 Alimentación de emergencia (qué se respalda)](#15-alimentación-de-emergencia)
- [1.6 Cómo leer cada ficha](#16-cómo-leer-cada-ficha)

**Parte 2 — Fichas por servicio (mayor → menor criticidad)**
1. [Quirófano (Cirugía) — Res. 810/2020](#1-quirófano-cirugía--res-8102020)
2. [Quirófano híbrido — Res. 810/2020](#2-quirófano-híbrido--res-8102020)
3. [UTI / Cuidados intensivos — Res. 748/2014](#3-uti--cuidados-intensivos--res-7482014)
4. [UCIP — Terapia intensiva pediátrica — Res. 747/2014](#4-ucip--terapia-intensiva-pediátrica--res-7472014)
5. [Neonatología (UTIN/UCIN) — Res. 306/2002](#5-neonatología-utinucin--res-3062002)
6. [Unidad Coronaria (UCO/UCIC) — Res. 375/2002](#6-unidad-coronaria-ucoucic--res-3752002)
7. [Hemodinamia — Res. 1184/2018](#7-hemodinamia--res-11842018)
8. [Guardia / Shock room — Res. 428/2001](#8-guardia--shock-room--res-4282001)
9. [Maternidad / Centro obstétrico — Res. 348/2003](#9-maternidad--centro-obstétrico--res-3482003)
10. [Terapia intermedia — Res. 748/2014](#10-terapia-intermedia--res-7482014)
11. [Atención del recién nacido (RN) — Res. 810/2020](#11-atención-del-recién-nacido-rn--res-8102020)
12. [Recuperación postquirúrgica — Res. 810/2020](#12-recuperación-postquirúrgica--res-8102020)
13. [Diagnóstico por imágenes: TC — Res. 610/2004 y 3590/2021](#13-tomografía-computada-tc--res-6102004-y-35902021)
14. [Diagnóstico por imágenes: RM — Res. 610/2004 y 3590/2021](#14-resonancia-magnética-rm--res-6102004-y-35902021)
15. [Radiología convencional (RX) y mamografía](#15-radiología-convencional-rx-y-mamografía)
16. [Ecografía](#16-ecografía)
17. [Internación — Res. 2547/2021](#17-internación--res-25472021)
18. [Servicio de pediatría (internación) — Res. 609/2004](#18-servicio-de-pediatría-internación--res-6092004)
19. [Cirugía ambulatoria — Res. 1866/2017](#19-cirugía-ambulatoria--res-18662017)
20. [Esterilización y servicios generales](#20-esterilización-y-servicios-generales)

- [Tablas rápidas comparativas](#tablas-rápidas-comparativas)

---

# Parte 1 — Consideraciones generales

## 1.1 Clasificación de salas AEA 710

La **AEA 90364-7-710** clasifica cada local médico por el **riesgo eléctrico para el paciente**, no por la especialidad. Aplica a salas de uso médico/dental, hidroterapia, fisioterapia y masajes; **no** aplica a pasillos, escaleras, baños, cocinas, salas de espera ni oficinas.

| Grupo | Definición | Ante 1ª falla | Ejemplos típicos |
|---|---|---|---|
| **0** | El paciente **no** contacta equipos electromédicos de red (o solo a batería). | La desconexión automática **no** es riesgo. | Consultorios sin equipamiento, esterilización, oficinas |
| **1** | El paciente contacta partes de equipo conectado a red; la discontinuidad **no** es riesgo vital. | Se admite corte. | Internación general, ecografía, masajes, terapia física, RX de diagnóstico |
| **2A** | Equipos para intervención/medición vital; debe seguir funcionando ante 1ª falla a tierra o corte. Sin riesgo de microchoque. | **No** puede interrumpirse → **red IT**. | Diálisis, endoscopía, RM, sala de parto |
| **2B** | Igual que 2A **pero** el paciente está expuesto a **microchoque** (catéter próximo al corazón). | **No** puede interrumpirse → **red IT** + vigilancia reforzada. | Quirófano, UTI, neonatología, cardiovascular, post-operatorio |

La diferencia 2A/2B está en el **tipo de monitor de aislación** y en el nivel de protección contra microchoque, no en si llevan red IT (ambos la llevan).

## 1.2 Qué implica una sala Grupo 2 — checklist de diseño

Cuando un servicio cae en **Grupo 2**, arrastra automáticamente todo este paquete (vale para quirófano, UTI, UCIP, neonato, UCO, hemodinamia, sala de parto):

- **Red IT (aislada)**: transformador de aislación monofásico, seco, **3,15–8 kVA** (5 kVA preferido para UTI y quirófanos), relación 1:1, ≤230 Vca. Un tablero IT **propio por sala** (nunca compartido entre 2 salas). Salas con **>4 puestos** no pueden tener un solo sistema IT.
- **Monitor de aislación (IMD)** + **repetidor** visible en la sala: vigila la impedancia/corriente de fuga y alarma ante deterioro, permitiendo continuar el trabajo tras la 1ª falla.
- **Doble alimentación** (preferencial + alternativa) con separación física; secundario del transformador a la carga **≤50 m**.
- **Equipotencialización (AEA 90364-7-710)**: barra hospitalaria (**BPATH**), conductores **PEH** radiales (uno por punto), diferencia de potencial entre masas **≤20 mV** en la zona del paciente. Se equipotencializan: bornes PE de todo TUM, piso semiconductivo (2 puntos), mesa de cirugía, cama, luminaria scialítica, torre de monitoreo, poliducto y cañería de gases metálica, cañería de agua, ductos de climatización, marcos de puertas/ventanas.
- **Tomas de uso médico (TUM)**: mín. **12 por puesto** en UTI adulto/pediátrico (**≥18** en neonatología), repartidos en **≥2 circuitos** de **≤6 tomas** c/u; si hacen falta más de 2 circuitos, alimentación **alternada (cruzada)** desde 2 redes IT.
- **IUG** (iluminación): la mitad de las bocas desde **UPS**; luminarias en ≥2 circuitos independientes; **scialíticas alimentadas desde la red IT**.
- **Consumo de referencia**: ~**600 W/puesto** crítico adulto/pediátrico; **1500 W/puesto** neonatología (+2000 W adicional de reserva).
- **Emergencia**: es servicio **crítico** → respaldo por **GE** (entrada <15 s) y **UPS on-line** para la transferencia sin corte.

> Denominación de red: es **TT** desde la acometida hasta el tablero de aislación, y **IT** de ahí en adelante (cambia en el transformador de aislación).

## 1.3 Macrochoque y microchoque

- **Macrochoque**: contacto externo (piel intacta) con un elemento bajo tensión. Se previene con la **continuidad de servicio** de la red IT (sigue funcionando tras la 1ª falla) y las protecciones diferenciales.
- **Microchoque**: la corriente entra al interior del cuerpo por un conductor (catéter, electrodo) cercano al corazón. Corrientes del orden de **µA** pueden provocar **fibrilación ventricular**. Se previene con **red IT + monitor de aislación + estructura equipotencial (≤20 mV)**. Es lo que distingue a las salas **2B**.

## 1.4 Presiones, renovaciones y filtros de aire

- **Presión positiva** (interior > exterior): protege al paciente/ambiente estéril de patógenos externos. Quirófano, hemodinamia, inmunodeprimidos.
- **Presión negativa** (interior < exterior): contiene patógenos adentro. Pacientes infecciosos / aislamiento.
- **Renovaciones/hora**: entre **2 y 12** según sala (quirófano 15–20; UTI 4 en habitación / 2 en resto; shock room 2).
- **HR**: las infecciones hospitalarias **aumentan con HR < 40%**; HR alta favorece microbiología; rango típico **30–60%**.
- **Filtros de alta eficiencia** (retención sobre el MPPS, ~0,3 µm):
  - **EPA**: E10 ≥85% · E11 ≥95% · E12 ≥99,5%
  - **HEPA**: H13 ≥99,95% · H14 ≥99,995%
  - **ULPA**: U15 ≥99,9995% y superiores
  - Quirófano: filtración escalonada **25% → 90% → HEPA 99,97–99,99%** terminal. Alta seguridad (trasplante/cardiovascular): 2º HEPA H14 o ULPA.
- **Rol del ingeniero en clima** (aclaración de cátedra): **no** se calculan cargas térmicas ni se dimensionan conductos/equipos. Se **asesora** sobre tipo de equipo y etapas de filtrado para cumplir la norma.

## 1.5 Alimentación de emergencia

- **Tiempo de entrada del GE en servicio: < 15 s.** UPS on-line cubre el intervalo sin corte (0 s).
- **Servicios críticos** (respaldo obligatorio): quirófanos, UTI, UTI neonatal, salas de parto, guardia de urgencias, hemodinamia/angiografía, hemodiálisis, laboratorio de urgencias, soporte vital (compresores de aire medicinal, bombas de vacío, PSA, telemetría), iluminación general de emergencia.
- **Parcialmente críticos**: cuidados intermedios, diagnóstico por imágenes, ascensores/montacargas, iluminación de circulación, agua potable, bombeo cloacal, seguridad/vigilancia, esterilización.

## 1.6 Cómo leer cada ficha

Cada servicio tiene:
- **Ficha compacta** — tabla con: Definición · Grupo AEA (tipo de local) · Locales médicos · Eléctrico · Gases (bocas O₂/aire/vacío en cabecera) · Climatización · Planta física · Norma.
- **Criterio de diseño** — el porqué de las decisiones y los detalles útiles para justificar en un final.

Los valores de gases son **bocas por cama/puesto en cabecera**. Los de clima son T [°C] / HR [%] / renovaciones-h / presión.

> **Definición**: qué es y qué hace el servicio. **Grupo AEA (tipo de local)**: el "tipo de local" del servicio según AEA 90364-7-710 (0/1/2A/2B, ver 1.1). **Locales médicos**: los ambientes principales que componen el servicio, cada uno con su tipo de local entre paréntesis. El tipo de cada local se asigna aplicando las definiciones de 1.1 al riesgo eléctrico de ese ambiente concreto (un mismo servicio puede combinar locales de distinto tipo: p. ej. quirófano 2B + comando 0). Ambientes no médicos (comando, office, sala de espera) quedan **fuera del alcance de la AEA** y se marcan como tal.

---

# Parte 2 — Fichas por servicio

## 1. Quirófano (Cirugía) — Res. 810/2020

| Campo | Requisito |
|---|---|
| **Definición** | Sala donde se realiza el acto quirúrgico con el paciente anestesiado e invadido; núcleo del área quirúrgica. |
| **Grupo AEA (tipo de local)** | **2B** (red IT, equipotencial, anti-microchoque) |
| **Locales médicos** | Quirófano (**2B**) · sala de recuperación/observación (**1–2**) · atención del RN en cesárea (**2**) · zona de lavado quirúrgico y office de enfermería (no médicos, fuera de AEA). |
| **Eléctrico** | Red IT con transformador de aislación **5 kVA** preferido; monitor de aislación + repetidor; scialíticas desde red IT; TUM ≥2 circuitos; IUG mitad desde UPS; equipotencial ≤20 mV. **Crítico** → GE + UPS. |
| **Gases** | **2 O₂ · 1 aire comprimido · 2 vacío** |
| **Climatización** | Flujo **unidireccional** (impulsa techo, extrae suelo); **15–20 renov/h**; **presión positiva** (Δp ≥ 2,5 Pa); **T 20–24 °C**; **HR 30–60% (óptimo 50–55%)**; toma de aire **100% exterior**; filtrado 3 etapas **25→90→HEPA 99,97–99,99%**; velocidad 0,20–0,30 m/s; 24 h en marcha. **Se excluye split/pared.** |
| **Planta física** | Polivalente: 20 / 24 / 30 / 36 m² · flujo laminar 40 / 48 m². Cesárea siempre 24 m². Altura cielorraso **≥3 m**; puertas **≥1,20 m**. |
| **Norma** | Res. 810/2020 (PNGCAM) |

**Criterio de diseño.** Es la sala más exigente: paciente anestesiado, invadido y con equipos de soporte vital → **2B** obligatorio. La red IT garantiza que una 1ª falla a tierra **no corte** el suministro (continuidad = evita macrochoque), y el monitor de aislación avisa para reparar sin detener la cirugía. El equipotencial ≤20 mV neutraliza el microchoque. La **climatización es tan crítica como la eléctrica**: presión positiva + HEPA terminal impiden contaminación de la herida; el flujo unidireccional "barre" partículas desde el campo estéril hacia la extracción baja. La toma 100% exterior evita recircular gases anestésicos. El equipamiento por riesgo define scialíticas: **Alto** (3 brazos con cámara, ecógrafo, arco en C, tomógrafo), **Mediano** (2 brazos, 2 monitores), **Bajo** (2 brazos, 1 monitor) — todas alimentadas desde la red IT.

## 2. Quirófano híbrido — Res. 810/2020

| Campo | Requisito |
|---|---|
| **Definición** | Quirófano que integra cirugía + imágenes de intervención (arco en C o resonador) en el mismo acto. |
| **Grupo AEA (tipo de local)** | **2B** (como quirófano, con cargas trifásicas altas del imagenología) |
| **Locales médicos** | Quirófano híbrido (**2B**) · sala técnica/comando de imágenes (no médico, fuera de AEA) · zona de lavado (no médico). |
| **Eléctrico** | Red IT + alta demanda por arco en C / resonador; blindaje plomado. **Crítico** → GE + UPS. |
| **Gases** | **2 O₂ · 2 aire · 2 vacío** |
| **Climatización** | Flujo **laminar**, presión positiva, HEPA terminal (criterio quirófano de alta seguridad). |
| **Planta física** | Con arco en C: **≥50 m²**. Con resonador anexo: **≥70 m²**. Cielorraso **≥3,80 m**. Blindaje plomado. |
| **Norma** | Res. 810/2020 |

**Criterio de diseño.** Combina cirugía + imágenes de intervención en el mismo acto, por eso duplica gases (2 aire para herramientas neumáticas/ventilación) y sube superficie/altura para alojar el equipo y su movimiento. El blindaje plomado protege de la radiación del arco en C; si hay resonador, aplican además las precauciones de RM (materiales no ferromagnéticos, línea de 5 Gauss). Flujo laminar por ser cirugía de alta complejidad.

## 3. UTI / Cuidados intensivos — Res. 748/2014

| Campo | Requisito |
|---|---|
| **Definición** | Unidad para pacientes críticos con soporte vital continuo y monitoreo permanente. |
| **Grupo AEA (tipo de local)** | **2B** |
| **Locales médicos** | Box/habitación de cuidados críticos (**2B**) · habitación de aislamiento (**2B**) · estación central de enfermería, offices y guardia médica (no médicos, fuera de AEA). |
| **Eléctrico** | Red IT; **≥12 TUM por cama** en ≥2 circuitos (≤6 por circuito); no más de 4 camas por red IT (disposición cruzada); enchufe/línea para rayos portátil; ~600 W/cama. **Crítico** → GE + UPS. |
| **Gases** | **2 O₂ · 1 aire (recomendable 2) · 2 vacío** por cama en cabecera. Aire seco/puro por compresor libre de aceite. **Alarma audible** de caída de presión de O₂. |
| **Climatización** | **T 24–26 °C · HR 30–60% · 4 renov/h en habitación, 2/h resto**; presión +/– según aislamiento. |
| **Planta física** | Superficie **≥9 m² × 2 × nº camas** (nuevas 12 m²/cama); 50% para apoyo. **Nivel 1: ≥8 camas · Nivel 2: ≥4 camas.** Puertas de paso de camilla con apertura hacia afuera; estación de enfermería con visualización directa. |
| **Norma** | Res. 748/2014 |

**Criterio de diseño.** Pacientes con soporte vital continuo y catéteres centrales → **2B** con todo el paquete Grupo 2. La regla de **≤4 camas por red IT** con disposición cruzada evita que una falla deje sin energía a un sector entero: cada cama toma de dos redes alternadas. Los ≥12 TUM por cama cubren respirador, monitores, bombas de infusión, etc. La climatización con 4 renov/h en habitación mantiene calidad de aire sin ser quirófano; el control de HR ≥40% reduce infecciones. Superficie ×2 porque la norma exige 50% de área de apoyo (enfermería, offices, guardia médica).

## 4. UCIP — Terapia intensiva pediátrica — Res. 747/2014

| Campo | Requisito |
|---|---|
| **Definición** | UTI pediátrica (1 mes–15 años) para pacientes críticos; incluye reanimación propia. |
| **Grupo AEA (tipo de local)** | **2B** |
| **Locales médicos** | Puesto de cuidados críticos pediátricos (**2B**) · habitación individual de aislamiento (**2B**) · unidad de reanimación/shock room (**2**) · cuidados intermedios (**1**) · estación de enfermería (no médico, fuera de AEA). |
| **Eléctrico** | Red IT; **≥12 enchufes por cama** + rayos portátil. **Crítico** → GE + UPS. |
| **Gases** | **2 O₂ · 1 aire (mejor 2) · ≥1 vacío (preferente 2)** |
| **Climatización** | Criterio UTI (T 24–26 °C, HR 30–60%, 4/h habitación). |
| **Planta física** | **≥7 m²/cama** en área abierta; **≥9 m²** en habitación individual (12 m² nuevas); total = doble de superficie de camas; 50% apoyo. **≥6 camas.** Pacientes de 1 mes a 15 años. Incluye Unidad de Reanimación (shock room) y Cuidados Intermedios. |
| **Norma** | Res. 747/2014 |

**Criterio de diseño.** Mismo nivel de criticidad que UTI adulto (2B, red IT, gases y clima equivalentes), adaptado a superficie pediátrica menor por cama en áreas abiertas pero con habitaciones individuales de aislamiento. Integra reanimación propia por la fragilidad del paciente pediátrico crítico.

## 5. Neonatología (UTIN/UCIN) — Res. 306/2002

| Campo | Requisito |
|---|---|
| **Definición** | Atención del recién nacido crítico (UTIN) e intermedio (UCIN). |
| **Grupo AEA (tipo de local)** | **2B** |
| **Locales médicos** | Sector UTIN/UCIN (**2B**) · habitación de aislamiento (**2B**) · recepción/reanimación del RN en sala de partos (**2**) · cocina de leche y lactario (no médicos, fuera de AEA). |
| **Eléctrico** | Red IT; **≥18 tomacorrientes** en panel de cabecera (mayor que UTI adulto); ~1500 W/puesto. **Crítico** → GE + UPS. |
| **Gases** | **2 O₂ · 1 aire · 1 vacío** por plaza. Alarmas visuales-acústicas de volumen; **≥2 compresores a pistón seco con filtros bacterianos**. |
| **Climatización** | **T ambiental 25–26 °C** (más cálida que UTI). |
| **Planta física** | **2,8 m²/paciente**; sectores de 24 m² con **máx. 6 pacientes**; habitación de aislamiento **24 m²**; estación de enfermería **>6 m²**; cocina de leche (limpio/sucio) y lactario. |
| **Norma** | Res. 306/2002 (641/2012) |

**Criterio de diseño.** El recién nacido no regula temperatura → ambiente más cálido (25–26 °C) y más tomas (≥18) por la cantidad de equipos por incubadora (respirador, monitores, luminoterapia, bombas). La exigencia de aire por **compresores a pistón seco con filtro bacteriano** es clave: el aire que respira un neonato debe ser puro y sin aceite. 1500 W/puesto (vs 600 W adulto) por la mayor densidad de equipamiento.

## 6. Unidad Coronaria (UCO/UCIC) — Res. 375/2002

| Campo | Requisito |
|---|---|
| **Definición** | Unidad de cuidados intensivos cardiológicos/coronarios; paciente cardíaco monitorizado con posible cateterismo. |
| **Grupo AEA (tipo de local)** | **2B** (cardiovascular / soporte vital) |
| **Locales médicos** | Box individual de cuidados coronarios (**2B**) · estación central de enfermería (no médico, fuera de AEA). |
| **Eléctrico** | **≥10 tomas de 220 V** por box; deseable 110 V y toma para rayos portátil con **línea independiente**; **grupo electrógeno** para suministro inmediato. Luz central ≥100 lux + luz de lectura + luz articulable para procedimientos. |
| **Gases** | **2 O₂ · 1 aire · 1 vacío** en cabecera |
| **Climatización** | Aire climatizado, insonorización. |
| **Planta física** | Superficie = **nº camas × 9 × 2** (50% apoyo / 50% atención); box individual **≥9 m²** con observación directa; acceso por 4 lados; luz natural. |
| **Norma** | Res. 375/2002 |

**Criterio de diseño.** Paciente cardíaco monitorizado con posible cateterismo → riesgo de microchoque = **2B**. La norma insiste en el **GE de suministro inmediato** porque una desfibrilación o marcapasos externo no admite corte. El acceso por 4 lados al box permite reanimación desde cualquier posición. Las tomas de 110 V son para equipos importados de monitoreo cardíaco.

## 7. Hemodinamia — Res. 1184/2018

| Campo | Requisito |
|---|---|
| **Definición** | Sala de cateterismo cardíaco/vascular guiado por radiología (intervencionismo); quirófano de cateterismo. |
| **Grupo AEA (tipo de local)** | **2** (sala de procedimiento con equipos vitales; intervencionismo con catéter → riesgo microchoque). |
| **Locales médicos** | Sala de procedimiento (**2**, zona restringida) · puesto de observación (**1**, zona semirrestringida) · sala de comando plomada y office (no médicos, fuera de AEA). |
| **Eléctrico** | Gases centrales + red segura; RX de radiación pulsada con control automático de kV, potencia recomendable **80 kW**; blindaje plomado. **Crítico** → GE + UPS. |
| **Gases** | Centrales: **O₂ · aire · aspiración** (sala de procedimiento y puesto de observación). Office: aire comprimido. |
| **Climatización** | **AA con filtros HEPA terminales 99,97%** (criterio quirúrgico). |
| **Planta física** | Sala de procedimiento **≥30 m²**, altura ≥3 m, blindaje plomado, puertas ≥1,20 m. Puesto de observación **≥8 m²** (con gases). Sala de comando **≥6 m²** (plomada). Office **≥6 m²**. Zonas: restringida (procedimiento + comando) y semirrestringida (observación + office). |
| **Norma** | Res. 1184/2018 |

**Criterio de diseño.** Es un quirófano de cateterismo: cateterismo cardíaco/vascular con guía radiológica. Por eso combina exigencias de **cirugía** (HEPA terminal 99,97%, presión de sala limpia, gases centrales) con las de **imágenes** (blindaje plomado, sala de comando separada, RX de 80 kW con control automático de kV para minimizar dosis). El catéter intravascular próximo al corazón obliga al tratamiento anti-microchoque de Grupo 2.

## 8. Guardia / Shock room — Res. 428/2001

| Campo | Requisito |
|---|---|
| **Definición** | Servicio de urgencias/emergencias: recepción, observación transitoria y estabilización del paciente agudo. |
| **Grupo AEA (tipo de local)** | Shock room / reanimación: criterio **Grupo 2** (soporte vital); observación: Grupo 1. |
| **Locales médicos** | Shock room/reanimación (**2**, criterio) · sala de observación transitoria (**1**) · admisión y sala de espera (no médicos, fuera de AEA). |
| **Eléctrico** | **Crítico** (guardia de urgencias) → GE + UPS; tomas para equipos de reanimación; apoyo de radiología. |
| **Gases** | Centrales O₂/aire/vacío en shock room (soporte vital de reanimación). *[Bocas exactas no tabuladas en resúmenes — usar criterio UTI: 2 O₂ / 1 aire / 2 vacío.]* |
| **Climatización** | **Shock room: T 25–26 °C · HR 30–60 % · 2 renov/h.** Observación: **T 24–25 °C.** |
| **Planta física** | **Shock room: ≥12 m²/cama.** Observación (transitoria ≤6 h): boxes ≥2 camas (preferible 4), **6 m²/cama**. Admisión con acceso directo desde el exterior. |
| **Norma** | Res. 428/2001 |

**Criterio de diseño.** La guardia tiene dos niveles: **observación** (paciente estable, transitorio → Grupo 1, 6 m²/cama) y **shock room / hospitalización de emergencia** (crítico, reanimación → criterio Grupo 2, 12 m²/cama para maniobrar el equipo de reanimación). Es servicio crítico completo por su rol en la emergencia: respaldo de GE obligatorio y radiología de apoyo inmediata.

## 9. Maternidad / Centro obstétrico — Res. 348/2003

| Campo | Requisito |
|---|---|
| **Definición** | Centro obstétrico: atención del preparto, parto y cesárea, con recepción del recién nacido. |
| **Grupo AEA (tipo de local)** | Sala de parto: **2A** (parto = sala grupo 2); quirófano de cesárea: **2B**. |
| **Locales médicos** | Sala de parto (**2A**) · quirófano de cesárea (**2B**) · sala de preparto (**1–2**) · recepción del RN (**2**). |
| **Eléctrico** | Criterio Grupo 2 en parto/cesárea (red IT); servicio **crítico** (salas de parto) → GE + UPS. |
| **Gases** | Según puesto de parto/cesárea (criterio quirúrgico para la cesárea: 2 O₂ / 1 aire / 2 vacío). *[Bocas de preparto/parto no tabuladas explícitamente.]* |
| **Climatización** | Criterio quirúrgico en cesárea; RN según Res. 810 (28 °C + radiante 37 °C). |
| **Planta física** | Preparto: ≥2 puestos de **9 m²**. Parto: ≥2 salas de **16 m²**, altura 3 m. Quirófano de cesárea: **≥24 m²**. RRN (parto gemelar): **≥6 m²**. |
| **Norma** | Res. 348/2003 |

**Criterio de diseño.** El parto es sala **Grupo 2** (monitoreo materno-fetal, posibilidad de intervención). La cesárea se trata como quirófano polivalente de 24 m² (opción 2) con local contiguo para el RN. La atención del recién nacido exige ambiente cálido y fuente radiante (ver ficha 11). Se integra con neonatología por proximidad funcional.

## 10. Terapia intermedia — Res. 748/2014

| Campo | Requisito |
|---|---|
| **Definición** | Escalón entre internación y UTI: paciente post-crítico estable que aún necesita monitoreo. |
| **Grupo AEA (tipo de local)** | **Grupo 1** (cuidados intermedios, sin soporte vital continuo). |
| **Locales médicos** | Puesto de cuidados intermedios (**1**) · cama de aislamiento (**1**) · estación central de enfermería (no médico, fuera de AEA). |
| **Eléctrico** | **6 tomas eléctricas por cama.** **Parcialmente crítico** (respaldo según diseño). |
| **Gases** | Criterio UTI atenuado *[bocas no tabuladas específicamente para intermedia]*. |
| **Climatización** | **Igual a UTI** (T 24–26 °C, HR 30–60%, 4/h habitación). |
| **Planta física** | **9 m²/puesto**; área de apoyo 40–50%; **≥8 camas** y no más de 2 por cada cama de cuidados críticos; camas de aislamiento; estación central de enfermería. |
| **Norma** | Res. 748/2014 |

**Criterio de diseño.** Escalón entre internación y UTI: el paciente sale de fase crítica pero necesita monitoreo. Menos tomas (6 vs ≥12), sin red IT obligatoria (Grupo 1), pero conserva la climatización de UTI porque comparte la unidad. Se dimensiona en relación a las camas críticas (≤2 intermedias por cada crítica).

## 11. Atención del recién nacido (RN) — Res. 810/2020

| Campo | Requisito |
|---|---|
| **Definición** | Recepción y reanimación inmediata del recién nacido, contiguo al quirófano de cesárea. |
| **Grupo AEA (tipo de local)** | **Grupo 2** (contiguo a quirófano de cesárea). |
| **Locales médicos** | Puesto de atención del RN (**2**) — 2 puestos simultáneos con fuente de calor radiante. |
| **Eléctrico** | Criterio Grupo 2. Fuente de calor radiante controlada. |
| **Gases** | **1 O₂ · 1 vacío** por puesto |
| **Climatización** | **T 28 °C** + **fuente de calor radiante a 37 °C** sobre mesada. |
| **Planta física** | Contiguo a quirófano de cesáreas; **2 puestos simultáneos**; **≥6 m²**. Incubadora de transporte. |
| **Norma** | Res. 810/2020 (A.2.2) |

**Criterio de diseño.** El RN pierde calor rápidamente: ambiente a 28 °C (el más cálido de todo el hospital) más radiante a 37 °C sobre la mesa de recepción. Gases mínimos (O₂ + vacío) para reanimación neonatal inmediata. Se ubica pegado a la cesárea para trasladar al RN en segundos.

## 12. Recuperación postquirúrgica — Res. 810/2020

| Campo | Requisito |
|---|---|
| **Definición** | Vigilancia postanestésica del paciente hasta recuperar consciencia y estabilidad tras la cirugía. |
| **Grupo AEA (tipo de local)** | **Grupo 1–2** según monitoreo (postanestésico vigilado). |
| **Locales médicos** | Puesto en sala de recuperación (**1–2**) · box individual cerrado (**1–2**) · office de enfermería (no médico, fuera de AEA). |
| **Eléctrico** | Tomas para monitoreo postanestésico; office de enfermería. **Parcialmente crítico.** |
| **Gases** | **1 O₂ · 1 aire · 1 vacío** por puesto (poliducto) |
| **Climatización** | Criterio quirúrgico atenuado *[no tabulado específicamente]*. |
| **Planta física** | **1 puesto de 6 m² por quirófano** en sala de recuperación; box individual cerrado **10 m²**; office de enfermería **6 m²**. |
| **Norma** | Res. 810/2020 (A.2.7 / A.2.8) |

**Criterio de diseño.** El paciente despierta de la anestesia bajo vigilancia: gases completos por poliducto (O₂ + aire + vacío) para asistir la ventilación si es necesario. Se dimensiona a razón de un puesto por quirófano, porque cada cirugía genera un paciente en recuperación.

## 13. Tomografía computada (TC) — Res. 610/2004 y 3590/2021

| Campo | Requisito |
|---|---|
| **Definición** | Diagnóstico por imágenes con tomógrafo computado (RX seccional). |
| **Grupo AEA (tipo de local)** | **Grupo 1** (o **2** si intervencionismo) |
| **Locales médicos** | Sala de examen/gantry (**1**, o **2** si intervencionismo) · sala de recuperación (**1**) · sala de comando plomada y sala técnica (no médicos, fuera de AEA). |
| **Eléctrico** | Trifásica **3×380 V + N + T**; relevamiento en **kVA**; **UPS esencial**; potencia del orden 50–80 kW. |
| **Gases** | O₂ en examen y recuperación; poliducto con **O₂ (4 bar) y vacío**; aire (4 bar) opcional. |
| **Climatización** | AA **obligatorio y exclusivo**; gantry **~20–22 °C constante**; sala técnica refrigerada 24 h. |
| **Planta física** | Locales: examen (gantry), comando separado (vidrio plomado/CCTV), recuperación (obligatoria nivel II–III), sala técnica. |
| **Norma** | Res. 610/2004 + 3590/2021 |

**Criterio de diseño.** El tubo de RX y la electrónica del gantry disipan mucho calor y son sensibles a la temperatura → AA exclusivo constante 20–22 °C, 24 h. La UPS es esencial porque un corte durante un estudio con contraste arruina la adquisición y puede comprometer al paciente. Comando separado con blindaje plomado por la radiación. Grupo 1 en diagnóstico; sube a 2 si se hacen punciones/intervenciones guiadas.

## 14. Resonancia magnética (RM) — Res. 610/2004 y 3590/2021

| Campo | Requisito |
|---|---|
| **Definición** | Diagnóstico por imágenes por resonancia magnética (campo magnético + radiofrecuencia). |
| **Grupo AEA (tipo de local)** | **Grupo 1** (o **2** si intervencionismo) |
| **Locales médicos** | Sala del imán/jaula de Faraday (**1**, o **2** si intervencionismo) · comando, sala técnica (chillers/gradientes) y vestidor (no médicos, fuera de AEA). |
| **Eléctrico** | Trifásica muy alta; alimentación dedicada. |
| **Gases** | O₂ y vacío; **prohibido acero/ferromagnéticos** dentro de la sala del imán (materiales no ferromagnéticos o fuera de la línea de 5 Gauss). |
| **Climatización** | AA **dedicado y constante**; chiller de agua fría para gradientes. |
| **Planta física** | Sala del imán = **jaula de Faraday**; sala técnica (chillers, gradientes); comando; vestidor. Instalación especial: **tubo de quench** (salida de emergencia del helio). |
| **Norma** | Res. 610/2004 + 3590/2021 |

**Criterio de diseño.** El campo magnético permanente domina el diseño: nada ferromagnético dentro (cañerías, tomas y equipos no ferrosos, o fuera de los 5 Gauss). La jaula de Faraday aísla de radiofrecuencia externa. El **tubo de quench** evacúa el helio si el imán pierde superconductividad (riesgo de asfixia). Chiller y AA constantes porque los gradientes generan calor y el imán exige estabilidad térmica.

> **Matiz de fuentes sobre el grupo:** el resumen de imágenes (`servicios-hospitalarios-resoluciones.md`) clasifica la RM como **Grupo 1 (o 2 si intervencionismo)**; en cambio, el diagrama de arquitectura eléctrica (`instalaciones-electricas.md`) la lista como ejemplo de sala **2A** (red IT). Ante la duda, para diagnóstico puro alcanza Grupo 1; si hay procedimientos guiados, tratarla como Grupo 2. Verificar contra el PDF fuente si el final exige un valor único.

## 15. Radiología convencional (RX) y mamografía

| Campo | Requisito |
|---|---|
| **Definición** | Radiología convencional de diagnóstico (proyección) y mamografía. |
| **Grupo AEA (tipo de local)** | Sala de examen **Grupo 1**; mamografía **Grupo 0 o 1**. |
| **Locales médicos** | Sala de examen RX (**1**) · mamografía (**0–1**) · comando blindado y vestidor (no médicos, fuera de AEA). |
| **Eléctrico** | Trifásica **3×380 V + N + T**; potencias **50–80 kW**. |
| **Gases** | Diagnóstico (nivel I–II): no requiere central, sí O₂ disponible. Intervencionista (III / mamografía intervencionista): **O₂ + vacío**. |
| **Climatización** | **20–24 °C · 40–60% HR** (evita estática en detectores digitales); extracción por calor de servidores. |
| **Planta física** | RX digital ~20–25 m² (con comando blindado); mamografía ~12–15 m². Locales según DR (examen + comando + vestidor) o CR/analógico. |
| **Norma** | Res. 610/2004 + 3590/2021 |

**Criterio de diseño.** Diagnóstico simple = Grupo 1 (el paciente no depende de equipo vital). La digitalización (flat panel) elimina el cuarto oscuro y la procesadora, reemplazados por workstations y servidores → aparece carga térmica de servidores a extraer. HR 40–60% para no dañar los detectores por estática. El comando blindado protege al operador de la radiación.

## 16. Ecografía

| Campo | Requisito |
|---|---|
| **Definición** | Diagnóstico por ultrasonido, sin radiación; la modalidad de imágenes menos exigente. |
| **Grupo AEA (tipo de local)** | **Grupo 0 o 1** |
| **Locales médicos** | Sala de examen con baño propio (**0–1**; sube a **1** con Doppler/punciones). |
| **Eléctrico** | **220 V estándar.** |
| **Gases** | Diagnóstico: no requiere. Intervencionismo (Doppler/punciones): **O₂ (tubo portátil) + aspiración**. |
| **Climatización** | **Split suficiente, 22–24 °C.** |
| **Planta física** | Sala de examen con baño propio; sin cuarto de revelado. |
| **Norma** | Res. 610/2004 + 3590/2021 |

**Criterio de diseño.** La modalidad menos exigente: sin radiación, sin equipo de soporte vital, sin gases en diagnóstico puro. Basta 220 V estándar y un split. Sube a Grupo 1 y suma O₂/aspiración solo si se hacen procedimientos invasivos guiados por eco.

## 17. Internación — Res. 2547/2021

| Campo | Requisito |
|---|---|
| **Definición** | Hospitalización de cuidados básicos del paciente estable. |
| **Grupo AEA (tipo de local)** | **Grupo 1** (internación general: el paciente puede tener equipos aplicados —monitor, bomba de infusión— pero su discontinuidad no es riesgo vital). |
| **Locales médicos** | Habitación de internación individual/doble (**1**) · habitación de paciente aislado (**1**) · office de enfermería y secretaría (no médicos, fuera de AEA). |
| **Eléctrico** | Instalación estándar; **parcialmente crítico**. |
| **Gases** | **O₂ y vacío** en cabecera. |
| **Climatización** | Central/zonal **regulable por habitación**. |
| **Planta física** | Habitación individual **20 m²** (obstetricia 22); doble **26 m²** (obstetricia 28); paciente aislado 20 m². Módulo estructural **7,20 × 7,20 m**; unidades de 24 habitaciones; puertas luz ≥0,80 m (deseable 1,20). Office de enfermería 6 m² (2 enfermeras) / 9 m² (3). |
| **Norma** | Res. 2547/2021 |

**Criterio de diseño.** Paciente estable que puede tener equipos aplicados (monitor, bomba de infusión) pero cuya interrupción no compromete la vida → **Grupo 1**: no requiere red IT ni equipotencial (eso es exclusivo de Grupo 2). Gases básicos (O₂ y vacío) por si se necesita oxigenoterapia o aspiración puntual. El módulo 7,20×7,20 m es la trama estructural típica que ordena la planta. Se construyen habitaciones "instaladas para 2 camas" aunque se usen individuales, para flexibilidad futura.

## 18. Servicio de pediatría (internación) — Res. 609/2004

| Campo | Requisito |
|---|---|
| **Definición** | Internación general pediátrica (cuidados básicos del paciente pediátrico estable). |
| **Grupo AEA (tipo de local)** | **Grupo 1** (internación pediátrica general). |
| **Locales médicos** | Habitación/box de internación pediátrica (**1**) · enfermería, estación de biberones y lactario (no médicos, fuera de AEA). |
| **Eléctrico** | Estándar de internación. |
| **Gases** | Criterio internación (O₂ y vacío). |
| **Climatización** | Confort de internación. |
| **Planta física** | Internación **≥9,50 m²/cama** (lado ≥3 m); habitaciones individuales o boxes de 3–6. Enfermería 8,50 m² (12 camas) / 11,5 m² (24–30). Estación de biberones 6 m² (12 camas) / 9,50 m² (48). |
| **Norma** | Res. 609/2004 |

**Criterio de diseño.** Internación general adaptada a pediatría: superficie algo mayor por cama (9,50 m²) para acompañante, y locales propios (estación de alimentación/biberones, lactario). Sin criticidad eléctrica especial (Grupo 1, como toda internación general); la pediatría crítica va a UCIP (ficha 4).

## 19. Cirugía ambulatoria — Res. 1866/2017

| Campo | Requisito |
|---|---|
| **Definición** | Quirófano para procedimientos menores con alta el mismo día (≤6 h, sin internación). |
| **Grupo AEA (tipo de local)** | **Grupo 2** (es quirófano, aunque de baja complejidad). |
| **Locales médicos** | Quirófano ambulatorio (**2**) · sala de recuperación/preanestesia (**1**). |
| **Eléctrico** | Criterio Grupo 2 atenuado (procedimientos ≤6 h, sin internación). |
| **Gases** | Criterio quirúrgico *[bocas no tabuladas para ambulatoria]*. |
| **Climatización** | Por **AA / calefacción / ventilación forzada** (menos exigente que quirófano central). |
| **Planta física** | **Quirófano ≥12 m²** (lado ≥3 m); sala de recuperación/preanestesia **≥12 m²**. Cuidados postoperatorios poco intensivos, ≤6 h, sin internación. |
| **Norma** | Res. 1866/2017 |

**Criterio de diseño.** Quirófano para procedimientos menores con alta el mismo día: sigue siendo Grupo 2 (es acto quirúrgico) pero con superficie mínima (12 m²) y climatización más simple, porque no se hacen cirugías mayores ni se interna. La recuperación es breve y poco intensiva.

## 20. Esterilización y servicios generales

| Campo | Requisito |
|---|---|
| **Definición** | Servicio de apoyo no médico: procesamiento y esterilización de material, más servicios generales. |
| **Grupo AEA (tipo de local)** | **Grupo 0** (servicio de apoyo, no médico). |
| **Locales médicos** | No tiene locales médicos: zona limpia/sucia de esterilización, lavandería, cocina y residuos (todos **Grupo 0**, fuera del alcance clínico de la AEA). |
| **Eléctrico** | Estándar; **parcialmente crítico** (esterilización). Autoclaves = cargas trifásicas de potencia. |
| **Gases** | No requiere gases medicinales en cabecera. |
| **Climatización** | Sin requisitos específicos citados en resúmenes *(flujo limpio→sucio por criterio de contaminación cruzada)*. |
| **Planta física** | Circulación diferenciada limpio/sucio. |
| **Norma** | PNGCAM (apoyo) |

**Criterio de diseño.** Servicio **no médico de apoyo** → Grupo 0. No hay paciente conectado, así que la exigencia eléctrica es de potencia (autoclaves) más que de seguridad del paciente. Los **servicios generales** (lavandería, cocina, residuos) siguen la misma lógica: apoyo, Grupo 0, sin gases medicinales.

---

# Tablas rápidas comparativas

## Clasificación AEA 710 por servicio

| Servicio | Grupo | Sistema eléctrico |
|---|---|---|
| Quirófano / híbrido | 2B | Red IT |
| UTI / UCIP / Neonatología | 2B | Red IT |
| Unidad Coronaria | 2B | Red IT |
| Hemodinamia | 2 | Red IT |
| Sala de parto | 2A | Red IT |
| Cesárea | 2B | Red IT |
| Cirugía ambulatoria | 2 | Red IT |
| Shock room (guardia) | 2 (criterio) | Red IT/segura |
| Atención RN | 2 | Red segura |
| Terapia intermedia | 1 | TT/TN |
| RX / TC / RM (diagnóstico) | 1 | TT/TN (UPS en TC/RM) |
| Ecografía | 0–1 | TT/TN |
| Internación / pediatría | 1 | TT/TN |
| Esterilización / generales | 0 | TT/TN |

## Gases por servicio (bocas en cabecera)

| Servicio | O₂ | Aire | Vacío |
|---|---|---|---|
| UTI (748) | 2 | 1–2 | 2 |
| UCIP (747) | 2 | 1–2 | 1–2 |
| Neonatología (306) | 2 | 1 | 1 |
| Quirófano polivalente (810) | 2 | 1 | 2 |
| Quirófano híbrido (810) | 2 | 2 | 2 |
| Atención RN (810) | 1 | — | 1 |
| Recuperación (810) | 1 | 1 | 1 |
| UCO cardiología (375) | 2 | 1 | 1 |
| Internación (2547) | sí | — | sí |

## Climatización por servicio

| Servicio | T [°C] | HR [%] | Renov/h | Presión |
|---|---|---|---|---|
| Quirófano (810) | 20–24 | 30–60 (50–55) | 15–20 | positiva |
| UTI (748) | 24–26 | 30–60 | 4 hab / 2 resto | +/– según aislam. |
| Neonatología (306) | 25–26 | — | — | — |
| Atención RN (810) | 28 (+37 radiante) | — | — | — |
| Shock room (428) | 25–26 | 30–60 | 2 | — |
| Observación guardia (428) | 24–25 | — | — | — |
| RX / TC (3590) | 20–24 / 20–22 | 40–60 | — | — |
| Ecografía (3590) | 22–24 | — | — | — |

## Planta física — superficies mínimas de referencia

| Servicio | Superficie |
|---|---|
| Quirófano polivalente | 20 / 24 / 30 / 36 m² (laminar 40 / 48) |
| Quirófano híbrido | ≥50 m² (arco C) / ≥70 m² (resonador) |
| Cesárea | ≥24 m² |
| UTI | ≥9 m²/cama ×2 (nuevas 12) |
| UCIP | ≥7 m²/cama abierta / ≥9 m² individual |
| Neonatología | 2,8 m²/paciente (aislam. 24 m²) |
| UCO | ≥9 m²/box ×2 |
| Hemodinamia | ≥30 m² (sala de procedimiento) |
| Shock room | ≥12 m²/cama |
| Observación guardia | 6 m²/cama |
| Parto | 16 m² · Preparto 9 m² |
| Internación individual / doble | 20 / 26 m² |
| Cirugía ambulatoria | ≥12 m² |

---

_Última actualización: 2026-07-28. Se agregó a cada ficha la **Definición** del servicio y sus **Locales médicos** (con el tipo de local de cada ambiente), y se corrigió **internación** a **Grupo 1** (antes Grupo 0) en fichas 17 y 18, la tabla AEA 1.1 y la tabla comparativa. El tipo de cada local se asigna aplicando las definiciones de 1.1; los ambientes no médicos (comando, office, espera) quedan fuera del alcance de la AEA. Los datos marcados **[no en resúmenes]** requieren abrir el PDF fuente citado en `INDICE.md`._

