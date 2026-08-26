# Final generado C — Diagnóstico por imágenes (TC + Hemodinamia)

> **Generado por el agente — enunciado en blanco (sin resolución) — sin plano.**
> Servicio ancla: **Tomografía computada (TC) + sala de Hemodinamia** (Institución Nivel III de riesgo).
> Datos inspirados en `Finales/finales-resueltos.md` (final RX 20/02/2025) + `resumenes/`. Sin plano: los datos van en el texto.
> Para autoevaluarte: resolvelo entero y después pedime "corregí el Final C".
> **6 preguntas — 100 puntos (15 + 25 + 15 + 10 + 15 + 20).**

---

## Enunciado

Una institución **Nivel III de riesgo** monta un servicio de imágenes con un **tomógrafo (TC)** y una **sala de hemodinamia**. Especificaciones de preinstalación:

- Equipo de **TC**: alimentación trifásica, potencia de placa 55 kW; por su régimen de trabajo (disparos intermitentes) se considera una **carga de 35 kW** durante los cortes. Bajada de línea directa, tensión de fase 370–400 V.
- El fabricante exige **R aparente del conductor de la bajada del TC < 0,30 Ω** y **RPAT < 1 Ω**.
- El servicio está a **480 m lineales** de la entrada de suministro eléctrico.
- Terreno adyacente **homogéneo, ρ = 20 Ω·m**.
- La sala de hemodinamia tiene un equipo de RX de radiación pulsada de **80 kW** recomendados y climatización con filtros HEPA terminales.
- La **fuente de vacío** del servicio (compartida con el resto del sector crítico) debe actualizarse. La instalación actual funciona con **2 bombas de anillo de agua de 5,5 HP**. El caudal de vacío de la instalación es **inferior a 1900 l/min**. Tabla de bombas disponibles del proveedor:

  | Modelo | 870C | 1170C | 1870C | 2670C | 3820C |
  |---|---|---|---|---|---|
  | Caudal [l/min] | 850 | 1100 | 1850 | 2600 | 3800 |
  | Caudal [m³/h] | 51 | 66 | 111 | 156 | 228 |
  | HP | 2 | 3 | 4 | 5,5 | 10 |
  | RPM | 2800 | 2800 | 1400 | 1400 | 1400 |

---

**1) Definiciones y clasificación** *(15P)*
a) Defina el servicio de TC y el de Hemodinamia; indique la superficie mínima y los locales que exige cada uno (Res. 3590/2021 y Res. 1184/2018).
b) Clasifique ambas salas según AEA 90364-7-710 y justifique.

**2) Diseñe la instalación eléctrica del equipo de TC.** *(25P)*
a) Dimensione el circuito dedicado del equipo (corriente de trabajo, protecciones mínimas: termomagnética trifásica + diferencial). Justifique si dimensiona por la potencia de placa o por la carga considerada.
b) Determine la **sección del conductor de la bajada** teniendo en cuenta que a **480 m** debe cumplirse **R aparente < 0,30 Ω**. Aclare si corresponde o no duplicar la longitud y por qué (criterio de resistencia vs. caída de tensión).
c) Dimensione la puesta a tierra para cumplir **RPAT < 1 Ω** con el terreno dado (nº de jabalinas, largo, separación).

**3) Diseñe la instalación de gases medicinales del servicio de imágenes** (TC + recuperación + hemodinamia). *(15P)*
Indique bocas por gas, caudales de diseño, presiones de trabajo, recorrido de cañerías y válvulas de seccionamiento. Justifique qué modalidades de imágenes requieren gases centralizados y cuáles no.

**4) Climatización del servicio** *(10P)*
Indique las condiciones de climatización de la sala de TC (gantry / sala técnica) y de la sala de hemodinamia. ¿Por qué la hemodinamia exige filtros HEPA terminales y la TC no necesariamente?

**5) Automatismo — bomba de vacío / compresor** *(15P)*
Las bombas del sistema de vacío se comandan con motores trifásicos.
a) Describa el circuito de comando y de potencia para el arranque, y cómo se realizaría la **inversión de giro** de un motor trifásico.
b) ¿Qué función cumple un **temporizador** en la secuencia de arranque de bombas en configuración duty/standby? Describa los contactos de un contactor y las características para comprarlo.

**6) Fuente de vacío medicinal** *(20P)*
Rediseñe la fuente de vacío del sector según la normativa vigente (IRAM-ISO 7396-1).
a) ¿Cumple la instalación actual (2 bombas de anillo de 5,5 HP)? Justifique con la norma **antes** de mirar la tabla.
b) Con la tabla de bombas y el dato de que el caudal es **< 1900 l/min**, seleccione el modelo y la configuración (nº de bombas, duty/standby), verificando que ante la falla de una bomba el resto cubra el 100 % de la demanda.
c) Realice el croquis del sistema de vacío (colector, trampa de líquido, filtro bacteriano, depósito, alarmas).
