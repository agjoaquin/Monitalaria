# Automatismo (elementos de mando y maniobra)
Fuente: `Clases actualizadas/Automatismo/Automatismo 2024.pptx.pdf` (16 pág) · Bioing. Mónica Baroli

## Mando/maniobra (pág 2)
Elementos capaces de conectar o interrumpir partes de un circuito, bajo carga o en vacío. Ej.: pulsadores, interruptores, conmutadores, relés, contactores, sensores.

## Pulsadores (pág 3-5)
Accionamiento manual, sin enclavamiento (retornan por resorte). Configuraciones: **NA** (normalmente abierto) y **NC** (normalmente cerrado). Tipos: simple, luminoso, encapsulado, botonera arranque/parada.
Código de colores: ROJO=emergencia/parada; AMARILLO=anomalía; AZUL=obligatorio/rearme; VERDE/BLANCO=normal (marcha); BLANCO/GRIS/NEGRO=sin significado específico.

## Interruptores y conmutadores (pág 6)
Acción manual, mantienen posición. Interruptor: abre/cierra un mismo circuito. Conmutador: abre uno y cierra otro simultáneamente.

## Relés (pág 7)
Interruptores accionados por electroimán (bobina + armadura de hierro). Protección de motores/equipos ante sobrecargas. Al circular corriente por la bobina se genera campo electromagnético que desplaza los contactos.

## Contactores (pág 8)
Abren/cierran contactos por electroimán. Contactos de **fuerza** (accionan receptores: motores, alumbrado) y **auxiliares** (NA y NC).

## Relés temporizadores (pág 9-11)
Retrasan apertura/cierre un tiempo predeterminado. Tres tipos:
- A la conexión: cuenta desde que el relé recibe corriente.
- A la desconexión: cuenta desde que cesa la corriente.
- A la conexión/desconexión: combinación de ambos.

## Otros elementos
- Detectores/sensores (pág 12): responden ante presencia del elemento a detectar; los electrónicos no requieren contacto físico.
- Indicadores luminosos (pág 13): se conectan siempre en paralelo a la bobina.

## Circuitos de potencia y comando (pág 14-15)
- Circuito de **potencia**: circulación de corriente nominal, fuente→carga.
- Circuito de **comando/mando**: elementos para accionar la bobina del contactor.
- Ejemplo: inversión de sentido de giro con dos contactores (giro horario BH / antihorario BAH), llave arranque/parada (S) y temporizador (T).

---
## Complemento — Guía de práctica, Guía Nº 4 (pág 38-43)
Fuente: `Clases actualizadas/Guía de práctica/Guía de práctica 2026.pdf`

### Contactor — definición y construcción ampliada
El contactor es un aparato de mando destinado a comandar equipamiento eléctrico en estado no perturbado o bajo sobrecargas normales de servicio, accionable a distancia y apto para altas frecuencias de operación. Tiene solo 2 estados: estable/reposo (sin acción del circuito de mando) e inestable (accionado y sostenido por su sistema de operación). Puede operar corrientes de **6 a 12 veces la corriente nominal**; poca inercia mecánica, respuesta rápida. Combinado con relés adecuados protege cargas (generalmente motores) contra falta de fase, sobretensión, sobrecarga, corrientes inversas — pero **la protección contra cortocircuito requiere otro elemento aguas arriba** (ej. fusibles).

**Elementos constructivos:**
- **Contactos principales**: en las vías de conducción de la corriente de servicio; abren/cierran el circuito de potencia; 2 puntos de interrupción; abiertos en reposo. Según nº de vías: bipolar, tripolar, tetrapolar (maniobra simultánea en todas las vías).
- **Contactos auxiliares**: acoplados mecánicamente a los principales; abren/cierran circuitos auxiliares/de mando, aseguran enclavamientos y señalización. Tipo NA o NC, 2 puntos de interrupción, dimensiones reducidas (corrientes pequeñas).
- **Bobina**: genera fuerza de atracción al circular corriente; alimentación 12/24/110/220 V CA o CC.
- **Armadura**: parte móvil; desplaza los contactos por la fuerza de atracción de la bobina.
- **Núcleo**: parte fija que cierra el flujo magnético de la bobina.
- **Resortes antagónicos**: devuelven los contactos a reposo al cesar la atracción.
- **Cámaras de extinción (apagachispas)**: alojan los contactos y alargan/dividen/extinguen el arco de ruptura.
- **Soporte**: fija las piezas entre sí y al tablero (tornillos o riel DIN).

**Funcionamiento**: al excitarse la bobina, el núcleo atrae la armadura y arrastra los contactos (por rotación, traslación o combinación), cerrando el circuito red-receptor. Al des-energizar la bobina, los resortes abren los contactos. Si se gobierna desde varios puntos: pulsadores de marcha en **paralelo**, pulsadores de parada en **serie** con la bobina.

### Símbolos adicionales
Contacto NA = k impar; contacto NC = k par. Pulsador NC de parada = p; pulsador NA de arranque = a. Protector térmico (NC) = t°. Interruptor = s. Conmutador = c.

### Ejercicios de práctica (Guía de cátedra 2026, pág 42-43)
1. Circuito de comando y potencia para iluminación de estacionamiento subterráneo de un hospital: 40 lámparas de 60 W (30 de accionamiento manual, siempre encendidas; 10 por célula fotoeléctrica); luces indicadoras en el tablero.
2. Circuito de mando de una incubadora neonatal: 2 sensores (calefacción y alarma fonoluminosa); temperatura consigna 36,5 °C, máxima 38 °C (el sistema se desconecta al superarla); indicadores de encendido, calefacción, baja temperatura y temperatura óptima.
3. Circuito con contactores para apertura/cierre de un portón de acceso de ambulancia: apertura manual (pulsador/llave/control remoto), cierre automático invirtiendo la marcha del motor, luces indicadoras en el tablero.
4. Mesa basculante de un equipo de RX (motor trifásico 0,75 kW, movimiento 90° a −15°): esquema de mando con opciones trendelenburg/antitrendelenburg/horizontal, dispositivos de fin de carrera y stop.
5. (Trabajo de laboratorio) Esterilizador por vapor: resistencias ~700 W comandadas por contactor (encendidas con el equipo, hasta fin de ciclo) + bomba de vacío con motor trifásico en estrella (funciona 30 s tras el encendido) + pulsador de parada de emergencia (aborta ciclo y apaga el equipo). Realizar esquemas de mando y potencia.
