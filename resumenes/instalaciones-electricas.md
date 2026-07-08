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
- Jabalinas en paralelo: RPAT = K·Rindiv; K: 2→0,57; 3→0,42; 4→0,33; 5→0,27; ... 10→0,15.
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

## Servicio de Radiología (archivo 05, imágenes)
Normativa: PNGCAM Res. 610/2004 y Res. 3590/2021. Contenido gráfico: transformador, pilar de acometida, acometida al servicio, sala de examen y comando, tablero seccional, revelado manual/automático, digitalizador CR e impresora. (Ver detalles de requisitos por modalidad en `servicios-hospitalarios-resoluciones.md`.)

## Miniductos, poliductos y torretas (archivo 10, imágenes)
Paneles de cabecera: **miniducto** (gases y eléctrico separados), **poliducto** (columna mural con bocas de gases + tomas), **torreta** (de techo). Contenido principalmente fotográfico (mismo material que `10_Redes Gases Medicinales`).
