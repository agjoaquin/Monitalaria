# Alimentación de emergencia
Fuente: `Clases actualizadas/Alimentación de emergencia/Alimentación de emergencia.pptx.pdf` (15 pág) · Bioing. Mónica Baroli
Tema: provisión de energía auxiliar confiable ante corte de suministro (riesgo de vida en hospital).

## Clasificación de fuentes según tiempo de interrupción (pág 3)
- Sin interrupción: 0 s
- Muy corta: hasta 0,15 s
- Corta: 0,15 – 0,5 s
- Media: 0,5 – 15 s
- Larga: > 15 s

## Sistemas de alimentación de emergencia (pág 4)
- **Ininterrumpidos**: UPS "on line"; grupos electrógenos de servicio continuo.
- **Interrumpidos**: circuitos de CC con acumuladores y/o red propia; UPS "off line"; grupos electrógenos (diversas configuraciones).

## UPS ON LINE — especificaciones (pág 5)
Potencia mín. X kVA · doble inversión · factor de potencia ≥0,9 · entrada/salida 220 V 50 Hz · mín. 4 tomacorrientes · display de parámetros · alarmas · protección sobrecarga y cortocircuito.

## Grupos electrógenos (GE) (pág 6-7)
- Potencias: 0,8 kVA – 3500 kVA.
- Ciclo Otto (nafta/gas natural) hasta 20 kVA; Ciclo Diesel (4 o 2 tiempos) hasta 3500 kVA.
- Sistemas de precalefacción mejoran tiempo de arranque.
- **Tiempo de entrada en servicio < 15 s.**
- Arranque: hasta 1000 kVA motor eléctrico CC; >1000 kVA por aire comprimido.
- **Tipos de potencia**:
  - COP (continua): sin límite de horas; donde no hay red comercial.
  - PRP (Prime): ciclo variable ilimitado; media 24 h ≤80% del valor Prime; sobrecarga 10% solo transitoria.
  - FTP/Stand-By: máx. disponible 500 h/año, factor carga medio 90%; no admite sobrecarga; respaldo ante fallas de red.

## Configuraciones de automatismo GE (pág 12-13)
- Manual: conexión/desconexión a mano (6 a 10 s).
- Automático con arrancador: arranque, conmutación y parada automáticos.
- Con volante de inercia + motor trifásico: 1 a 2 s.
- Sin interrupción: generador alimenta constantemente, accionado por motor trifásico; ante falla, volante de inercia asume el abastecimiento.

## Criterio de dimensionamiento del GE (pág 14)
1. Definir servicios hospitalarios a alimentar. 2. Definir consumo de esos sectores. 3. Definir potencia mínima requerida. 4. Seleccionar equipo según mercado. 5. Definir sistema de transferencia.

---
## Complemento — Guía de práctica, Guía Nº 6 (pág 59-62)
Fuente: `Clases actualizadas/Guía de práctica/Guía de práctica 2026.pdf`

### Clasificación de servicios hospitalarios según criticidad eléctrica
Clave para decidir el paso 1 del dimensionamiento (qué se alimenta desde el GE).

**Servicios críticos** (deben tener alimentación de emergencia):
- Quirófanos
- UTI
- UTI neonatal
- Salas de parto
- Guardia de urgencias
- Salas de angiografía/hemodinamia
- Hemodiálisis
- Laboratorios de urgencias
- Sistema de soporte vital: compresores de aire medicinal, bombas de vacío, PSA (planta de oxígeno por adsorción), telemetría
- Sistemas de iluminación general de emergencia

**Servicios parcialmente críticos** (según diseño, pueden recibir emergencia parcial o con prioridad menor):
- Unidades de cuidados intermedios
- Servicios de diagnóstico por imágenes
- Elevadores y montacargas
- Iluminación de accesos y circulación prioritaria
- Suministro de agua potable
- Pozos de bombeo cloacales
- Sistemas de seguridad y vigilancia
- Monitoreo de equipos y maquinaria
- Esterilización

### Ejercicios de práctica (pág 62)
1. Calcular la potencia del GE para: UTI 8 camas, UTIP 4 camas, Neonatología 5 puestos, 3 quirófanos, 1 sala de partos, 2 ascensores, sala de máquinas (2 compresores 5,5 HP c/u + 2 bombas de vacío 3 HP c/u, todos trifásicos), internación 35 habitaciones dobles con AA 3000 frig. c/u, internación 12 habitaciones individuales con AA 3000 frig. c/u, laboratorio de análisis clínicos (3000 W de equipos + AA 4500 frig.).
2. Institución pediátrica de 3 plantas: 2 pisos de internación (25 habitaciones de 1 cama + office de enfermería c/u), PB con guardia/laboratorio/2 quirófanos/UTI de 10 camas. Indicar: (a) qué servicios recibirían alimentación de un GE en el subsuelo; (b) tensión y potencia características del GE.
3. Diseñar un panel de cabecera de UTI con alimentación de red y de emergencia, solo en la mitad de sus tomacorrientes.

*Nota: estos ejercicios requieren sumar potencias de equipos (HP→kW, frigorías→kW, W) y aplicar simultaneidad/criterio propio; no hay coeficientes de simultaneidad para GE citados en los resúmenes — si un final los pide, aclarar el supuesto adoptado en vez de inventar un factor.*
