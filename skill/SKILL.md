---
name: ficha-de-datos
description: Prepara un análisis de datos de investigación antes de escribir código. Completa la ficha del dataset, diagnostica los datos y recomienda la familia de machine learning con su justificación.
---

# Ficha de datos

Usa esta skill cuando la persona comparta un conjunto de datos, una pregunta de investigación o pida un análisis con machine learning.

## Pasos

1. **Ficha primero.** Antes de analizar, completa con la persona la ficha del dataset: pregunta, unidad de análisis, familia de ML, criterios, cómo verifica, variables y estado del dato, herramienta. Si falta algo, pregúntalo; no lo supongas.
2. **Diagnóstico.** Revisa el dataset y reporta: número de filas y columnas, qué representa cada fila, faltantes por variable, duplicados, tipos de variable y valores raros.
3. **Familia.** Recomienda supervisado, no supervisado o mixto según si existe una respuesta conocida en todos, ninguno o unos pocos casos. Explica por qué en dos o tres frases.
4. **Plan antes del código.** Propón los pasos del análisis y espera confirmación.
5. **Reporte.** Al terminar, di qué hiciste, qué resultado obtuviste, qué no es concluyente y cómo se puede verificar.

## Reglas

- No inventes datos ni completes faltantes sin decirlo.
- En problemas supervisados, guarda una parte de los datos para probar y reporta el resultado con esos datos.
- Divide según los datos: al azar con semilla fija; estratificada si una clase es rara; por tiempo en series (entrenar con el pasado, probar con el futuro); por grupos si un mismo caso aparece varias veces. Evita la fuga de datos: prepara (escalar, imputar) solo con el entrenamiento.
- Al clasificar, reporta precision, recall, F1 y AUC-ROC además de la exactitud, y pregunta qué error cuesta más (exclusión o inclusión) antes de escoger el punto de corte.
- Al predecir un número, reporta RMSE y R² en datos de prueba; cuando sea posible, un intervalo bootstrap para la cifra principal.
- Compara siempre contra una alternativa simple (repetir el último dato, la categoría más frecuente).
- En problemas no supervisados, deja por fuera la variable que se quiere explicar y úsala después para validar.
- Explica en lenguaje sencillo; la persona decide qué resultado creer.
