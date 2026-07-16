# Finales resueltos — banco de exámenes

Cada final: **enunciado completo transcripto** (texto, para no tener que abrir la foto/imagen — ahorra tokens en cada consulta) + resolución razonada citando `resumenes/<tema>.md`. Formato pensado para que el agente lo use como ejemplo al resolver un final nuevo o al generar ejercicios tipo. Fuente original (fotos) guardada en `Finales/<fecha>/` — solo hace falta abrirla si se necesita ver un plano/tabla no transcriptos acá.

---

## Final 20/02/2025
**✅ Revisado por el usuario, pregunta por pregunta, el 2026-07-15.**

Final de 6 preguntas, 100 puntos totales (25+15+15+10+20+15). Fuente: `Finales/2025-02-20/` (2 fotos). Sin plano — es 100% de datos/texto.

### Enunciado completo

**1) Diseñar la instalación eléctrica de un servicio de RX.** El fabricante del equipo realiza las siguientes especificaciones de preinstalación:
- Bajada de línea directa. Tensión de fase entre 370 y 400V.
- R aparente < 0,27 Ω (resistencia de conductor).
- El equipo es de 50 KW, trifásico, pero por su condición de trabajo se considerará una carga de 30KW, durante un tiempo de 100 mseg.
- Protecciones mínimas: llave termomagnética trifásica y disyuntor diferencial.
- La resistencia a tierra debe ser < 1 Ω.
- La mesa radiológica de tablero flotante es monofásica de 4,4 KW.

Consideraciones generales:
- El equipo digitalizador CR es monofásico y consume 0,30 KW en modo operación y 0,095 KW en stand by.
- El servicio cuenta con dos equipos de aire acondicionado que consumen c/u: 2,75 KW en frío y 2,4 KW en calor.
- La iluminación general se compone de 10 tubos led de 18 W.
- Posee 17 tomacorrientes para uso general.
- El servicio se encuentra a 540 mts lineales de la entrada de suministro eléctrico.
- El terreno adyacente al servicio es heterogéneo, con ρ1 = 30 Ωm y profundidad 1,7 m, y ρ2 = 8 Ωm.

*(25P)*

**2) Realice el croquis de una instalación eléctrica** desde el transformador de alimentación de la empresa distribuidora de energía, hasta la lámpara scialítica de un quirófano dentro de una Institución Nivel III de riesgo, e indique qué tipos de redes eléctricas existen allí, dónde se cambia la denominación y a qué se debe. Indicar también los tableros, si hubiere, en el trayecto. *(15P)*

**3) Luminotecnia**
a) Defina los diferentes tipos de iluminación que se encuentran en el quirófano, y señale las diferencias *(5P)*
b) Describa el/los método/s de cálculo *(10P)*

**4) Automatismo**
a) Describa los contactos principales y auxiliares de un contactor *(5P)*
b) Enuncie las características a indicar para comprar un contactor *(5P)*

**5) La unidad coronaria de la Institución se compone de 10 camas, dispuestas en U sobre los laterales de la sala (4, 2, 4).**
a) Realice el diseño completo de la instalación de gases medicinales *(15P)*
b) Sabiendo que el consumo de aire medicinal del servicio de UCO representa un 25% del consumo total de la Institución, y el de UTI (14 camas) el 40%, ¿podría dimensionar la fuente adecuada a la norma IRAM 7396-1? Justifique detalladamente. *(5P)*

**6) Climatización:**
a) ¿Cuáles son las condiciones para climatizar un Quirófano y una sala de UTI según los requerimientos del PNGCAM? *(5P)*
b) ¿Cómo lo logra? Justifique *(10P)*

### Resolución (borrador sin revisar)

#### 1) RX — ✅ revisado por el usuario (2026-07-15)
Datos clave: ver enunciado. Suelo heterogéneo ρ1=30Ω·m (H=1,7m) / ρ2=8Ω·m. Servicio a 540m de la entrada de suministro.

**Clasificación del servicio**: sala de examen RX = **Grupo 1** AEA 710 (`servicios-hospitalarios-resoluciones.md` — Imágenes/RX: "Sala de examen Grupo 1"; también confirma trifásica 3×380V+N+T, potencias 50-80kW).

**Distribución de cargas (croquis)**: aplicando el paso 2 de la metodología de diseño del resumen (`instalaciones-electricas.md`, "Pasos de diseño": clasificación → croquis → circuitos → conductores → tablero), aunque el enunciado no adjunta plano ni lo pide explícitamente para este punto. Composición típica del servicio (`servicios-hospitalarios-resoluciones.md`): vestidor + sala de examen + sala de comando, separadas por vidrio plomado. Criterio de ubicación: equipo RX y mesa centrados en la sala de examen (ejes de disparo); consola y digitalizador CR en comando (operador fuera del haz); tablero seccional (TS-RX) en comando, junto al pasillo técnico (accesible sin interrumpir un examen, cerca de las cargas que alimenta); jabalina de PAT en el exterior pegada al TS-RX (conductor de tierra corto, en el terreno heterogéneo descripto); AA-1 en examen alejado del equipo (evita interferencia/corrientes de aire sobre el tubo) y AA-2 en comando; tomas TUG y luces IUG repartidas perimetralmente/en grilla de techo. La bajada directa dedicada del equipo RX entra aparte, sin pasar por el TS-RX (ver más abajo, motivo: especificación de fábrica).

**Circuitos** (criterio: separar por función y por régimen de uso, `instalaciones-electricas.md` clasificación de circuitos):
- **Dedicado equipo RX**: carga considerada 30kW trifásica (pico de exposición, 100ms), tensión de línea 370-400V. I≈30000/(√3·380)≈45,6A (cosφ=1, no hay dato de fp del equipo en el enunciado). Conductor y protección dimensionados por este pico, no por los 50kW nominales (la exposición es intermitente, se dimensiona por la corriente de operación real, no la de placa). **Sección 50mm² (ver justificación de la sección más abajo), TM trifásica 50A, diferencial tetrapolar 63A/30mA** (protección de personas — el enunciado exige diferencial explícitamente en el equipo).
- **Mesa radiológica + digitalizador CR combinados** (decisión propia, no exigida por norma en los resúmenes — justificada por factor de coincidencia: mesa a plena carga y CR en operación no suman su pico simultáneo pleno): I≈(4400+300)/(220×0,8)≈26,7A. **Sección 10mm², TM 32A.**
- **AA-1 y AA-2, circuitos TUE separados** (consumo >10A cada uno → no van a TUG, `instalaciones-electricas.md`): peor caso frío 2,75kW, I≈2750/(220×0,8)≈15,6A. **Sección 4mm², TM 20A c/u** (próximo valor comercial; el margen del 25% queda algo justo — 20/15,6≈1,28 — pero es la opción estándar inmediata superior y cumple Ic≤InI≤Iadc igual, criterio válido).
- **Iluminación**: 10×18W=180W → I≈0,8A. Un solo circuito IUG (**1,5mm², TM 10A**) — no se exige split en 2 circuitos porque la regla de "≥2 circuitos de iluminación independientes" del resumen aplica a salas de pacientes críticos Grupo 2 (cirugía/terapia/neonatología), no a Grupo 1; la redundancia la cubre la iluminación de emergencia del edificio.
- **Tomas**: 17 bocas > 15 (máximo por circuito de uso general) → **2 circuitos TUG (9+8), 2,5mm², TM 16A c/u** (mismo patrón que el ejemplo Red TT del resumen: TUG 2,5mm²/In16A).

**Conductor del dedicado RX a 540m — criterio de resistencia, no solo térmica**: el fabricante fija **R aparente <0,27Ω (resistencia de conductor)** (dato de preinstalación, junto con "bajada de línea directa") — interpretado como la resistencia de la línea que alimenta directamente al equipo a lo largo de los 540m (no de los demás circuitos, que son tiradas cortas desde el TS-RX).

*Nota sobre un error corregido en esta revisión*: en un primer cálculo se dobló la longitud (540m → 1,08km "ida+vuelta"), tomando prestada la convención de la fórmula δ=2·I·(l/s)·ρ del resumen — pero esa fórmula es de **caída de tensión de una línea monofásica** (el 2 sale de que la corriente va por un conductor y vuelve por el otro, cerrando un lazo de 2×L). El dato del enunciado no es una caída de tensión monofásica: es literalmente "resistencia de conductor" de una línea trifásica, es decir R=ρ·L/S de un solo conductor, con L=540m sin duplicar (el resumen no tiene una fórmula de caída de tensión trifásica propia; ante esa falta de dato, corresponde ir a la definición directa de resistencia de un conductor, no importar la convención de una fórmula distinta). **Regla para no repetir el error: la duplicación de longitud (ida+vuelta) solo aplica cuando se calcula la caída de tensión de un lazo cerrado (ida por un conductor, vuelta por otro, típico en monofásico); para una resistencia simple de conductor (como esta R aparente) o para razonamientos trifásicos sin neutro, se usa la longitud real del tendido sin duplicar.**

Con la tabla IRAM 2183 (columna Resist. máx. 20°C, `instalaciones-electricas.md`), a 540m (0,540km, sin duplicar): 35mm² → 0,554×0,540=0,299Ω (no cumple, por poco); **50mm² → 0,386×0,540=0,208Ω <0,27Ω (cumple)**. Sección final del dedicado RX: **50mm²** — sobredimensionada para la térmica (Iadm=108A contra 50A de protección) pero es el criterio de resistencia el que gobierna a esta distancia (verificación por ≥2 métodos, el más restrictivo define la sección, `instalaciones-electricas.md` pág 34).

**PAT — suelo heterogéneo, R<1Ω exigido**: ρ2<ρ1 → longitud equivalente L'=(L−H)+(ρ2/ρ1)·H (`instalaciones-electricas.md`, terrenos heterogéneos). Con jabalina normalizada L=3m (IRAM 2309): L'=(3−1,7)+(8/30)×1,7=1,753m.
- **Método aproximado** (R=ρ2/L', el que se puede aplicar en el final sin fórmulas a mano): Rind≈8/1,753≈4,56Ω. Jabalinas en paralelo (Rpat=K·Rind): n=6 (K=0,24) → 1,09Ω (no alcanza); **n=7 (K=0,21) → 4,56×0,21≈0,96Ω <1Ω → 7 jabalinas de 3m, separadas ≥4m entre sí.**
- **Método de Dwight** (más preciso, referencia — no usado como respuesta final del examen por no poder consultar la fórmula durante el final): R=0,366·(ρ2/L')·log₁₀(L'/d), con d=16mm → Rind≈3,4-4,2Ω según el diámetro exacto asumido; con ese rango, entre 5 (K=0,27) y 7 jabalinas ya verifican R<1Ω. Se deja aclarado en la resolución que el valor puede variar con el método más preciso, y que el aproximado (7 jabalinas) es el que se sostiene como respuesta de examen.

**Tablero seccional TS-RX (protección general)**: agrupa mesa+CR (32A), AA-1 (20A), AA-2 (20A), TUG1 (16A), TUG2 (16A), IUG (10A) — la bajada dedicada de RX NO pasa por acá. No hay coeficiente de simultaneidad citado en los resúmenes para tableros hospitalarios (mismo vacío de dato señalado en `alimentacion-de-emergencia.md`) → se suman las protecciones sin diversidad (criterio conservador, explícito). Repartiendo 2 circuitos por fase para balancear el trifásico: fase más cargada = mesa+CR+IUG = 42A → **TM general trifásico 50A** (serie preferencial). Diferencial general **300mA** (no 30mA: cada circuito individual ya lleva su propio diferencial de 30mA aguas abajo para protección de personas; el general en 300mA da selectividad — ante una fuga dispara primero el diferencial del circuito afectado, no el general — y protección contra incendio), In=**63A**.

#### 2) Croquis eléctrico transformador → scialítica — ✅ revisado por el usuario (2026-07-15)

Diagrama (esquemático/unifilar, no plano):

```
                    Transformador MT/BT (distribuidora)
                                  │  Red TT (acometida)
                                  ▼
                       TABLERO PRINCIPAL (TGBT)
                                  │
              ┌───────────────────┴──────────────────────┐
              │                                           │
        Red Pública ───────────────────────────►   NO ESENCIAL
              │                                    (auditorios, cafetería,
   Grupo      │                                     sala de espera, compresor
   Electrógeno┤                                     de vacío, agua — sin respaldo)
              │
              └──► ANALIZADOR DE REDES ──► barra ESENCIAL
                    (relés V/I; conmuta            │
                     Red o GE automático)           ▼
                                    TABLERO SECCIONAL BLOQUE QUIRÚRGICO
                                    (Red TT — alimentación preferencial
                                     de todos los quirófanos del bloque)
                                                     │
                     ┌───────────────────────────────┼────────────────────────────────┐
                     ▼                                                                 ▼
       Quirófano 1 — tablero local (Red TT)                       Quirófano 2 — tablero local (Red TT)
                     │                                                                 │
        ┌────────────┴────────────┐                               ┌────────────────────┴──────┐
        ▼                         ▼                                ▼                          ...
  TUG general Q1          TABLERO DE AISLACIÓN Q1 ◄── UPS       TUG general Q2         (ídem por cada
  (fuera área paciente,    on-line Q1 (alimentación               (fuera área          quirófano adicional
   diferencial 30mA)       alternativa)                            paciente)            — no compartidos)
                                  │
                    ├─ Conmutación preferencial/alternativa
                    ├─ Transformador de aislación 5kVA
                    ├─ Monitor de aislación: Z (mide impedancia) + R (alarma en sala)
                                  │
                        *** cambia a Red IT acá ***
                                  │
                ┌─────────────────┼──────────────────┐
                ▼                 ▼                   ▼
         IUG (½ bocas       TUM (≥2 circuitos,   LÁMPARA SCIALÍTICA
          desde UPS)         ≤6 tomas c/u)        (Red IT + UPS on-line
                                                   directo, por tiempo de
                                                   interrupción 0,15-0,5s)
```

**Recorrido y tableros**: transformador MT/BT de la distribuidora → tablero principal (Red TT desde acá) → bifurcación esencial/no esencial mediante analizador de redes (Red pública + GE, `instalaciones-electricas.md` "Arquitectura general...") → tablero seccional del bloque quirúrgico → tablero local por quirófano (Red TT) → bifurca en TUG general de esa sala (fuera del área del paciente, circuito propio con diferencial 30mA) y tablero de aislación de esa sala. **Un tablero de aislación por quirófano, no compartido entre salas** (`instalaciones-electricas.md`, Red IT: "tableros IT propios por sala, no compartidos"; salas grupo 2 con >4 puestos no admiten un solo sistema IT).

**Dónde cambia la denominación y por qué**: de Red TT a Red IT exactamente en el tablero de aislación de cada quirófano, por el transformador de aislación que allí se aloja. Motivo: en TT la primera falla a tierra dispara el diferencial y corta el suministro — inadmisible en una intervención en curso; la Red IT permite seguir operando ante esa primera falla (no se cierra un camino de baja impedancia hasta que ocurre una segunda falla).

**UPS on-line — ubicación**: entra como alimentación **alternativa** directo al tablero de aislación de cada quirófano (no al bus esencial compartido), junto a la alimentación preferencial (esencial/GE) — así lo indica la doble alimentación "preferencial + alternativa" del tablero de aislación (`instalaciones-electricas.md`, Red IT). Alimenta la mitad de bocas IUG y, en paralelo con la Red IT, la lámpara scialítica — porque su tiempo de interrupción admisible (0,15-0,5s, `luminotecnia.md`) es más corto que el tiempo de entrada en servicio del GE (<15s, `alimentacion-de-emergencia.md`); un UPS de esa escala dedicado a un solo quirófano es viable, uno para todo el bus esencial del hospital no lo sería.

**Z y R (monitor de aislación, dentro del tablero de aislación, no cableado aparte desde la scialítica)**: Z es el elemento que mide continuamente la impedancia entre los conductores activos de la red IT y tierra, inyectando una señal de prueba de baja intensidad; con el aislamiento sano esa impedancia es altísima (contacto no genera corriente peligrosa). Ante una primera falla a tierra, aparece una vía adicional de baja impedancia y Z detecta la caída, disparando una alarma sin cortar el suministro (el circuito sigue funcionando: solo una falla no cierra un cortocircuito real entre los dos conductores activos). R es el repetidor de esa alarma, instalado visible dentro del quirófano, que avisa al equipo médico para que termine la intervención con margen y repare antes de que una eventual segunda falla sí genere un cortocircuito real y corte el circuito.

#### 3) Luminotecnia — ✅ revisado por el usuario (2026-07-15)
**a) Tipos de iluminación en quirófano y diferencias**: general/ambiente (ilumina todo el local, sistema semidirecto/difuso para bajo deslumbramiento del cirujano, niveles ≥500 lux en salas anexas) vs. **localizada (scialítica)** sobre el campo operatorio (10.000-120.000 lux, sin sombras, sin calor, CRI>90, 4500K). Difieren en función (ambiente vs. campo quirúrgico), magnitud (cientos vs. decenas/cientos de miles de lux) y alimentación (general normal vs. Red IT+UPS+equipotencial para la scialítica). Fuente: `luminotecnia.md`.

**b) Método de cálculo**: **método de los lúmenes** para iluminación general — ya está el desarrollo completo de los 8 pasos en `luminotecnia.md` (Complemento — Guía de práctica): Φtotal=(E·S)/(η·fm), N°luminarias=Φtotal/(n·Φlámpara), verificación Ereal=N·Φlámpara·η·fm/S ≥ Eexigido. Aclaración importante: este método aplica solo a la iluminación general — la scialítica **no se calcula** con lúmenes, se selecciona de catálogo según tipo de intervención, altura de techo y nº de brazos/satélites (`luminotecnia.md`, "Lámpara scialítica — Selección").

#### 4) Automatismo — ✅ revisado por el usuario (2026-07-15)
**a) Contactos de un contactor** (`automatismo.md`, "Contactor — definición y construcción ampliada"): **contactos principales** — en las vías de conducción de la corriente de servicio, abren/cierran el circuito de potencia (carga: motor, alumbrado), 2 puntos de interrupción, abiertos en reposo, clasificados por nº de vías (bipolar/tripolar/tetrapolar, maniobra simultánea). **Contactos auxiliares** — acoplados mecánicamente a los principales (misma armadura), NA o NC, 2 puntos de interrupción, dimensiones reducidas (corrientes chicas, no la de la carga); función: enclavamientos y señalización.

**b) Características para comprar un contactor** (`automatismo.md`): tensión de la bobina de comando (12/24/110/220V CA o CC); cantidad de polos/vías del circuito de potencia según la carga a comandar; corriente nominal del circuito de potencia, considerando que el contactor debe soportar picos de 6 a 12 veces esa nominal; necesidad de protección adicional contra cortocircuito aguas arriba (el contactor no protege contra cortocircuito por sí solo); cantidad y tipo (NA/NC) de contactos auxiliares necesarios para los enclavamientos/señalización del circuito de mando. *(En la práctica de catálogo también se especifican otros datos — categoría de empleo, poder de corte, grado IP, vida eléctrica/mecánica — pero no están citados en el resumen de cátedra, así que se dejan fuera de esta respuesta.)*

#### 5) UCO — 10 camas en U (4,2,4) — ✅ revisado por el usuario (2026-07-15)
**a) Diseño instalación de gases medicinales** (Res. 375/2002 + IRAM-ISO 7396-1, `gases-medicinales.md`): por cabecera **2 O2 (una regulada por presión a 8bar, otra por caudal a 4bar — modelo por analogía con la fila de UTI de la tabla de la guía práctica pág 64, UCO no tiene fila propia) + 1 aire (8bar) + 1 vacío** → total 20 bocas O2 (10 a 8bar + 10 a 4bar), 10 aire, 10 vacío.

Caudales (CU=1): O2@4bar=10×7=70 l/min (4,2 m³/h); O2@8bar=10×20=200 l/min (12 m³/h); Aire=10×20=200 l/min (12 m³/h); Vacío=10×30=300 l/min (18 m³/h, P=0,65bar).

Diámetros (Dint=18,8·√(Q/(v·P)), v=8m/s O2/aire — **no 15m/s: la guía práctica aclara que 15 es el límite máximo a no exceder, 8 es el valor normal que da mayor coeficiente de seguridad** —, v=100m/s vacío; dc=dint+2mm, 2mm = 2× espesor de pared estándar de 1mm):
- Red secundaria O2 8bar (200 l/min, antes de la reducción): Dint=8,14mm+2=10,14mm → **1/2"**
- Ramal O2 4bar (70 l/min, después del reductor de 2ª reducción): Dint=6,81mm+2=8,81mm → **3/8"**
- Aire (200 l/min): Dint=8,14mm+2=10,14mm → **1/2"**
- Vacío (300 l/min): Dint=9,89mm+2=11,89mm → **1/2"**

**Tirada de cañería**: la red secundaria de O2 que ingresa al servicio corre a 8bar (presión primaria) por el total combinado (270 l/min, Ø1/2" antes de dividirse) — no se llevan 2 redes paralelas desde el hospital; recién en el ingreso a la UCO un **reductor de presión (2ª reducción, 8→4bar)** deriva la porción que necesita 4bar (70 l/min, Ø3/8"), mientras el resto sigue a 8bar (200 l/min, Ø1/2"). Junto con las redes de aire y vacío, todas llegan a una **válvula de seccionamiento general de la UCO**, de la que salen **3 ramales** (uno por tramo físico de la disposición en U: ala 1 de 4 camas, centro de 2, ala 2 de 4), cada uno con su propia válvula de sectorización, llevando las 4 líneas juntas (O2 8bar, O2 4bar, aire, vacío) hasta el poliducto de cada cabecera (bajadas O2 8bar ½", O2 4bar 3/8", aire ½", vacío ½", con reducción final a 3/8"-5/16" en el poliducto).

**b) Fuente de aire medicinal — respuesta: NO se puede dimensionar con los datos dados.** El enunciado da que UCO=25% y UTI=40% del **consumo** total de la institución. Pero `gases-medicinales.md` distingue explícitamente dos magnitudes distintas: el "consumo estimado real" (m³/mes, el que se usa para elegir la fuente de **O2**) y el "caudal de diseño de la cañería troncal" a CU=1 (el que exige la norma para dimensionar la fuente de **aire y vacío** — "no el consumo estimado real como en O2", pág 73). El dato que da el enunciado es de consumo, no de caudal de diseño CU=1 — y no hay motivo para asumir que esas proporciones coinciden, porque cada servicio tiene un patrón de uso/ocupación real distinto de su caudal de diseño a plena simultaneidad. Deducir un "total institucional" a partir de 200/0,25=800l/min da una aproximación al consumo real, no al caudal de diseño que la norma exige para la fuente de aire. Para responder correctamente haría falta el caudal de diseño (CU=1) de cada servicio del hospital, dato que no está en el enunciado — no se inventa, se señala el faltante (regla de precisión del proyecto).

#### 6) Climatización — ✅ revisado por el usuario (2026-07-15)
**a) Condiciones Quirófano (Res.810) y UTI (Res.748)**: Quirófano: flujo unidireccional, 15-20 renov/h, presión positiva (≥2,5 Pa), T 20-24°C, HR 30-60% (óptimo 50-55%), v aire 0,20-0,30 m/s, toma de aire 100% exterior, filtrado 3 etapas (25%/90%/HEPA 99,97-99,99%), funcionamiento 24h. UTI: T 24-26°C, HR 30-60%, recambio **4/h habitación, 2/h resto de unidad**, presión +/- según necesidad de aislamiento del paciente (no es fija como en quirófano, se define según necesidad de aislamiento de cada paciente — inmunodeprimido: positiva; infeccioso: negativa). *(El resumen no detalla explícitamente 3 etapas de filtrado para UTI como sí lo hace para cirugía — se asume esquema de filtrado equivalente por principio general, aclarando que la cita puntual de 3 etapas es específica de cirugía.)*

**b) Cómo se logra**: Quirófano → UTA exclusiva por quirófano con filtración escalonada, caudal de impulsión ~15% mayor que el de extracción (genera la sobrepresión), difusores de techo + extracción a piso (patrón unidireccional), sin split. UTI → UTA/central de zona con HEPA, caudalímetro para verificar renovaciones, extractor dedicado en las habitaciones de aislamiento para poder pasar a presión negativa cuando el paciente lo requiera.

---

## Final 19/12/2024 — reconversión de "Aislamiento" a UTI, contigua a Shockroom
**⚠️ Pendiente de revisión por el usuario — resolución generada automáticamente, no chequeada punto por punto todavía.**

Final de 10 preguntas (5+5+5+5+20+20+10+10+10+10 = 105P). Fuente: `Finales/2024-12-19/` (3 fotos, incluye plano). Caso: institución Nivel III de riesgo.

### Enunciado completo

*"En el servicio de Ingeniería de una institución Nivel III de riesgo, se está trabajando en la reestructuración del área del plano adjunto. En el espacio que durante la pandemia se había destinado a 'Aislamiento', se pretende instalar una UTI. Como se puede apreciar el local 'shockroom' se encuentra cercano."*

(Plano: local "Aislamiento" de 86,00 m², contiguo a "Shockroom"; ver `Finales/2024-12-19/` 3ª foto para el plano completo — no reproducible en texto).

1. Definir UTI, clasificar el local según AEA. *(5P)*
2. Definir shockroom, clasificar el local según AEA. *(5P)*
3. Indicar por lo menos 3 características relevantes que ayuden a tomar la decisión de la pertinencia del proyecto. *(5P)*
4. Ubicar los poliductos de cabecera, en ambos locales y describirlos completamente. *(5P)*
5. Diseñar la instalación eléctrica de UTI y del local shockroom. Considerar que la resistividad del terreno es de 6,8 [Ωm]. *(20P)*
6. Diseñar la instalación de gases medicinales. Indicar recorrido y características de las cañerías. Válvulas de sectorización. *(20P)*
7. Describir los equipos de utilización que colocará en cada boca y definir su función. *(10P)*
8. La sala de máquinas se encuentra ubicada a unos 30 mts de este sector, la fuente de aire medicinal ha sido recientemente actualizada bajo norma, pero resta actualizar la fuente de vacío que hasta ahora ha funcionado con 2 bombas de anillo de agua de 5,5 HP.

   Tabla de bombas AR (modelos y especificaciones):
   | | 870C | 1170C | 1870C | 2670C | 3820C |
   |---|---|---|---|---|---|
   | Caudal [l/min] | 850 | 1100 | 1850 | 2600 | 3800 |
   | Caudal [m³/h] | 51 | 66 | 111 | 156 | 228 |
   | Vacío máx. a 20°C (presión residual mmHg) | 30 | 30 | 30 | 30 | 30 |
   | Ø Aspiración bridada | (R)1"BSP | (R)1"BSP | 1½" | 1½" | 2½" |
   | Ø Expulsión bridada | (R)1"BSP | (R)1"BSP | 1½" | 1½" | 2½" |
   | Sello de cierre mecánico | Cerámica, carbón y NBR (todos los modelos) | | | | |
   | Consumo máx. (ref. H2O) [l/m] | 5 | 6 | 9 | 11 | 15 |
   | HP | 2 | 3 | 4 | 5,5 | 10 |
   | RPM | 2800 | 2800 | 1400 | 1400 | 1400 |
   | Alto [mm] | 207 | 207 | 320 | 320 | 420 |
   | Largo X [mm] | 380 | 410 | 520 | 557 | 650 |
   | Ancho [mm] | 270 | 270 | 350 | 376 | 400 |
   | Distancia entre bocas Asp-Exp | 110 | 110 | 182 | 182 | 205 |
   | Entrada de agua (BSP hembra) | 1/4" | 1/4" | 1/2" | 1/2" | 3/4" |
   | Peso bomba monoblock [Kg] | 33 | 40 | 65 | 75 | 148 |

   *Nota del enunciado: el caudal de la instalación existente es inferior a 1900 l/min.*

   Diseñar y graficar la fuente de vacío medicinal, según la normativa vigente. *(10P)*

9. De acuerdo a las directrices de organización y funcionamiento del servicio de UTI del PNGCAM, se puede plantear el diseño del sistema de iluminación general. ¿Cómo procede para verificarlo según el cálculo de luminarias basado en el método de los lúmenes? *(10P)*
10. ¿Cómo realizará la alimentación de emergencia de este sector, sabiendo que el grupo electrógeno existente (trifásico) tiene una potencia remanente de 40 KVA? Justifique la decisión adoptada. *(10P)*

*(La tabla de bombas fue transcripta por OCR de la foto — el enunciado no da el n° de camas de esta UTI en ningún punto; para las preguntas 3, 9 y 10 se estima a partir de los 86 m² del plano vía Res.748/2014, como se hace en la pregunta 3 abajo. Si en la sesión de revisión se ve la foto y hay más precisión, ajustar.)*

### Resolución (borrador sin revisar)

#### 1) Definir UTI, clasificar el local según AEA
UTI: servicio de internación para pacientes en estado crítico que requieren monitoreo continuo y soporte vital (Res.748/2014, `servicios-hospitalarios-resoluciones.md`). AEA 710: **Grupo 2** — no admite discontinuidad ante 1ª falla. Subtipo: **2B** si hay pacientes con vías centrales/catéteres intracardíacos (riesgo de microchoque) — criterio conservador recomendado para UTI en general (`instalaciones-electricas.md`).

#### 2) Definir shockroom, clasificar según AEA
Shockroom: sala de reanimación/estabilización inmediata de pacientes críticos ingresados por guardia (Res.428/2001, mín 12 m²/cama, `servicios-hospitalarios-resoluciones.md`). AEA: también **Grupo 2** (maniobras de reanimación ininterrumpibles), subtipo 2B por el mismo criterio (uso de desfibrilador/vías centrales).

#### 3) 3 características para decidir la pertinencia del proyecto
- **Superficie**: 86 m² vs. exigencia Res.748/2014 (≥9m²×2×N°camas, 50% apoyo) → alcanza para ≈4-5 camas: cumple el mínimo de **UCI Nivel 2** (≥4 camas) pero no Nivel 1 (≥8 camas). Condiciona qué nivel de UTI se puede habilitar ahí.
- **Adyacencia con shockroom**: favorable — permite traslado rápido de pacientes críticos desde reanimación a internación crítica (mismo criterio de proximidad que UTI-quirófano-UCO).
- **Preexistencia como sala de aislamiento**: probablemente ya tiene presión negativa/extracción independiente (útil para aislar pacientes infecciosos dentro de la UTI) pero hay que auditar si tiene gases medicinales e instalación eléctrica grupo 2 ya hechas, o si implica obra completa (impacta costo/plazo del proyecto).

#### 4) Poliductos de cabecera en ambos locales
Poliducto = columna mural de cabecera con bocas de gases + tomas eléctricas integradas (a diferencia del miniducto, que las separa). UTI (por cama, tabla `gases-medicinales.md`/`servicios-...md`): 2 O2, 1-2 aire, 2 vacío, + TUM (mín 12/puesto en ≥2 circuitos de ≤6, identificando toma normal/emergencia en rojo) + IUG. Shockroom (asimilable a fila "UTI/Shock room" de la tabla de caudales): 1-2 O2, 1 aire, vacío doble (2 tomas, redundancia para reanimación simultánea de vía aérea + gástrica) + TUM suficientes para desfibrilador/monitor/bomba de infusión simultáneos.

#### 5) Instalación eléctrica de UTI y shockroom, ρ=6,8 Ω·m
Grupo 2 → **Red IT** obligatoria: transformador de aislación monofásico 3-8kVA (5kVA recomendado), monitor de aislación (IMD), tablero de aislación propio y no compartido por sala. **Si la UTI tiene >4 puestos, no puede resolverse con un único sistema IT** — hay que subdividirla en módulos de ≤4 puestos, cada uno con su propio tablero de aislación (`instalaciones-electricas.md`).

Circuitos: TUM (≥12/puesto), IUG (mitad de bocas desde UPS), TUG (1 cada 12 m², mín 2/puesto, fuera de la zona del paciente).

**PAT** (suelo homogéneo, más favorable que el otro final): con la fórmula convencional Rt=ρ/L (`instalaciones-electricas.md`) y jabalina L=3m: R=6,8/3≈2,27Ω. Con 2 jabalinas en paralelo (K=0,57): R≈1,3Ω, cumple el ≤2Ω general. Además del RPAT, montar la equipotencialización de zona de paciente (BEP único del edificio → BPATH → PEH radiales a cada masa: camas, mesas, poliducto metálico, cañería de gases, marcos de puertas), exigencia aparte del valor de R (máx 20 mV entre masas, no depende de la resistividad del suelo).

#### 6) Instalación de gases medicinales: recorrido, cañerías, válvulas de sectorización
Recorrido: sala de máquinas (a 30m) → regulación primaria 8bar en cañería troncal → regulación secundaria a 4bar cerca del sector → cañería secundaria hasta poliductos de UTI y shockroom → bajadas de cabecera. Cañerías: cobre electrolítico (válido para todos los gases), uniones por soldadura, pendiente hacia la fuente en el tramo de vacío (evacuar condensado), velocidades de diseño 8 m/s (O2/aire) y 100 m/s (vacío). Válvulas de sectorización: una general del sector (permite cortar UTI+shockroom sin afectar el resto del hospital) + una por local (UTI, shockroom) + una por módulo si la UTI se subdivide en >1 sistema IT/gases — todas accesibles, señalizadas, con indicador de posición.

#### 7) Equipos de utilización por boca
O2: caudalímetro + humidificador (mide/regula caudal, humidifica) o reductor de presión (si alimenta un equipo, p.ej. ventilador). Aire: caudalímetro/reductor. Vacío: regulador de vacío con vaso/trampa (limita la depresión y colecta el líquido aspirado). Fuente: `gases-medicinales.md`.

#### 8) Fuente de vacío — actualizar desde 2 bombas de anillo de agua de 5,5HP; caudal existente <1900 l/min
**El dato clave no es la tabla, es la norma**: IRAM-ISO 7396-1 exige **mínimo 3 bombas** para el sistema de vacío (`gases-medicinales.md`), y la instalación actual tiene solo **2** — no cumple, más allá de si el caudal alcanza. Esa es la primera corrección, antes de elegir modelo.

Con la tabla transcripta arriba, 5,5HP corresponde al modelo **2670C** (2600 l/min c/u). Se rediseña con **3 bombas** en config. duty/standby (norma: ante la falla de 1, las restantes cubren el 100%). Con demanda <1900 l/min, evaluar el modelo más chico que en configuración 2-de-3 (con 1 fuera de servicio) siga superando 1900 l/min:
- **1870C** (1850 l/min c/u, **4 HP** — corregido; una versión anterior de esta resolución decía "9HP", pero la tabla no tiene ese valor): con 2 de 3 en servicio → 3700 l/min, cubre holgadamente los 1900 exigidos, con mucho menor consumo/potencia que sobredimensionar a 2670C.
- Se descartan 870C/1170C (con 2 en servicio dan 1700-2200 l/min, insuficiente margen o directamente por debajo del mínimo en el peor caso).

**Este ítem quedó marcado para reconfirmar en la sesión de revisión** — recalcular con la tabla ya transcripta arriba (antes se leía la foto cada vez, con riesgo de error de OCR como el del HP).

Esquema (para dibujar): 3 bombas de anillo de agua 1870C en paralelo → colector de succión con válvulas de aislación individuales por bomba → trampa de líquido + filtro bacteriológico → tanque/depósito de vacío → línea troncal a 100 m/s hacia el sector, con manómetro/vacuómetro y alarma de baja presión en el tablero de control.

#### 9) UTI — verificación de iluminación general por método de lúmenes
Con los niveles de `luminotecnia.md` (cuidados intensivos: hasta 300 lux general, ≥1000 lux al examinar) se aplica el método de los lúmenes completo (8 pasos, ya en `luminotecnia.md`): definir E exigido → k índice de local → η coef. utilización → fm (limpio 0,8) → Φtotal=(E·S)/(η·fm) → N° luminarias → verificar Ereal≥Eexigido. Superficie a usar: los 86 m² del local (o la superficie que resulte de la subdivisión en módulos de la pregunta 5, si aplica) — **definir con el usuario en la sesión de revisión qué S tomar exactamente.**

#### 10) Alimentación de emergencia de la UTI, GE remanente 40kVA
Criterio (`alimentacion-de-emergencia.md`): 1) listar cargas esenciales de continuidad vital (servicio UTI = **crítico**, según la clasificación de servicios de la guía de práctica) — TUM de cabecera a 600W/cama, IUG parcial (mitad de bocas por UPS), equipos electromédicos críticos; 2) sumar consumo con N° de camas estimado (≈4-5, de la pregunta 3); 3) comparar contra la potencia disponible del GE (40kVA remanente ≈32kW útiles a fp 0,8); 4) **decisión**: no volcar climatización ni TUG de uso general al remanente del GE salvo que sobre capacidad — priorizar exclusivamente lo que es riesgo de vida si se corta. Con 4-5 camas × 600W ≈2,4-3kW + equipos críticos, el remanente de 40kVA alcanza con margen amplio — a diferencia de una UTI grande, acá no debería hacer falta excluir cargas.

---

## Nota sobre las fuentes originales
Las fotos de ambos finales están guardadas como archivo en la carpeta:
- `Finales/2025-02-20/` (2 fotos, preguntas 1-6 completas — el final termina ahí, 100 puntos, sin plano).
- `Finales/2024-12-19/` (3 fotos: enunciado 1-8 + tabla de bombas, enunciado 9-10, y el plano del sector Aislamiento/Shockroom/UTI de 86 m²).

Con el enunciado ya transcripto arriba en texto, solo hace falta abrir las fotos para: el plano del 19/12/2024 (pregunta 3-6, no reproducible en texto) o para verificar algún dato puntual ante duda de OCR.
