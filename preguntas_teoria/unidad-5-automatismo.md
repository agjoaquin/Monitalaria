# Unidad 5 — Automatismo

¿Defina contactor?
Es un aparato de mando destinado a comandar equipamiento eléctrico en estado no perturbado o bajo sobrecargas normales de servicio, accionable a distancia y apto para altas frecuencias de operación. Abre y cierra sus contactos por medio de un electroimán. Solo tiene 2 estados posibles: estable/reposo (sin acción del circuito de mando, contactos abiertos) e inestable (accionado y sostenido por su sistema de operación, contactos cerrados).

¿Características básicas de un contactor?
Puede operar corrientes de 6 a 12 veces la corriente nominal; tiene poca inercia mecánica y respuesta rápida. Combinado con relés adecuados, protege cargas (generalmente motores) contra falta de fase, sobretensión, sobrecarga y corrientes inversas, pero no protege por sí solo contra cortocircuito, eso requiere otro elemento aguas arriba (ej. fusibles). Construcción: contactos principales (potencia, 2 puntos de interrupción, abiertos en reposo, bipolar/tripolar/tetrapolar), contactos auxiliares (NA/NC, para mando, señalización y enclavamientos), bobina (12/24/110/220 V CA o CC), armadura (parte móvil), núcleo (parte fija), resortes antagónicos (retorno a reposo) y cámara de extinción (apaga el arco al abrir).

¿Defina sistema de enclavamiento?
Es un sistema de seguridad que impide que dos elementos (típicamente dos contactores) se activen al mismo tiempo cuando eso generaría una condición peligrosa. Se implementa conectando un contacto auxiliar NC de cada contactor en serie con la bobina del otro: al energizarse uno, abre el circuito de mando del contrario. El caso típico es la inversión de sentido de giro de un motor: sin enclavamiento, si se energizan a la vez el contactor de giro horario y el de antihorario se produce un cortocircuito franco entre fases.

¿Criterio de elección de contactor?
Se elige en función de: la corriente nominal de la carga a comandar (el contactor debe soportar igual o más), la categoría de empleo según el tipo de carga (AC-1 para cargas resistivas o poco inductivas; AC-3 para motores asíncronos de jaula de ardilla, que exige soportar la corriente de arranque), la tensión de la bobina de mando disponible en el circuito de control, el número de polos/contactos auxiliares necesarios, y la frecuencia de maniobra esperada (vida útil eléctrica/mecánica del contactor).

¿Diferencia entre un interruptor NC y un pulsador NC?
El interruptor es de accionamiento manual pero mantiene la posición tras accionarlo: un interruptor NC arranca cerrado y, al accionarlo, pasa a abierto y se queda así hasta la próxima maniobra. El pulsador no tiene enclavamiento: vuelve a su posición de reposo por resorte apenas se deja de presionar. Un pulsador NC está cerrado en reposo, se abre solo mientras se lo mantiene presionado, y se cierra de nuevo al soltarlo.

¿Qué es un aparato de mando?
Es cualquier elemento de un circuito eléctrico capaz de conectar o interrumpir una o varias partes de la línea que transporta la energía, ya sea bajo carga o en vacío.

¿Clasificación de aparatos de mando?
Pulsadores: accionamiento manual sin enclavamiento (retorno por resorte); NA o NC; tipos simple, luminoso, encapsulado, botonera de arranque/parada; código de colores (rojo=emergencia/parada, amarillo=anomalía, azul=obligatorio/rearme, verde/blanco=marcha normal). Interruptores: acción manual, mantienen posición; abren o cierran un mismo circuito. Conmutadores: acción manual, mantienen posición; abren un circuito y cierran otro simultáneamente. Relés: interruptores accionados por electroimán; protegen motores/equipos ante sobrecargas. Contactores: abren/cierran contactos por electroimán; contactos de fuerza y auxiliares. Relés temporizadores: retrasan la apertura/cierre un tiempo predeterminado (a la conexión, a la desconexión, o a la conexión/desconexión combinadas). Detectores/sensores: responden ante la presencia del elemento a detectar (los electrónicos no requieren contacto físico). Indicadores luminosos: se conectan siempre en paralelo a la bobina, para señalizar el estado del sistema.
