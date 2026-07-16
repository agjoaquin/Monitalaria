# Gases medicinales
Fuentes (5 archivos en `Clases actualizadas/Gases medicinales/`):
- `Gases medicinales.pptx.pdf` (24 pág) — teoría general, dimensionamiento, equipos de utilización
- `Gases medicinales _fuentes.pdf` (33 pág) — fuentes O2/aire/vacío bajo IRAM-ISO 7396-1
- `IH Diseño de instalaciones de gases medicinales 2025.pdf` (35 pág) — diseño paso a paso de una UCO + tablas de caudal/diámetro
- `10_Redes Gases Medicinales_Campus.pdf` (43 pág) — imágenes: paneles de cabecera, miniductos, poliductos, torretas, cañerías, alarmas
- `11_Fuentes de Gases Medicinales_Campus.pdf` (34 pág) — imágenes: baterías de tubos, tanque criogénico, termos, aire comprimido, vacío

## Definición y normas (teoría pág 2-3)
Gas medicinal (Res. 1130-2000 MSN): producto gaseoso en contacto directo con el organismo, con propiedades farmacológicas/inmunológicas/metabólicas. Normas: **IRAM-ISO 7396-1** (redes gases comprimidos y vacío), ISO 7396-2 (evacuación gases anestésicos), ISO 10083 (aire por concentradores), Farmacopea Argentina T.I, NFPA 99, **IRAM 2588** (colores de cilindros), ISO 10524 (reguladores), **IRAM-FAAAR 37218** (colores de tuberías).

## Gases de uso hospitalario (pág 4)
O2, aire comprimido, óxido nitroso N2O, vacío/succión, CO2, óxido nítrico, carbógeno (O2 95% + CO2 5%), helio.

## Código de colores para tuberías (IRAM-FAAAR 37218, pág 7)
- BLANCO: oxígeno
- AMARILLO: aire comprimido
- ROJO: vacío
- AZUL CLARO: óxido nitroso
- VIOLETA: dióxido de carbono
- NEGRO: nitrógeno
- CASTAÑO: helio

## Materiales permitidos (pág 8)
Cobre electrolítico, acero inox, poliamidas: todos los gases. Hierro galvanizado, polipropileno, PVC: solo vacío.

## Regulación de presiones (2 etapas, teoría pág 11)
- Regulación **primaria**: reduce P de la fuente a **8 bar**, en cañería troncal.
- Regulación **secundaria**: reduce a **4 bar**, en cañerías secundarias.
- (Vacío no se regula por etapas.)

## Dimensionamiento fluidodinámico (teoría pág 9-14; diseño pág 17-18)
Parámetros: caudal, presión de servicio, longitud de cañerías, pérdida admisible, estrangulamientos (long. equivalente), diámetro.
- Hipótesis: coeficiente de uso simultáneo **CU = 1** (todos los consumos simultáneos).
- Velocidades: **O2 y aire 6–15 m/s** (se adopta 8 m/s); **vacío 30–100 m/s** (se adopta 100 m/s). Aclaración textual de la Guía de práctica (pág 63-64, justo antes de la fórmula de Dint): "Se recomienda que la velocidad del fluido no exceda los 15 m/seg, **trabajando normalmente con 8 m/seg, de esta manera el coeficiente de seguridad es mayor**." Es decir: **15 m/s es el límite máximo a no superar, no el valor de diseño** — trabajar a 8 m/s da MÁS margen de seguridad (mayor diámetro), no menos. No usar 15 m/s como "peor caso" para dimensionar; el valor de cálculo normal es 8 m/s salvo que el enunciado pida explícitamente verificar el límite superior.
- Presiones: O2/aire **P = 4–8 bar**; aspiración/vacío **0,6 bar (≤60 kPa)** (teoría) / **0,65 bar** (Guía de práctica pág 64, "depresión media de 0,65 bar" con v=100m/s — cifra algo distinta según la fuente, usar 0,65 si el enunciado remite a la guía práctica).
- **Fórmula diámetro interno**: `Dint = 18,8 · √(Q/(v·P))` aprox. (Q caudal m³/h, v m/s, P bar). Diámetro comercial/exterior: **dc = dint + 2 mm** (2mm = 2× el espesor de pared estándar de 1mm, uno a cada lado del diámetro — no sumar solo 1mm).
- Diámetro mínimo: 3/8" fuera de paneles/poliductos/torretas; dentro ≥1/4" (preferente 5/16").
- Reducir al mínimo los cambios de diámetro; cañería calculada a plena carga.

## Tabla de caudales teóricos por boca [l/min] (teoría pág 13; diseño pág 16)
| Servicio | O2 (4 bar) | O2 (8 bar) | Vacío | Aire (4) | Aire (8) |
|---|---|---|---|---|---|
| Internación/Guardia | 7 | | 10 | | 7 |
| UTI / Shock room | 7 | 20 | 2×30 | | 20 |
| UCO | 7 | 20 | 30 | | 20 |
| Quirófano | 7 | 20 | 2×60 | | 20 |
| Partos | 7 | | 25 | | |
| RRN | 2×3 | | 2×10 | | |
| Neonatología | 3 | | 15 | | 2×10→15 |
| Imágenes/Resonancia | 7 | 20 | 25 | | 20 |
| Laboratorio / office sucio | | | | | 50 |

## Sistemas de suministro (IRAM-ISO 7396-1, fuentes pág 2-3)
- Cada sistema: **mínimo 3 fuentes independientes** (5.1.1). Sistema de vacío: **mínimo 3 bombas** (5.1.2).
- Tipos de fuente: gas en cilindro/batería, líquidos criogénicos/no criogénicos (móviles o estacionarios), compresor de aire, mezclador, concentrador de O2.
- Clasificación: **primaria** (conexión permanente, principal), **secundaria** (automática si falla la principal), **de reserva** (manual/automática si fallan ambas o hay mantenimiento).

## Oxígeno medicinal (teoría pág 15; fuentes pág 4)
Incoloro, inodoro, insípido; comburente; más denso que el aire; pureza 98% (libre de CO/CO2); T ebullición **-182,97 °C**; **1 L O2 líquido = 840 L gaseoso**; peso específico 1,35 kg/m³ (15 °C, 1,013 bar). Reacciona con grasas/aceites.
### Fuentes de O2 y capacidad (fuentes pág 5-12)
- Tubos (gaseoso): 10 m³ (rampa, 200 bar) / 5-7 m³ (150 bar). Presión constante; baja capacidad; alta tasa de recambio.
- Termos/tanque criogénico móvil (líquido): 130-180 m³; P trabajo 10/12 bar; peso vacío 95-130 kg. Presión variable, venteo.
- Tanque criogénico fijo (líquido): 800 – 10.000 m³. Mayor capacidad, menor costo, requiere espacio/accesibilidad.
### Rotulado O2 (fuentes pág 9)
Cruz griega verde; leyenda de generación por adsorción; composición; datos del centro y director técnico (matrícula); lote; fechas llenado/vencimiento; leyenda de prescripción médica obligatoria.

## Aire de grado médico (teoría pág 17; fuentes pág 17,21-28)
20,4% ≤ O2 ≤ 21,4%; aceite ≤0,1 mg/m³; CO ≤5 ml/m³; CO2 ≤500 ml/m³; vapor de agua ≤67 ml/m³; SO2 ≤1 ml/m³; NO+NO2 ≤2 ml/m³. Calidad fina PR = -40 °C.
- Configuraciones IRAM-ISO 7396-1: (1) 1 compresora + colector + acondicionadora + 2 baterías; (2) 2 compresoras + 2 colectores + 2 acondicionadoras + 1 batería; (3) 3 compresoras + 2 colectores + 2 acondicionadoras.
- Unidad compresora: filtro, compresores, postenfriador, separador de aceite. Unidad acondicionadora: secador, filtros, sensor de punto de rocío con alarma.
- **Importante (5.5.1.5)**: compresores y mezcladores deben conectarse al suministro eléctrico de emergencia.

## Vacío (teoría pág 23; fuentes pág 29-31)
- Regulador de vacío: rango 0 a -0,2 bar (pediatría), 0 a -0,6 bar (adultos). Vaso de vacío con trampa y flotador (250 ml – 5 L).
- Fuentes: bomba seca (vacíos bajos, eficiente, cara) vs. bomba de anillo líquido (agua/aceite; robusta, aspira húmedo, requiere agua). Sistema de vacío con trampa de líquido + filtro bacteriano + depósito.

## Equipos de utilización (teoría pág 18-22)
| Gas | Equipo | Parámetro |
|---|---|---|
| O2 | Caudalímetro + humidificador / reductor de presión | Caudal / Presión |
| Aire | Caudalímetro / reductor | Caudal / Presión |
| Vacío | Regulador de vacío | Depresión |
| N2O | Reductor de presión (mesa de anestesia/mezclador) | Presión |
- Caudalímetro: mide y regula caudal, uso vertical, con humidificador.
- Humidificador: 3 ml agua/h a 4 l/min; 9 ml/h a 12 l/min. Pérdida de carga <0,1 bar a 15 l/min.
- Reductor de presión: cámara alta P → válvula/diafragma → cámara baja P.

---
## Complemento — Guía de práctica, Guía Nº 7: Redes medicinales (pág 63-68)
Fuente: `Clases actualizadas/Guía de práctica/Guía de práctica 2026.pdf`

### Regulación de presiones — definiciones de la guía (rangos, complementa "Regulación de presiones" arriba)
- **Presión primaria**: la que entrega la central de almacenamiento, **7-10 bar**; es la existente en la red troncal; se fija en la prueba de funcionamiento.
- **Presión secundaria**: obtenida al regular la primaria, normalmente **3,5 ± 0,7 bar**; existente en las redes secundarias (requiere válvulas reguladoras — segunda reducción — en cada red secundaria).
- *Nota: la teoría general (`Gases medicinales.pptx.pdf`) redondea estos valores a 8 bar (primaria) y 4 bar (secundaria) para el dimensionamiento fluidodinámico; ambas cifras son válidas — la guía práctica da el rango real de tolerancia, la teoría el valor nominal de cálculo.*
- **Prueba de estanqueidad**: se realiza antes de la prueba de funcionamiento, con toda la cañería montada; verifica que no haya pérdidas; duración **mínima 12 horas continuas**.
- **Red principal/troncal**: desde la central de almacenamiento hasta las centrales de segunda reducción o válvulas de seccionamiento de cada red secundaria.
- **Red secundaria**: desde la válvula de seccionamiento o central de regulación secundaria; en su extensión están los puestos de consumo.

### Componentes de red — datos adicionales
- Cañerías en caño de Cu electrolítico (alto coeficiente de seguridad, resistente al poder oxidante del O2). Caño de 1 mm de espesor de pared (el más usado): presión de utilización máxima **30 bar**, presión de trabajo **15 bar**.
- Válvulas de seccionamiento: tipo esférica, montadas al inicio de cada red secundaria en punto de fácil acceso.

### Tabla de caudales teóricos por boca — variante de la Guía práctica (pág 64)
*Cifras algo distintas a la tabla de "Dimensionamiento fluidodinámico" (proveniente de otro material de cátedra); ambas están citadas por la cátedra — verificar cuál pide el enunciado o usar el PDF fuente pág 64 si hace falta el valor exacto. Corregida (2026-07-15) — la versión anterior tenía una sola columna de Aire y le faltaba la de 4bar; se verificó contra la imagen original de la diapositiva.*
| Servicio | O2 4 kg/cm² | O2 8 kg/cm² | Vacío | Aire 4 kg/cm² | Aire 8 kg/cm² |
|---|---|---|---|---|---|
| Internación | 7 | — | 10 | 7 | — |
| UTI (adulto y pediátrico) | 7 | 20 | 30×2 | — | 20 |
| Quirófano | 7 | 20 | 60×2 | — | 20 |
| Neonatología | 3 | 15 | 10×2 | — | 15 |
Notas de la guía: en quirófano, con 1 boca de O2 regulada por presión (8 kg/cm²) alcanza; la boca regulada por caudal (4 kg/cm²) puede tomarse de la mesa de anestesia. En UTI (y por extensión servicios similares como UCO), el vacío se calcula tomando el caudal de 1 sola boca (no sumando las 2 de la cabecera). No hay fila propia de UCO en esta tabla — si se necesita, se modela por analogía con la fila de UTI (mismo nivel de criticidad/monitoreo).

### Tabla de peso de caños de cobre redondos [g/m] (pág 68, referencia comercial)
| Ø [pulg] | Ø [mm] | e=0,5mm | e=0,75mm | e=0,8mm | e=1mm | e=1,5mm | e=2mm |
|---|---|---|---|---|---|---|---|
| 1/8 | 3,175 | 38 | 51 | 52 | — | — | — |
| ¼ | 6,35 | 82 | 117 | 123 | 150 | 204 | 246 |
| 3/8 | 9,52 | 126 | 184 | 193 | 243 | 337 | 426 |
| ½ | 12,7 | 171 | 251 | 265 | 331 | 470 | 602 |
| ¾ | 19,05 | 261 | 384 | 407 | 512 | 737 | 963 |
| 1 | 25,4 | 349 | 530 | 556 | 690 | 1004 | 1320 |
| 1 ½ | 38,1 | 527 | 784 | 850 | 1047 | 1540 | 2037 |
(tabla completa de 18 diámetros en PDF fuente pág 68; e = espesor de pared)

### Ejercicios de práctica (pág 66-67)
1. Diseñar el recorrido de cañerías de gases medicinales para: 5 camas UTI, 1 quirófano, internación general (6 hab. dobles + 6 hab. individuales). Justificar.
2. Del ejercicio 1: (a) diámetro de cañería troncal; (b) diámetros de cañerías secundarias; (c) ¿importa el orden de cálculo (troncal→secundaria o secundaria→troncal)?
3-5. Cálculo de cañería para sector quirúrgico y UTI de un croquis dado (Croquis A, no incluido en el corpus digital — pedir el plano si se necesita resolver); diagramar la instalación completa señalando presión de trabajo por tramo, reguladores de 2ª reducción y válvulas de corte.
6. Neonatología con 6 puestos completos: (a) gases por puesto; (b) equipos de utilización y su función; (c) esquema de la instalación distinguiendo cada cañería.
7. Hemodiálisis con 4 puestos, cañería de O2 existente de ½" y 1 mm de espesor; se agregan 4 puestos más: (a) parámetros de P y Q de trabajo; (b) ¿hace falta modificar la cañería? Justificar; (c) accesorios de esas bocas.
8. Incubadora de UTI con boca de O2, chapa: "entrada limitada al 40% a 2,5 l/min de O2". Especificar parámetros de presión/caudal, croquis de la instalación (pared→incubadora) y equipos de utilización.

## Diseño de instalación de una UCO (archivo "IH Diseño…", pág 2-35)
- Normativa: **Res. 375/2002 PNGCAM** (unidades coronarias) + IRAM-ISO 7396-1:2014.
- Superficie **9 m² por cama**; 50% internación / 50% apoyo.
- Por cabecera de cama: **2 tomas O2, 1 aire comprimido, 1 vacío** (acoples distintos por gas, tipo Diss). Office sucio: salida de aire para secado. Office limpio: alarma de los 3 gases. Toma = boca = unidad terminal.
- Diámetros de bajadas: O2 ½", Vacío ½", Aire 3/8" (troncales); poliductos por cama con reducciones a 3/8"–5/16".
- Ejemplo cálculo red secundaria O2 (pág 21): tramo UCO 4 bocas×7 = 28 l/min; + internación 5 bocas×7 = 35; total 63 l/min → 3/8".
- Aire (pág 23): 4 bocas UCO ×20 + secado 50 = 130 l/min → 3/8". Vacío (pág 25): 4×30 + 5×10 = 170 l/min → ½".
- **Tablas de caudal máximo por diámetro** (pág 31-33): para O2/aire a 4 y 8 bar (v=8 m/s) y vacío a 0,6 bar (v=100 m/s), en pulgadas 1/4"–2", dando caudal m³/h, m³/día y l/min. Ej. O2/aire 8 bar: 3/8"→10 m³/h; ½"→21; 1"→99; 2"→431. Vacío: 3/8"→15 m³/h; ½"→27; 1"→110; 2"→438.

---
## Complemento — Guía de práctica, Guía Nº 8: Centrales de almacenamiento (pág 69-77)
Fuente: `Clases actualizadas/Guía de práctica/Guía de práctica 2026.pdf`

### Alcance
Se centralizan por canalización 4 servicios de gases: **oxígeno, aire, vacío y óxido nitroso**. El resto (nitrógeno, CO2, mezclas especiales) es de consumo puntual y no requiere sistema centralizado.

### Tipos de centrales por gas
- **Oxígeno**: baterías de tubos de gas comprimido; tanques de O2 líquido móvil (termos); tanques de O2 líquido fijo.
- **Aire**: baterías de tubos; centrales compresoras de aire comprimido.
- **Aspiración/vacío**: bombas de vacío; compresores invertidos.

### Centrales manuales vs. automáticas
- **Manuales**: permiten alto consumo pero **no aseguran suministro continuo**.
- **Automáticas**: alto consumo **y** suministro continuo asegurado; la batería automática tiene una **central de inversión automática** en lugar de los dos reductores de presión de la manual.

### Capacidad de las centrales de O2 (orientativo, depende del proveedor)
- Tubos: 10 m³ en rampa fija; 5, 6 o 7 m³ para mover dentro del hospital.
- Termos: 150-180 m³.
- Tanques: desde 800 m³ hasta 10.000 m³.

### Selección de la fuente principal de O2 (criterio, pág 71)
1. Calcular el **consumo estimado real** (m³/mes), a partir del análisis cuantitativo del consumo de cada boca — no es el mismo caudal usado para dimensionar la cañería.
2. Considerar el tiempo de abastecimiento (proveedor-institución).
3. El tendido de cañería sirve para cualquier fuente; se evalúan ventajas/desventajas:
   - **Tubos**: ventaja — si no se consume, no cambian las propiedades del gas (presión constante). Desventaja — fuente menos económica, alto recambio, queda O2 residual en el envase.
   - **Termos**: ventaja — mayor capacidad, más económico que tubos. Desventaja — si no se consume, sube la presión interna y ventea; exige recambio, queda residual.
   - **Tanque**: ventaja — mayor capacidad, más económico, sin volumen residual, no se recambia. Desventaja — si no se consume, sube la presión interna y exige abrir la válvula de venteo.

### Selección de la fuente de reserva de O2 (pág 71)
- Se usa solo si fallan la fuente principal **y** la secundaria.
- Por las ventajas/desventajas anteriores, **la batería de reserva se realiza con tubos**.
- Capacidad: según tiempo de abastecimiento del proveedor y consumo diario; en condiciones normales debe **garantizar 24 horas de abastecimiento**.

### Selección de la fuente de aire y vacío (pág 73)
A diferencia del O2, no es tan simple cambiar de fuente ante un pico de consumo: el equipo debe poder abastecerlo. **El caudal de diseño de la fuente = caudal de la cañería troncal calculado para su dimensionamiento** (no el consumo estimado real como en O2).

### Compresores/bombas de uso medicinal, exentos de aceite — ejemplo de ficha técnica (pág 74, catálogo comercial)
Presión máxima habitual **8,4 kg/cm² (≈120 psi)**. Potencias de ejemplo: 3 CV (desplazamiento 380 Nl/min), 5,5 CV (715 Nl/min), configuraciones dobles 2×3 CV y 2×5,5 CV para redundancia. (Ficha completa —tanque, RPM, dimensiones, peso— en PDF fuente pág 74; son valores de catálogo de un fabricante, no de norma: no usarlos como exigencia normativa en un final.)

### Componentes típicos de un esquema de doble etapa (glosario de planos, pág 72-74)
Fuente primaria/secundaria/reserva con regulador propio → válvulas de corte (de fuente, principal, ascendente, de rama, para mantenimiento) → válvula de alivio → válvula unidireccional → regulador de presión de línea → unidad terminal (boca) → interruptor de alarma. En vacío se agrega: trampa de líquido, filtro bacteriano, depósito.

### Ejercicios de práctica (pág 77)
1. Institución con 10 camas UTI, 2 quirófanos, 1 sala de partos, 2 puestos de neonatología, 1 consultorio de guardia general, 20 habitaciones de 1 cama: (a) caudal total de cada gas; (b) consumo diario y mensual estimado de O2; (c) central de almacenamiento de O2 a usar, justificar; (d) batería de reserva de O2; (e) selección de fuente de aire comprimido con accesorios, justificar; (f) croquis de instalación de aire comprimido con presión de trabajo por tramo; (g) abastecimiento de vacío y valores de P en boca; (h) equipos de utilización por puesto.
2. Batería de reserva para institución en zona aislada por nieve, tanque de 1200 m³ de O2 medicinal, consumo estimado en invierno 1500 m³/mes, proveedor garantiza abastecimiento mensual. Croquis de la alimentación general (tanque, reguladores, válvulas seccionadoras, tubos y/o termos).
3. UTI con sistema central de aire comprimido medicinal exclusivo para fuerza motriz de respiradores de última generación: 10 camas, 4 respiradores, ocupación 95%. (a) diámetro de cañería; (b) dimensionar y caracterizar el sistema de abastecimiento; (c) croquis desde compresores a bocas con reguladores/válvulas/accesorios y presiones a lo largo de la línea.
