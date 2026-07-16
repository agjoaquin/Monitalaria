# Instalaciones eléctricas a baja tensión
Fuentes (7 archivos en `Clases actualizadas/Instalaciones electricas a baja tensión/`):
- `Instalaciones eléctricas clase 1.pptx.pdf` (22 pág) — AEA 710, grupos de salas, macro/microchoque, componentes, dimensionamiento
- `Protecciones_ Red TT.pptx.pdf` (15 pág) — fallas y protecciones (térmica, termomagnética, diferencial)
- `Puesta a tierra.pptx.pdf` (35 pág) — PAT, jabalinas, equipotencialización, AEA 90364-710
- `Red IT.pptx.pdf` (17 pág) — sistema IT aislado para salas grupo 2
- `03_Instalación Red TT_2025.pdf` (18 pág) — ejemplo consultorio: circuitos, secciones
- `05_Servicio Radiología.pdf` (32 pág, imágenes) — acometida, sala de examen, tableros, reveladoras
- `10_Miniductos, Poliductos y Torretas_2025_Campus.pdf` (18 pág, imágenes) — paneles de cabecera

## Reglamentación AEA 710 (clase 1, pág 2-3)
AEA (con IRAM, vía CEA, parte de IEC). Aplica a salas de uso médico/dental, hidroterapia, fisioterapia, masajes. NO son sectores médicos: pasillos, escaleras, baños, cocinas, salas de espera, administración, oficinas.

## Clasificación de salas por grupo de aplicación (clase 1, pág 4-7)
- **Grupo 0**: paciente no contacta equipos electromédicos de red (o solo a batería); una 1ª falla y desconexión automática no es riesgo.
- **Grupo 1**: paciente contacta partes de equipo conectado a red; la discontinuidad NO es riesgo vital.
- **Grupo 2**: equipos para intervenciones/mediciones vitales; no puede interrumpirse.
  - **2A**: sigue funcionando ante 1ª falla a tierra o corte de red; sin riesgo de microchoque.
  - **2B**: además, paciente expuesto a **microchoque**; difiere en el tipo de monitor de aislación.

## Seguridad eléctrica (clase 1, pág 8-9)
- **Macrochoque**: contacto externo (piel intacta) con elemento bajo tensión.
- **Microchoque**: corriente accede al interior del cuerpo por dispositivo conductor (catéter) próximo al corazón; **corrientes del orden de µA** pueden provocar **fibrilación ventricular**.

## Componentes de la instalación (clase 1, pág 10-13)
Acometida → líneas de alimentación → tablero principal (centro de distribución, aloja protecciones) → líneas seccionales → tableros seccionales → líneas de circuitos → consumos.

## Clasificación de circuitos (clase 1, pág 14)
- Uso general (máx **15 bocas**): iluminación IUG, tomacorrientes TUG.
- Especiales TUE: por función o por potencia (consumo >10 A).
- Dedicados/fijos: alimentan una sola carga.

## Dimensionamiento de conductores (clase 1, pág 15-17)
Determinar sección del conductor y, a In, la protección contra sobrecorrientes. Verificar por **al menos 2** de: cálculo térmico, caída de tensión, económico, resistencia mecánica.
### Secciones mínimas [mm²]
| Tipo de línea | Tramo | Sección mín |
|---|---|---|
| Principal | medidor–tablero principal | 4 |
| Seccional | tablero ppal–seccionales | 2,5 |
| Circuito | seccional–tomacorrientes | 2,5 |
| Circuito | bocas de luz | 1,5 |
| Derivación/retorno | boca de luz–llave | 1 |
| Conductor de protección | todos | 2,5 |

## Requisitos por grupo de sala (clase 1, pág 18-19)
- **Grupo 0** (710.4.3.3): mín 4 TUG y mín 1 IUG por consultorio; TUG e IUG de circuitos distintos (máx 15 bocas); AA → a TUE.
- **Grupo 1** (710.4.3.4): mín 4 TC (tomas de cabecera) por cama; mín 2 TUG cada 4 camas; 1 luz de examen por cama; mín 2 IUG (1 cada 12 m²); TUG e IUG de 2 circuitos; identificar TC normal y de emergencia (rojo).

## Ejemplo Red TT — consultorio (archivo 03, pág 6-7)
- C1 (TUG): 15 tomacorrientes, 2,5 mm², Imáx 18 A, In TMG 16 A.
- C2 (IUG): 7 bocas, 1,5 mm², Imáx 13 A, In 10 A.
- C3 (TUE): 2 tomacorrientes, 4 mm², Imáx 24 A, In 20 A.
- Pasos de diseño: (1) clasificación de servicio/local, (2) distribución de cargas en croquis, (3) descripción de circuitos, (4) distribución de conductores, (5) diseño del tablero (protecciones + PAT).

## RED TT (Protecciones, pág 2-3)
Sistemas BT según puesta a tierra: **TT, TN, IT**. TT: neutro del sistema directamente a tierra + carcasa del equipo directamente a tierra.

## Fallas y protecciones (Protecciones, pág 4-13)
- **Fallas**: sobrecorrientes (sobrecarga <100% In; cortocircuito >>In), sobretensiones (maniobras/rayos), fugas de corriente.
- **Relé térmico**: protege ante sobrecargas pequeñas prolongadas (motores).
- **Interruptor termomagnético**: sobrecargas por efecto **térmico** (bimetal) + cortocircuito por efecto **magnético** (bobina). Curva: zona A térmica, zona B magnética, zona C transición.
  - Tipo B: 3–5×In (sin arranque de motores). Tipo C: 5–10×In (el más usado). Tipo D: 10–20×In (motores de inercia, transformadores).
- **Disyuntor diferencial**: aguas abajo; protege contra contactos directos/indirectos y derivaciones a tierra. Suma de corrientes de línea = 0; sensibilidad habitual **30 mA**; reacción no inferior a 30 ms. Clasificación por fases, tensión (230/400 V), In, sensibilidad, tiempo.

## Puesta a tierra — PAT (archivo Puesta a tierra, pág 2-33)
### Tipos (pág 3-4)
- **PAT de servicio**: conecta el neutro a electrodo; estabiliza potencial, evita sobre/subtensiones, disipa corrientes de retorno.
- **PAT de protección**: conecta a tierra todas las masas metálicas; dirige corrientes de fuga a tierra; evita diferencias de potencial peligrosas.
### Tierra de instalación (pág 8)
Conductor perimetral en fondo de cimientos. Materiales: cobre electrolítico desnudo **35 mm²** (IRAM 2022, alambres ≥1,80 mm); o acero-cobre 5 mm (40% conductividad); o planchuela de cobre 20×3 mm. En anillo/malla; caja de inspección cada 30 m; uniones por soldadura (no roscadas/abulonadas). **Resistencia a tierra ≤ 2 Ω.**
### Factores de la RPAT (pág 9-16)
- Efecto suelo: mayor R cerca del electrodo; a 2,5 m el efecto ≈0; jabalinas en paralelo a **4 m** entre sí.
- Diámetro jabalina: de ½" a ¾" solo baja R ~10%; >¾" no conviene.
- Forma: la jabalina es ideal (0,12 m² vs 1,66 m² de placa para RPAT=5 Ω en suelo 15 Ω·m).
- Profundidad: máxima disminución entre **1,5 y 3 m**; >5 m poco útil; mejor poner en paralelo.
- Humedad óptima **30–35%**; por debajo de 20% sube mucho la R.
- Temperatura: incidencia mínima >0 °C; bajo -2/-3 °C sube la resistividad.
- Jabalinas en paralelo: RPAT = K·Rindiv; K: 2→0,57; 3→0,42; 4→0,33; 5→0,27; 6→0,24; 7→0,21; 8→0,19; 9→0,17; 10→0,15 (tabla completa, `Clases actualizadas/Guía de práctica/Guía de práctica 2026.pdf`).
### Conductores de protección (pág 18)
IRAM 62267, bicolor verde/amarillo. Secciones mín: PEH circuitos (TUM) = igual al neutro; PEH masas extrañas 4 mm²; PEHs seccionales 6 mm²; PEHp principales 25 mm².

## AEA 90364-7-710 — equipotencialización salas grupo 2 (Puesta a tierra pág 19-31)
- PAT de protección del inmueble es **única**; debe existir **Barra Equipotencial Principal (BEP)**.
- En zona de seguridad del paciente, la diferencia de potencial entre masas **no debe superar 20 mV** (verificado en funcionamiento sin falla).
- Equipotencialización radial con conductores **PEH** desde una **BPATH** (barra hospitalaria); un PEH por punto.
- Deben equipotencializarse (si tienen borne accesible): borne PE de todo TUM, piso semiconductivo (2 puntos), mesa de cirugía, cama, mesas de apoyo, luminaria scialítica, torre quirúrgica/monitoreo, poliducto metálico, cañería de gases medicinales, cañería de agua, ductos de climatización, marcos de puertas/ventanas.
- Evitar unir PEH con PE; pieza aislante (corte galvánico) en cañerías que ingresan; único punto de vinculación = BEP del edificio.
- Protección contra rayos: DPS primarios/secundarios según análisis de riesgo.
- Bibliografía: AEA 90364 Parte 7 Sec. 710 ed. 2024; AEA 95501-2/IRAM 2281-2 (2021).

## RED IT — suministro aislado salas grupo 2 (archivo Red IT, pág 2-15)
- Tres funciones ante 1ª falla a tierra: seguridad eléctrica del paciente, continuidad del suministro, evitar explosión/incendio.
- Conductores activos separados de tierra (o a tierra vía impedancia); ante fallo solo circula corriente pequeña (capacidad de derivación).
- Tableros IT propios por sala (no compartidos); doble alimentación (preferencial + alternativa) con separación física/dieléctrica; montaje externo, próximo a la sala, fuera del área limpia.
- Salas grupo 2 con **>4 puestos** no pueden tener un solo sistema IT.
- **Tablero de aislación** (4 partes): conmutación red principal/alternativa; **transformador de aislación**; **monitor de aislación (IMD)** + repetidor; mando/control/protección.
- Transformador (AEA 90364-7-710): monofásico, aislación seca, **3,15–8 kVA** (5 kVA preferido para UTI y quirófanos).
- Monitor de aislación: vigila impedancia de pérdida / corriente de fuga y alarma ante deterioro.
- Distribución de circuitos en grupo 2: IUG (½ de bocas desde UPS), TUG (1 cada 12 m², mín 2 por puesto, fuera del área paciente, color distinto), TUE, TUM (mín 12 por puesto en ≥2 circuitos de ≤6 TUM); scialíticas alimentadas desde red IT.
- Estimación de consumos: **600 W/cama**; **1500 W/puesto neonatología**; 2000 W adicional.

### Arquitectura general de la instalación — Red pública/GE → esencial/no esencial → grupos (archivo Red IT, última diapositiva antes de las de cierre, ~pág 15, diagrama "Instalación hospitalaria completa")
- **Red Pública** y **Grupo Electrógeno (GE)** confluyen en un **analizador de redes** (relés de tensión y corriente) que selecciona la fuente y alimenta la barra **Esencial**. La Red Pública, además, alimenta directamente (sin pasar por GE) la barra **No esencial** (cargas sin respaldo ante corte: auditorios, cafetería, sala de espera, compresor de vacío, suministro de agua, iluminación de emergencia como fuente redundante — coherente con "servicios no críticos" de `alimentacion-de-emergencia.md`).
- Desde **Esencial**: alimenta **UPS on-line** y, según el sistema de puesta a tierra, se reparte en dos ramas:
  - **TT/TN/TNS** → **Grupo 0** (consultorios, salas de esterilización/internación) y **Grupo 1** (ecografía, masajes, terapia física).
  - **Aislado IT** → **Grupo 2A** (diálisis, endoscopia, resonancia magnética, sala de parto) y **Grupo 2B** (post-operatorio, terapia intensiva, neonatología, cardiovascular, quirófano), cada uno con **vigilancia de aislamiento**: el monitor de aislación integra un medidor de impedancia (**Z**) que vigila la red IT y un **repetidor (R)** visible en la sala (parte del "tablero de aislación" ya descripto arriba, no un cableado aparte desde cada equipo de la sala).
- Denominación de red: **Red TT** desde la acometida hasta el tablero de aislación; **Red IT** de ahí en más (cambia justo en el tablero de aislación, por el transformador de aislación que allí se aloja).

## Servicio de Radiología (archivo 05, imágenes)
Normativa: PNGCAM Res. 610/2004 y Res. 3590/2021. Contenido gráfico: transformador, pilar de acometida, acometida al servicio, sala de examen y comando, tablero seccional, revelado manual/automático, digitalizador CR e impresora. (Ver detalles de requisitos por modalidad en `servicios-hospitalarios-resoluciones.md`.)

## Miniductos, poliductos y torretas (archivo 10, imágenes)
Paneles de cabecera: **miniducto** (gases y eléctrico separados), **poliducto** (columna mural con bocas de gases + tomas), **torreta** (de techo). Contenido principalmente fotográfico (mismo material que `10_Redes Gases Medicinales`).

---
# Complemento — Guía de práctica (Guías Nº 1, 2 y 3)
Fuente: `Clases actualizadas/Guía de práctica/Guía de práctica 2026.pdf`

## Guía 1 — Locales hospitalarios (pág 2)
Tabla de grupos de aplicación AEA 90364-7-710 usada en la guía = la misma clasificación ya resumida arriba ("Clasificación de salas por grupo de aplicación"). Sin datos normativos nuevos; ver también `estructura-hospitalaria.md` (definición de hospital, PNGCAM) y `servicios-hospitalarios-resoluciones.md` (definición y locales de cada servicio).

## Guía 2 — Sistemas de red TT/TN/IT, ampliado (pág 3-5)
- **TT**: neutro de la distribuidora puesto rígidamente a tierra (centro de estrella del transformador); el conductor de protección lo provee el usuario desde su propia PAT. Es el sistema empleado en Argentina, trifásico 3×380/220 V. **Nunca usar el neutro de la distribuidora como conductor de protección** (por desequilibrios/terceras armónicas puede quedar a potenciales >24 V respecto de tierra, la máxima tensión de contacto admitida).
- **TN**: poco usado en el país (motivos técnicos/económicos).
- **IT**: tres fases activas (RST), neutro no rígidamente conectado a tierra (aislado o vía impedancia elevada). Es la base del sistema de red aislada para salas grupo 2.

## Transformadores de aislación de uso médico — especificación técnica completa (AEA 90364-7-710, IEC 61558-2-15) (pág 5-6)
Amplía lo ya resumido: deben satisfacer salas grupo 2 (a y b) porque en ellas es indispensable la red aislada IT para dar suministro seguro a equipos electromédicos soporte de vida. Una red aislada previene el **macrochoque** (continuidad de servicio ante 1ª falla) y, con monitor de aislación + estructura equipotencial, el **microchoque**.
Características técnicas exigidas (Sección 710):
1. Monofásico, aislación seca.
2. Rango de potencia: **3 – 8 kVA** (5 kVA preferido para UTI y quirófanos).
3. Relación 1:1, tensión nominal máx **230 Vca**.
4. Corriente de vacío < **3% Inom**.
5. Corriente de conexión < **12×Inom**.
6. Tensión de cortocircuito < **3%** de la nominal.
7. Clase térmica **H**.
8. Nivel de aislación **3 kVca**.
9. Rigidez dieléctrica > **500 MΩ**.
10. Corriente de fuga a tierra < **0,1 mA**.
11. Nivel de ruido < **40 dB** a 30 cm, a potencia nominal.
12. Pantalla electrostática entre primario y secundario.
13. Conexión para monitoreo de fuga a mitad del bobinado secundario, a borne aislado.
14. Sensor de temperatura tipo PTC o PT100.
15. Elevada capacidad de sobrecarga.

**Protección del transformador de aislación (710.4.3.5.7)**: en el primario solo se admite protección contra cortocircuito (apertura de la alimentación). En el secundario: si tiene una sola salida, solo protección contra cortocircuito; si tiene más de una salida, protección contra sobrecarga **y** cortocircuito.

### Consideraciones generales de redes IT (ampliación)
- ≥1 red IT propia por sala grupo 2; nunca un único transformador para 2+ salas (aumenta la capacidad distribuida a tierra).
- Tablero del sistema IT lo más cerca posible de la sala; **longitud del secundario a la carga ≤ 50 m**.
- Salas >1 paciente (esp. UTI): recomendado no alimentar más de 4 camas con una misma red IT; en salas >4 camas, disposición alternada (cruzada) de las redes IT.
- Tomacorrientes de la red IT deben identificarse claramente.

## Requisitos AEA por grupo de sala — ampliación con datos de la guía (pág 9)
### Grupo 1
- Mín. **4 tomacorrientes de uso médico por cama**, desde 2 circuitos independientes, **al menos 2 de ellos alimentados desde el sistema eléctrico de emergencia**.
- Mín. **2 TUG cada 4 camas** + **1 IUG cada 12 m²** de superficie de sala.
- 1 boca de iluminación para luz de examen por cama/puesto.
- Si hay AA y/o calefacción eléctrica individual: mín. 1 TUE.
### Grupo 2
- Red IT para tomas de uso médico; no alimentar >4 camas por red IT en salas multipaciente.
- Salas de pacientes críticos (cirugía, terapia, neonatología): tomacorrientes de cada cama divididos en ≥2 circuitos; **máx. 6 tomacorrientes por circuito** en cada panel.
- **≥12 tomacorrientes** en paneles de cabecera de UTI (adulto/pediátrico); **≥18** en neonatología.
- Si se necesitan más de 2 circuitos por puesto (equipos dependientes de red para intervenciones/soporte vital): alimentación alternada (cruzada) desde 2 redes.
- Consumo aproximado por panel: **600 W** (crítico adulto/pediátrico), **1500 W** (neonatología).
- Luminarias alimentadas de **≥2 circuitos de iluminación independientes**.

## Cálculo por caída de tensión (pág 11-13)
Línea abierta de sección uniforme (alimentada por un extremo). Caída de tensión absoluta total en el conductor completo (ida + vuelta):

**δ = 2 · I · (l/s) · ρ**
donde δ = caída absoluta [V], I = corriente [A], l = longitud [m], s = sección [mm²], ρ = resistividad del conductor.

**⚠️ Ojo con el "×2" — quándo corresponde y cuándo no**: esta fórmula es de caída de tensión de una línea **monofásica** cerrada en lazo (la corriente va por un conductor y vuelve por el otro, por eso 2×longitud). El resumen no tiene una fórmula de caída de tensión trifásica propia. Si un dato de un enunciado pide una **resistencia simple de un conductor** (p. ej. "R aparente" o "resistencia de conductor" de una bajada, sin mencionar caída de tensión ni lazo), **no corresponde duplicar la longitud** — se usa la definición directa R=ρ·L/S con L=la longitud real del tendido, aunque el circuito sea trifásico. Duplicar solo tiene sentido cuando se calcula explícitamente la caída de tensión de un lazo cerrado ida-vuelta.

- A UI (generador) constante, si aumenta I entonces disminuye UII (tensión en el receptor).
- **Caída de tensión porcentual (Pu)**: referida a UII (tensión del receptor).
- Relación con la **pérdida porcentual de potencia (Pp)**: a partir de Pu o Pp (datos habituales) se despeja la sección:
  **S = Pii · l / (Pu · Uii²)** (forma general; Pii = potencia en bornes de la carga [W], Ui/Uii en V, S en mm²) — ver PDF pág 12 para el desarrollo completo si se necesita la deducción paso a paso.
- **Máxima caída de tensión admisible (AEA)**: motores, **5%** en operación continua y **15%** en el arranque.

## Cálculo térmico / capacidad de conducción de corriente (pág 13-14)
La corriente que produce el "equilibrio térmico" a la temperatura máxima de servicio continuo define la **capacidad de conducción**. En la práctica se usan tablas de fabricante (referidas a tensión nominal y condiciones de instalación típicas: cañería embutida para unipolares, aire libre o enterrado para subterráneos).

### Tabla IRAM 2183 — cables unipolares aislados en PVC (cañería embutida o vista)
| Sección [mm²] | Ø ext. aprox. [mm] | Peso [kg/km] | I adm. en cañería [A] | I adm. al aire libre [A] | Caída tensión [V/A·km] | Resist. máx. 20°C CC [Ω/km] |
|---|---|---|---|---|---|---|
| 0,75 | 2,4 | 12 | 8 | 10 | 50 | 26 |
| 1,0 | 2,8 | 16 | 10,5 | 12 | 37 | 19,5 |
| 1,5 | 3,0 | 21 | 13 | 15,5 | 26 | 13,3 |
| 2,5 | 3,7 | 32 | 18 | 21 | 15 | 7,98 |
| 4 | 4,2 | 46 | 24 | 28 | 10 | 4,95 |
| 6 | 4,8 | 65 | 31 | 36 | 6,5 | 3,3 |
| 10 | 6,1 | 110 | 42 | 50 | 3,8 | 1,91 |
| 16 | 7,9 | 185 | 56 | 68 | 2,4 | 1,21 |
| 25 | 9,8 | 290 | 73 | 89 | 1,54 | 0,78 |
| 35 | 11,1 | 390 | 89 | 111 | 1,2 | 0,554 |
| 50 | 13,6 | 550 | 108 | 134 | 0,83 | 0,386 |
| 70 | 16,1 | 785 | 136 | 171 | 0,61 | 0,272 |
| 95 | 18,3 | 1000 | 164 | 207 | 0,48 | 0,206 |
| 120 | 19,7 | 1250 | 188 | 239 | 0,39 | 0,161 |
(Condiciones: 3 cables en cañería o al aire, plano, 30 °C, no se cuenta el de protección; caída de tensión con CA monofásica 50 Hz, cos φ=0,8.)

**Coeficientes de corrección de la I admisible**: 2 cables en cañería ×1,10; 4-6 cables ×0,8; 7-9 cables ×0,7; al aire libre ×1,12; temperatura ambiente 40 °C ×0,89.

## Fuerza motriz y factor de potencia (pág 15-16)
Fuerza motriz (motores de ascensores, bombas, AA, compresores, etc.): conductores independientes del alumbrado, protección propia por circuito. Distribución trifásica 3×380 V (la monofásica en potencias altas exige secciones mayores). El cálculo del ramal es igual al de una línea seccional: sección a In + verificación por caída de tensión.
- **Factor de potencia**: cos φ = potencia activa / potencia aparente.
- **Potencia trifásica**: St = √3·VL·IL [VA]; Pt = √3·VL·IL·cos φ [W] (válida en triángulo o estrella).

## Elementos de protección — ampliación (pág 18-25)
- **Fusibles**: rápidos (fusión instantánea) o retardados (fusión demorada, usados en protección de motores con corrientes de arranque elevadas). Capacidad de ruptura ≥ la calculada en el punto de utilización.
- **Norma IRAM 2169** (basada en IEC 898): interruptores automáticos de sobreintensidad para uso doméstico/similar. Aplica a ruptura en aire, CA 50/60 Hz, tensión <440 V entre fases, In <125 A, capacidad de cortocircuito <25 kA.
- **Corriente nominal del interruptor termomagnético**: no debe exceder en más de **25%** la corriente de carga nominal del circuito. Serie preferencial: **5-10-15-20-25-32-40-50-63-80-100 A**.
- **Capacidad de cortocircuito nominal**: valores normales **1,5 – 3 – 4,5 – 6 – 10 – 20 kA**.
- **Criterio de selección de la protección térmica** (una vez elegida la sección por corriente de carga):
  1) **Ic ≤ InI ≤ Iadc**
  2) **Ift ≤ 1,45·Iadc**
  donde Ic = corriente de carga, InI = corriente nominal del interruptor, Iadc = corriente admisible del conductor, Ift = corriente de funcionamiento de la protección térmica en <1 h. Como el fabricante garantiza Ift ≤1,45·InI, al cumplir 1) se cumple automáticamente 2).
- **Interruptor diferencial**: normas **IRAM 2301 / IEC 1008**; actúa a partir de fuga ≥30 mA en ≤0,03 s. Sensibilidades de fabricación habituales: **30 mA** (protección de personas) y **300 mA** (solo protección contra incendio/uso industrial, no protege personas). Funciona por suma vectorial de corrientes de línea = 0 en condición normal; ante fuga, un transformador toroidal induce una FEM que dispara un relé polarizado (tiempo máx. de apertura 0,03 s). Debe combinarse con protección de sobrecarga/cortocircuito (fusible o termomagnético), antes o después según conveniencia/normativa.

### Coordinación (selectividad) de protecciones (pág 23-24)
Objetivo: que ante una falla se abra solo la protección más próxima a ella (aguas abajo), sin afectar el resto del sistema. Técnicas: **selectividad amperométrica** (separar umbrales de disparo instantáneo/corto retardo; usada en distribución terminal) y **selectividad cronométrica** (escalonar tiempos de disparo).
Reglas prácticas de coordinación:
- Fusible con fusible: **Infa > 1,6·Infp** (recomendado >2×); Infa = fusible más alejado de la carga, Infp = más cercano. Ej.: cercano 16 A, alejado 25 A.
- Fusible con interruptor termomagnético: **Inf > 1,2·InfI**.
- Termomagnético con termomagnético: **Ina > 2·Inp** (Ina alejado, Inp cercano; si los térmicos son regulables, usar la corriente térmica ajustada).
La protección magnética (instantánea) es difícil de coordinar en corrientes altas por no tener temporización; conviene separar lo más posible los umbrales de disparo magnético.

### Dimensionamiento típico de tablero
Esquema general: (1) fusible de la distribuidora (ej. 100 A) → (2) medidor → (3) interruptor termomagnético bipolar (tablero principal) → (4) interruptor diferencial 30 mA (tablero seccional) → (5) interruptores termomagnéticos bipolares por circuito.

### Valores comerciales de referencia (ejemplo Siemens, catálogo)
- **Termomagnéticos**: capacidad de ruptura 3 kA (residencial), 6 kA (comercial), 10 kA (industrial/altas corrientes); curvas B/C/D según IEC 60898; corrientes nominales disponibles de 0,5 a 125 A; ejecuciones uni/bi/tri/tetrapolar.
- **Diferenciales**: bipolares y tetrapolares; corrientes nominales 16/25/40/63/80/125 A; sensibilidades 10/30/100/300/500/1000 mA; disparo instantáneo, selectivo o de retardo breve.

## Puesta a tierra — fórmulas de cálculo de electrodos (Guía 3, pág 33-36)
Complementa la sección de PAT ya resumida (factores de la RPAT, PEH, equipotencialización).

### 1. Picas/jabalinas
- **Método convencional**: Rt = ρ/L (ρ = resistividad del terreno [Ω·m], L = longitud de la jabalina).
- **Método de Dwight**: Rt = 0,366·(ρ/L)·log₃(L/d) (d = diámetro de la jabalina).
- **Tabla práctica de RPAT** con jabalina de 16 mm Ø, hincado directo, suelo homogéneo (Norma IRAM 2281):

| Largo jabalina [m] | 10 Ω·m | 15 | 20 | 25 | 30 | 35 | 40 | 45 | 50 | 55 |
|---|---|---|---|---|---|---|---|---|---|---|
| 1,50 | 7,12 | 10,68 | 14,24 | 17,80 | 21,36 | 24,92 | 28,48 | 32,04 | 35,60 | 39,16 |
| 2,00 | 5,57 | 8,35 | 11,14 | 13,92 | 16,71 | 19,49 | 22,28 | 25,06 | 27,85 | 30,63 |
| 3,00 | 3,93 | 5,89 | 7,86 | 9,82 | 11,78 | 13,75 | 15,71 | 17,68 | 19,64 | 21,60 |
| 4,50 | 2,76 | 4,14 | 5,52 | 6,91 | 8,29 | 9,67 | 11,05 | 12,43 | 13,81 | 15,19 |
| 6,00 | 2,15 | 3,22 | 4,30 | 5,37 | 6,44 | 7,52 | 8,59 | 9,67 | 10,74 | 11,81 |
(valores de resistencia de PAT en Ω, para cada largo y resistividad tabulados; interpolar si no coincide exactamente)

- **Para ρ fuera de la tabla**: Rt = C·ρ, con C según tipo de jabalina: JL-16×1500 → 0,7123; JL-16×2000 → 0,5572; JL-16×3000 → 0,3930; JL-16×4500 → 0,2764; JL-16×6000 → 0,2149.
- **Terrenos heterogéneos (2 capas)**: si ρ2 < ρ1, longitud equivalente L' = (L−H) + (ρ2/ρ1)·H (H = profundidad de la capa superior, H>>d); por Dwight: R = 0,366·(ρ2/L')·log₃(L'/d); método aproximado: R = ρ2/L'. Si ρ1 < ρ2, se desprecia la parte enterrada en ρ2 → L' = H; por Dwight: R = 0,366·(ρ1/L')·log₃(L'/d); aproximado: R = ρ1/L'.
- **Jabalinas en paralelo**: Rpat = K·Rindiv, con distancia entre sí ≥4 m (tabla de K ya incluida arriba en "Factores de la RPAT").

### 2. Anillo
Método simplificado: **Rt = ρ/P** (P = perímetro del anillo).

### 3. Malla
Método simplificado: **Rt = ρ/L** (L = suma de todos los lados/longitud de conductores activos de la malla).

### Jabalinas normalizadas — IRAM 2309 (acero revestido de cobre, 254 µm)
| Denominación | Diámetro | Largo |
|---|---|---|
| JL 1015/1020 | 9,0 mm | 1500/2000 mm |
| JL 1415/1420/1430 | 12,6 mm | 1500/2000/3000 mm |
| JL 1615/1620/1630 | 14,6 mm | 1500/2000/3000 mm |
| JL 1815/1820/1830 | 16,2 mm | 1500/2000/3000 mm |

## Ejercicios de práctica (Guía de cátedra 2026)
Fuente: `Clases actualizadas/Guía de práctica/Guía de práctica 2026.pdf`. Enunciados resumidos; usar las fórmulas/tablas de este resumen y de `servicios-hospitalarios-resoluciones.md` para resolverlos. Ninguno de estos ejercicios tiene resolución modelo propia todavía (a diferencia de `Finales/finales-resueltos.md`); si se resuelven, agregar el criterio aplicado a ese banco.

### Guía 1 (pág 2)
1. Definir hospital; definir PNGCAM.
2. Definir y clasificar (grupo AEA 90364-7-710) cada servicio: UTI, terapia intermedia, pediatría, neonatología, cirugía, cirugía ambulatoria, internación, neumonología, cardiología, hemodinamia, guardia, maternidad, esterilización, diagnóstico por imágenes, servicios generales. *Nota: "neumonología" como servicio puntual no está desarrollado en `servicios-hospitalarios-resoluciones.md`; si se pide resolver, aclarar el faltante y no inventar cifras de superficie/gases para ese servicio.*
4. Definir el servicio de ingeniería de un hospital.

### Guía 2 (pág 29-31, laboratorio pág 31)
1. Diseñar circuitos eléctricos de un consultorio de guardia tipo (camilla, lámpara de pie, cardiodesfibrilador, nebulizador ultrasónico, aspirador, ECG, negatoscopio 2 cuerpos, AA frío-calor, iluminación general).
2. Servicio de radiología a 180 m del tablero de entrada; equipo RX 30 kW trifásico, R entre tablero principal y seccional ≤0,4 Ω. Calcular acometida y circuitos del servicio (procesadora 4 A/220 V; salas de estudio, revelado, secretaría, médicos).
3. Lavadero: 2 lavadoras 90 kg/2 HP, 4 centrífugas 30 kg/2 HP, 2 secadoras 60 kg/2 HP, 1 planchadora 80 kg/¾ HP (todo trifásico 3×380 V) + 12 tubos LED 10 W. Diseñar la instalación.
4. Esterilizador por vapor monofásico, resistencias 2300 W, ciclo 121 °C (calefacción 10 min, esterilización 10 min, secado 20 min); instalación con conductor 1,5 mm² e interruptor termomagnético 10 A (dispara en 18 min a 10,12 A). Graficar curva de funcionamiento y curva tiempo-corriente del interruptor; indicar si la instalación es correcta.
5. Esterilizador por vapor: consumo 6 kW por fase, cos φ 0,95, alimentación 3×380 V+N+T. Calcular sección del conductor y protección térmica.
6. Servicio de cirugía (1 quirófano mediana complejidad + 1 de cirugía ambulatoria): diseño eléctrico según normativa vigente.
7. Diseño eléctrico de UTI de 6 camas.
8. (Laboratorio) Armar circuito con protector térmico, variar carga y levantar curva de funcionamiento (≥3 mediciones); determinar corriente nominal. Conectar motor monofásico y medir corriente de arranque en vacío/carga; protegerlo con interruptor térmico y concluir.

### Guía 3 — Puesta a tierra (pág 37)
1. Quirófano con RPAT medida de 8 Ω (pica de 3 m, ρ=20 Ω·m). Proponer y calcular una mejora para bajar de 2 Ω.
2. UTI en planta baja: calcular electrodos (jabalinas) necesarios con datos de estudio de suelo (tabla resistividad/profundidad de capa: 20 Ω·m a 1,07 m; 10 Ω·m a 1,65 m; entre otros — terreno heterogéneo, usar fórmulas de Dwight para 2 capas).
3. Diseñar PAT de servicio de RX: bajada de línea directa, tensión de fase 370-400 V, Raparente <0,27 Ω, equipo 50 kW trifásico (carga considerada 30 kW durante 100 ms), protecciones mínimas (termomagnética trifásica + diferencial), RPAT <1 Ω, terreno ρ=15 Ω·m.

(Ejercicios de Guía 4 — Mando y maniobra: ver `automatismo.md`.)
