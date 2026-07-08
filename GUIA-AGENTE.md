# Guía para el agente (uso de la base de conocimiento)

Objetivo: responder consultas de Ingeniería Hospitalaria (p. ej. resolver un parcial) con el mínimo consumo de tokens, sin cargar los PDF completos.

## Protocolo de consulta (orden obligatorio)
1. **Abrir `INDICE.md`** y localizar el/los tema(s) relevantes por keywords. Es liviano; siempre empezar acá.
2. **Leer solo el/los `resumenes/*.md`** que correspondan. Contienen definiciones, fórmulas, valores numéricos, normas y referencias de página. En la mayoría de los casos alcanza con esto.
3. **Abrir el PDF fuente solo si** se necesita una figura, plano, esquema o tabla no transcripta. La ruta y la página exactas están citadas en cada resumen (formato `archivo (N pág)` y `(pág X)`).
4. Al responder, **citar la resolución/norma y, si aplica, el resumen o el PDF + página** de donde sale el dato.

## Reglas de precisión
- Priorizar valores de `servicios-hospitalarios-resoluciones.md` cuando la pregunta sea "qué exige la norma" (m², bocas, T/HR) — es la referencia normativa.
- Priorizar `gases-medicinales.md` e `instalaciones-electricas.md` para cálculos (diámetros, secciones, caudales, potencias).
- Varios PDFs de gases/radiología son imágenes escaneadas; su texto fue obtenido por OCR (motor inglés) y puede tener typos en tildes. Los números/fórmulas fueron revisados, pero ante duda numérica crítica, verificar contra el PDF fuente en la página citada.
- Si un dato no está en los resúmenes, decirlo y ofrecer abrir el PDF fuente; no inventar cifras.

## Mantenimiento
Al agregar nuevos PDFs a `Clases actualizadas/`: extraer texto (con OCR si es escaneo), crear/actualizar el `resumenes/*.md` del tema y agregar la fila correspondiente en `INDICE.md`.
