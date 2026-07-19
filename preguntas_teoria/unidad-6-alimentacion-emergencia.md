# Unidad 6 — Alimentación de emergencia

¿Explique los pasos a elegir para la elección de un grupo electrógeno?
Son 5 pasos: (1) definir qué servicios hospitalarios se van a alimentar (según su criticidad: servicios críticos como quirófanos, UTI, UTI neonatal, salas de parto, guardia de urgencias, hemodinamia, hemodiálisis, soporte vital; y parcialmente críticos como cuidados intermedios, imágenes, ascensores, esterilización), (2) definir el consumo de esos sectores, (3) definir la potencia mínima requerida, (4) seleccionar el equipo adecuado según disponibilidad de mercado, (5) definir el sistema de transferencia (conmutación o paralelo).

¿Clasificación de los sistemas de alimentación de emergencia?
Ininterrumpidos (tiempo de interrupción 0 s): UPS "on line", grupos electrógenos de servicio continuo. Interrumpidos (hay un corte breve antes de que entre el respaldo): circuitos de CC con acumuladores y/o red propia, UPS "off line", grupos electrógenos en sus distintas configuraciones. En general, según el tiempo de interrupción admitido, las fuentes se clasifican en: sin interrupción (0 s), muy corta (≤0,15 s), corta (0,15-0,5 s), media (0,5-15 s) y larga (>15 s).

¿Diferencias entre un acumulador y un grupo electrógeno?
El acumulador (batería) es una fuente de energía química almacenada: entrega corriente continua y puede suministrar corriente de forma prácticamente inmediata (no necesita "arrancar" como una máquina rotativa). Sin embargo, según cómo esté desplegado en la instalación (circuito de CC con transferencia, o UPS off-line) se lo clasifica como interrumpido, porque hay una etapa de detección y conmutación entre la red y la batería que introduce un corte breve; la excepción es el UPS on-line, donde la batería/inversor ya alimenta la carga de forma continua y por eso se clasifica como ininterrumpido. Su autonomía además está limitada por su capacidad (Ah), se agota. El grupo electrógeno es una máquina rotativa que genera electricidad quemando combustible (nafta, gas o diésel) para mover un alternador: entrega corriente alterna, tarda unos segundos en entrar en servicio (<15 s según norma, por el arranque del motor), es ruidoso y requiere mantenimiento e infraestructura (tanque, ventilación, escape), pero su autonomía es prácticamente ilimitada mientras se le reponga combustible. Por eso en un hospital se combinan: acumuladores/UPS para el corte instantáneo o breve, y el GE para sostener la carga durante un corte prolongado.

¿Esquema de servicio de conmutación?
Es el modo de operación de emergencia: el grupo electrógeno nunca está conectado a la red al mismo tiempo que ella (para no retroalimentarla y proteger al personal de la distribuidora). Un equipo de control de conmutación, con un conmutador de potencia formado por un disyuntor de red y un disyuntor de grupo enclavados entre sí (para que jamás cierren simultáneamente), transfiere la carga de una fuente a la otra ante la falla de la red pública, y la retransfiere cuando la red se normaliza. Es el esquema típico del GE Stand-By hospitalario.

¿Esquema de servicio en paralelo?
El grupo electrógeno se sincroniza con la red pública (misma tensión, frecuencia y ángulo de fase, dentro de tolerancias) y ambas fuentes alimentan la instalación al mismo tiempo, cada una aportando una parte de la carga. Requiere un equipo de sincronismo automático. Se usa para recorte de picos de demanda (aplicación de potencia Prime) o para lograr una transferencia sin corte entre red y grupo (continuidad absoluta del suministro).

¿Clasificación de los grupos (equipos/locales) según tiempo de conmutación?
Manual: conexión/desconexión a mano (6 a 10 s). Automático con arrancador: arranque, conmutación y parada automáticos. Con volante de inercia + motor trifásico: 1 a 2 s. Sin interrupción: el generador alimenta constantemente, accionado por un motor trifásico; ante una falla, el volante de inercia asume el abastecimiento sin corte (0 s). Esta clasificación, junto con la criticidad del servicio, determina qué configuración de GE corresponde a cada sector (un quirófano no puede depender de una conmutación manual de 10 s).

¿Esquema del GE?
Componentes principales: motor de combustión interna (ciclo Otto o Diesel) que acciona un alternador (generador de CA); regulador de velocidad (mantiene la frecuencia en 50 Hz); regulador automático de tensión (AVR, mantiene la tensión de salida constante); sistema de arranque (motor eléctrico de CC o por aire comprimido, según la potencia); sistema de refrigeración (por agua o aire); sistema de escape de gases; tanque y alimentación de combustible; batería de arranque; y tablero de control con instrumentos, protecciones y el sistema de transferencia (que conmuta la carga entre red y grupo).

¿Dispositivos de arranque del GE?
Hasta 1000 kVA, el arranque es por motor eléctrico de corriente continua (alimentado por una batería). Para potencias mayores a 1000 kVA, el arranque es por aire comprimido (más potente, necesario para vencer la inercia de motores diésel grandes). Además, los sistemas de precalefacción (que calientan el motor antes de arrancar) mejoran el tiempo de entrada en servicio.

¿Elección del combustible del GE?
Se elige según el rango de potencia requerido: ciclo Otto (nafta o gas natural), para grupos de hasta 20 kVA; ciclo Diesel (motores de 4 o 2 tiempos), para grupos de hasta 3500 kVA, es el más usado en aplicaciones hospitalarias de mediana/alta potencia, por su robustez y menor consumo específico.

¿Defina potencia Stand-By?
Potencia Stand-By o Fuel Stop Power (FTP): potencia máxima disponible para uso con cargas variables durante un máximo de 500 horas al año, con un factor de carga medio del 90% de la potencia Stand-by declarada. No admite sobrecarga. Es la aplicación típica de respaldo ante fallas de la red eléctrica comercial, el uso habitual de un GE hospitalario.

¿Defina potencia Prime?
Potencia Prime (PRP): valor de potencia máxima disponible para un ciclo de potencia variable, que el generador puede entregar durante un número ilimitado de horas al año. La potencia media en 24 h no debe superar el 80% del valor Prime. Admite una sobrecarga del 10% solo para cargas transitorias (no para alimentación normal). Se usa en aplicaciones donde el grupo es fuente de uso frecuente pero no constante (ej. recorte de punta de demanda).
