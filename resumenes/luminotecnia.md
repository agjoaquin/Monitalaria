# Luminotecnia
Fuentes (2 archivos en `Clases actualizadas/Luminotecnia/`):
- `Luminotecnia.pptx.pdf` (29 pág) — magnitudes, sistemas y niveles de iluminación
- `09_Lámparas scialiticas_2025.pdf` (23 pág) — lámpara scialítica de quirófano

## Magnitudes fotométricas (Luminotecnia pág 4-10)
| Magnitud | Símbolo | Definición | Unidad | Fórmula |
|---|---|---|---|---|
| Flujo luminoso | Φ | potencia luminosa total emitida | lumen (lm) | — |
| Iluminancia | E | densidad de flujo sobre una superficie | lux (lx = lm/m²) | E = Φ/S |
| Intensidad luminosa | I | flujo por unidad de ángulo sólido | candela (cd = lm/sr) | I = Φ/ω |
| Luminancia | L | luz que emite/ve una superficie | cd/m² | L = I/S |
| Eficiencia/rendimiento | H | rendimiento energético de la lámpara | lm/W | H = Φ/W |
- Relación: flujo (lm) = iluminancia (lx) × superficie (m²).

## Aspectos de iluminación de interiores (pág 11-16)
- **Deslumbramiento**: luminancia del objeto >> entorno. Perturbador (velo luminoso, visión borrosa) y molesto (fatiga visual, principal en interiores). Por observación directa o reflejada.
- Color: temperatura de color correlacionada → luz fría (blanco azulado), neutra (blanca), cálida (blanco rojizo). El aspecto final depende de iluminancia + apariencia de color.

## Sistemas de alumbrado (según distribución del flujo, pág 17-23)
- **Directa**: todo el flujo al suelo; más económico y de mayor rendimiento; alto deslumbramiento y sombras duras.
- **Semidirecta**: mayoría al suelo, resto reflejado; sombras suaves; techos no muy altos.
- **Difusa**: 50% suelo / 50% arriba; bajo deslumbramiento, sin sombras; aspecto monótono; pintar claro.
- **Semiindirecta**: 60–90% hacia arriba; pérdidas y consumo altos; buena calidad de luz.
- **Indirecta**: casi toda al techo; similar a luz natural; muy cara; requiere pinturas blancas de alta reflectancia.

## Métodos de alumbrado (pág 24-26)
- General: iluminación uniforme, luminarias regulares en techo.
- General localizado: no uniforme, concentrado en áreas de trabajo; ahorro energético.
- Localizado: suplementario cerca de la tarea (>1000 lux); cuidar relación de luminancias.

## Niveles de iluminación recomendados por local (pág 27)
| Local | Nivel (lux) | Nota |
|---|---|---|
| Consultas médicas | 500–1000 | LED, IRC >90, uniforme |
| Pasillos/áreas comunes | ≥100 | semidirecta |
| Habitaciones de pacientes | 300 (día), baja de noche | LED regulable + natural |
| Emergencia y cirugía | 10.000–20.000; hasta **100.000** sobre área quirúrgica | luz directa sin sombras; salas anexas ≥500 |
| Cuidados intensivos | hasta 300; **≥1000** al examinar | LED ajustable, sin parpadeo |
| Lavandería | 200 | |
| Laboratorios | 500 | |
| Oficinas | 500 | tonos neutros, evitar reflejos en pantallas |

## Depreciación de la eficiencia luminosa (pág 28)
Disminución progresiva de iluminancia por ensuciamiento de lámparas/superficies y depreciación del flujo → programa de mantenimiento y sustitución.

---
## Complemento — Guía de práctica, Guía Nº 5: Diseño de alumbrado de interiores (pág 44-49)
Fuente: `Clases actualizadas/Guía de práctica/Guía de práctica 2026.pdf`

### Método de los lúmenes — procedimiento de cálculo completo
Para dimensionar el alumbrado general de un local (nº de luminarias), 8 puntos:
1. **Nivel de iluminación requerido (E)**: valor mínimo tabulado según tarea visual (ver Tabla de niveles ya resumida arriba).
2. **Elección del tipo de luminaria**: según la actividad; evitar deslumbramiento, dar bienestar visual.
3. **Índice del local (k)**: número entre 1 y 10 (valores >10 se toman como 10, diferencia despreciable), calculado a partir de la geometría del local (ancho, largo, altura entre luminaria y plano de trabajo — 0,85 m salvo que se ajuste). *(la fórmula completa de k está en la imagen del PDF, pág 44; no transcripta — abrir PDF si se necesita el detalle exacto)*.
4. **Coeficientes de reflexión** de techo, paredes y suelo: tabulados según material/acabado.
5. **Coeficiente de utilización (η)**: relación entre los lúmenes que llegan al plano de trabajo (0,85 m sobre el suelo) y los lúmenes totales de la lámpara. Depende de k y de los factores de reflexión; tabulado por el fabricante de cada luminaria (puede superar 1 por reflexiones múltiples).
6. **Factor de conservación/mantenimiento (fm)**: por envejecimiento de lámparas y suciedad de luminarias. Si el fabricante no lo da: **ambiente limpio fm=0,8**; **ambiente sucio fm=0,6**.
7. **Flujo luminoso total requerido**:
   **ΦT = E·S / (η·fm)**  (E = iluminancia media deseada [lx], S = superficie del plano de trabajo [m²])
   **Número de luminarias: N = ΦT / (n·ΦL)**  (n = lámparas por luminaria, ΦL = flujo de 1 lámpara [lm])
8. **Emplazamiento**: luminarias distribuidas uniformemente en filas paralelas a los ejes de simetría (locales rectangulares); separación máxima según ángulo de apertura del haz y altura de montaje (mayor apertura/altura → más superficie cubierta pero menor iluminancia en el plano); luminarias cercanas a la pared, a la mitad de la distancia entre filas.

**Comprobación de resultados**: Em = N·ΦL·η·fm / S  debe ser **≥ Etablas** (iluminancia recomendada).

### Equivalencias LED vs. incandescente (orientativo, pág 58)
Ejemplos: 1×3W LED ≈ 100-200 lm ≈ 15 W incandescente; 9W LED ≈ 680-800 lm ≈ 50-80 W incandescente; 18W LED ≈ 1300-1500 lm ≈ 140 W incandescente; 40W LED ≈ 2850-3600 lm ≈ 120-270 W incandescente. (Tabla completa en el PDF fuente pág 58.)

### Ejercicios de práctica (pág 49)
1. Sala de traumatología: 7,30×12,20×2,75 m (ancho×largo×alto). Reflexión techo 80%, paredes 50%, plano de trabajo 10%, buena conservación de luz. Diseñar el alumbrado (aplicar el método de los lúmenes completo).
2. Pasillo: 3,05×21,25×3,20 m. Reflexión techo 80%, paredes 50%, plano de trabajo 30%, buena conservación de luz. Diseñar el alumbrado.
3. UTI de 10 camas: diseñar el alumbrado general y calcular tipo y potencia de la lámpara de examen en cada cabecera de cama (considerar dimensiones de la sala y demás factores de diseño; para la lámpara de examen ver niveles de la Tabla de niveles de iluminación — "cuidados intensivos" y "emergencia y cirugía" según el uso).

## Lámpara scialítica (archivo 09, pág 2-10)
Luminaria de quirófano: iluminación homogénea, alta intensidad, **sin calor** y **sin sombras** (elimina sombras de manos/instrumentos). No distorsiona el color de los tejidos.
### Características (pág 3)
- **Temperatura de color** regulable, típicamente **4.500 °K**.
- **Intensidad luminosa** regulable **10.000 – 120.000 lux**.
- **Índice de reproducción cromática (CRI/IRC) alto (>90)** para identificar hemorragias/necrosis.
- Luz "virtualmente fría": filtra infrarrojo y ultravioleta; refleja ~60% de la luz visible. Óptica PRISMALIX (superposición de haces de 2 prismas).
### Requisitos eléctricos (AEA 90364-7-710, pág 9)
Alimentada desde **red IT**; por tiempo de interrupción 0,15–0,5 s → alimentada por **UPS**; conectada a la **barra equipotencial** del quirófano.
### Selección (pág 10)
Según tipo de intervención (intensidad), de pie/techo, fija/retráctil, altura de techo, nº de brazos/satélites.
