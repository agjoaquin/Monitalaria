# ÍNDICE — Ingeniería Hospitalaria (base de conocimiento)

Router para consulta eficiente. **Para responder una pregunta: (1) identificá el/los tema(s) en esta tabla por sus keywords, (2) leé SOLO el/los `.md` de `resumenes/` correspondiente(s), (3) si necesitás una figura/detalle no textual, abrí el PDF fuente indicado en la ruta y página.** Los resúmenes ya contienen las cifras, fórmulas y normas; el PDF solo se abre para imágenes/planos.

## Cómo está organizado
- `resumenes/` — un `.md` denso por tema, con referencias de página al PDF fuente.
- `Clases actualizadas/` — PDFs originales (fuentes), en subcarpetas por tema.
- `Resumen Hospitalaria.docx` — resumido en `resumenes/servicios-hospitalarios-resoluciones.md`.

## Mapa temático (tema → resumen → keywords)

| Tema | Resumen | Keywords para ruteo | PDFs fuente |
|---|---|---|---|
| Alimentación de emergencia | `resumenes/alimentacion-de-emergencia.md` | UPS on-line/off-line, grupo electrógeno GE, COP/PRP/FTP, kVA, tiempo de interrupción <15s, transferencia, ciclo Otto/Diesel, volante de inercia | `Clases actualizadas/Alimentación de emergencia/` (1 PDF, 15 pág) |
| Automatismo | `resumenes/automatismo.md` | pulsador NA/NC, relé, contactor, temporizador, código de colores, circuito de potencia/comando, inversión de giro, sensores | `Clases actualizadas/Automatismo/` (1 PDF, 16 pág) |
| Climatización (HVAC) | `resumenes/climatizacion.md` | HVAC, rooftop, UTA, split, fan coil 2/4 tubos, VRV, filtros HEPA/EPA/ULPA, EN 779/1822, ISO 16890/29463/14644, MERV, renovaciones/hora, presión positiva/negativa, T/HR quirófano, MPPS, sala limpia | `Clases actualizadas/Climatización/` (2 PDF, 67 pág) |
| Estructura hospitalaria | `resumenes/estructura-hospitalaria.md` | definición hospital OMS, REFES, tipología/categoría, ESCIG/ESSID, complejidad, PNGCAM, niveles de atención I/II/III, riesgo Nivel I/II/IIIA/IIIB, Res. 900-E/2017 | `Clases actualizadas/Estructura hospitalaria/` (1 PDF, 21 pág) |
| Gases medicinales | `resumenes/gases-medicinales.md` | O2/aire/vacío/N2O/CO2, IRAM-ISO 7396-1, colores tubería FAAAR 37218, regulación 8/4 bar, caudales l/min, dimensionamiento diámetro cañería, CU=1, velocidades 8/100 m/s, fuentes (tubos/termos/tanque criogénico), cilindros, reductor, caudalímetro, humidificador, diseño UCO, tablas caudal/diámetro | `Clases actualizadas/Gases medicinales/` (5 PDF, 169 pág) |
| Instalaciones eléctricas BT | `resumenes/instalaciones-electricas.md` | AEA 710 / 90364-7-710, salas grupo 0/1/2/2A/2B, macro/microchoque, fibrilación µA, Red TT/TN/IT, TUG/IUG/TUE/TUM/TC, secciones mm², termomagnética curva B/C/D, disyuntor diferencial 30mA, puesta a tierra jabalina RPAT ≤2Ω, PEH/BEP/BPATH 20mV, transformador de aislación 5kVA, monitor de aislación, radiología | `Clases actualizadas/Instalaciones electricas a baja tensión/` (7 PDF, 154 pág) |
| Luminotecnia | `resumenes/luminotecnia.md` | flujo luminoso lumen, iluminancia lux, intensidad candela, luminancia, eficiencia lm/W, deslumbramiento, sistemas directa/indirecta/difusa, niveles lux por local, lámpara scialítica 4500K 10000-120000lux CRI>90, quirófano 100000 lux | `Clases actualizadas/Luminotecnia/` (2 PDF, 52 pág) |
| Transporte de pacientes | `resumenes/transporte-de-pacientes.md` | ambulancia, Res. 906-E/2017, móvil alta/mediana/baja complejidad, neonatal-pediátrica, habitáculo 2,35×1,50×1,60, camilla 190×55, tomas 12V/220V, equipamiento médico, estrella de la vida | `Clases actualizadas/Transporte de pacientes/` (1 PDF, 60 pág) |
| Servicios y resoluciones (requisitos) | `resumenes/servicios-hospitalarios-resoluciones.md` | Res. 748/747/609/306/810/1866/2547/375/1184/428/348/610/3590, m² por cama, bocas de gases por servicio, T/HR/renovaciones por servicio, dimensiones quirófano, UCI/UCIP/neonato/hemodinamia/guardia/maternidad/imágenes RX-TC-RM-ecografía | `Resumen Hospitalaria.docx` |

## Índice cruzado (tópicos que aparecen en varios temas)
- **Filtros HEPA / calidad de aire**: `climatizacion.md` (clasificación y normas) + `servicios-hospitalarios-resoluciones.md` (exigencia por servicio: cirugía, hemodinamia).
- **Bocas/caudales de gases por servicio**: `gases-medicinales.md` (cálculo y tabla teórica) + `servicios-hospitalarios-resoluciones.md` (nº de bocas exigido por norma).
- **Salas grupo 2 / red IT / equipotencialización**: `instalaciones-electricas.md`.
- **Lámpara scialítica**: `luminotecnia.md` (características) + `instalaciones-electricas.md` (alimentación red IT/UPS/equipotencial) + `servicios-hospitalarios-resoluciones.md` (nº de brazos por riesgo de cirugía).
- **Climatización de quirófano/UTI**: `climatizacion.md` (parámetros técnicos) + `servicios-hospitalarios-resoluciones.md` (valores exigidos por resolución).

_Total fuentes: 20 PDF (557 pág) + 1 DOCX. Última generación: 2026-07-08._
