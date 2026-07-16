# Guía para el agente (uso de la base de conocimiento)

Objetivo: responder consultas de Ingeniería Hospitalaria (p. ej. resolver un parcial) con el mínimo consumo de tokens, sin cargar los PDF completos.

## Protocolo de consulta (orden obligatorio)
1. **Abrir `INDICE.md`** y localizar el/los tema(s) relevantes por keywords. Es liviano; siempre empezar acá.
2. **Leer solo el/los `resumenes/*.md`** que correspondan. Contienen definiciones, fórmulas, valores numéricos, normas y referencias de página. En la mayoría de los casos alcanza con esto.
3. **Abrir el PDF fuente solo si** se necesita una figura, plano, esquema o tabla no transcripta. La ruta y la página exactas están citadas en cada resumen (formato `archivo (N pág)` y `(pág X)`).
4. Al responder, **citar la resolución/norma y, si aplica, el resumen o el PDF + página** de donde sale el dato.

## Resolver un final / generar ejercicios nuevos
- Antes de resolver un final (propio o nuevo), leer `Finales/finales-resueltos.md`: tiene el criterio ya aplicado a ese tipo de consigna (qué norma usar, qué asumir cuando falta un dato, cómo justificar la decisión de diseño) y sirve de plantilla de estilo de respuesta.
- Cada `resumenes/*.md` de tema (salvo transporte de pacientes y servicios-resoluciones) termina con una sección **"Ejercicios de práctica"** (enunciados de la guía de TP de cátedra, sin resolución modelo) — son otro insumo de consigna real de cátedra, distinto de `Finales/`. Los finales tienden a no parecerse mucho a estos ejercicios (son de TP, no de examen), así que al generar un final nuevo dar más peso al estilo/nivel de `Finales/finales-resueltos.md` y usar estos ejercicios sobre todo como fuente de datos/escenarios (nº de camas, servicios, equipos) para variar.
- Para generar un final/ejercicio nuevo: combinar un caso de `Finales/finales-resueltos.md` (o un enunciado de "Ejercicios de práctica") con los datos de `resumenes/` del tema pedido, y variar los números/servicio; no inventar normas o resoluciones que no estén citadas en los resúmenes.
- Si faltan datos del enunciado (n° de camas, superficie, etc.), decirlo explícitamente y resolver con el criterio/método aplicable, sin inventar la cifra faltante.
- El final 20/02/2025 tiene exactamente 6 preguntas (100 puntos: 25+15+15+10+20+15) — no inventar preguntas 7 en adelante para ese final aunque el archivo de resolución las haya tenido antes por error.

## Reglas de precisión
- Priorizar valores de `servicios-hospitalarios-resoluciones.md` cuando la pregunta sea "qué exige la norma" (m², bocas, T/HR) — es la referencia normativa.
- Priorizar `gases-medicinales.md` e `instalaciones-electricas.md` para cálculos (diámetros, secciones, caudales, potencias).
- Varios PDFs de gases/radiología son imágenes escaneadas; su texto fue obtenido por OCR (motor inglés) y puede tener typos en tildes. Los números/fórmulas fueron revisados, pero ante duda numérica crítica, verificar contra el PDF fuente en la página citada.
- Si un dato no está en los resúmenes, decirlo y ofrecer abrir el PDF fuente; no inventar cifras.

## Mantenimiento
Al agregar nuevos PDFs a `Clases actualizadas/`: extraer texto (con OCR si es escaneo), crear/actualizar el `resumenes/*.md` del tema y agregar la fila correspondiente en `INDICE.md`.
Al agregar un final nuevo: guardar la fuente (foto/PDF) en `Finales/<fecha>/` y sumar su resolución a `Finales/finales-resueltos.md` con el mismo formato (enunciado resumido + resolución citando resúmenes de tema).
