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
- Velocidades: **O2 y aire 6–15 m/s** (se adopta 8 m/s); **vacío 30–100 m/s** (se adopta 100 m/s).
- Presiones: O2/aire **P = 4–8 bar**; aspiración/vacío **0,6 bar (≤60 kPa)**.
- **Fórmula diámetro interno**: `Dint = 18,8 · √(Q/(v·P))` aprox. (Q caudal m³/h, v m/s, P bar). Diámetro comercial/exterior: **dc = dint + 2 mm**.
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

## Diseño de instalación de una UCO (archivo "IH Diseño…", pág 2-35)
- Normativa: **Res. 375/2002 PNGCAM** (unidades coronarias) + IRAM-ISO 7396-1:2014.
- Superficie **9 m² por cama**; 50% internación / 50% apoyo.
- Por cabecera de cama: **2 tomas O2, 1 aire comprimido, 1 vacío** (acoples distintos por gas, tipo Diss). Office sucio: salida de aire para secado. Office limpio: alarma de los 3 gases. Toma = boca = unidad terminal.
- Diámetros de bajadas: O2 ½", Vacío ½", Aire 3/8" (troncales); poliductos por cama con reducciones a 3/8"–5/16".
- Ejemplo cálculo red secundaria O2 (pág 21): tramo UCO 4 bocas×7 = 28 l/min; + internación 5 bocas×7 = 35; total 63 l/min → 3/8".
- Aire (pág 23): 4 bocas UCO ×20 + secado 50 = 130 l/min → 3/8". Vacío (pág 25): 4×30 + 5×10 = 170 l/min → ½".
- **Tablas de caudal máximo por diámetro** (pág 31-33): para O2/aire a 4 y 8 bar (v=8 m/s) y vacío a 0,6 bar (v=100 m/s), en pulgadas 1/4"–2", dando caudal m³/h, m³/día y l/min. Ej. O2/aire 8 bar: 3/8"→10 m³/h; ½"→21; 1"→99; 2"→431. Vacío: 3/8"→15 m³/h; ½"→27; 1"→110; 2"→438.
