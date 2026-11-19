# Ficha del dataset · Luces nocturnas del Cauca

> Versión completa de la ficha que se construye en vivo durante la sesión.

## 1. Pregunta de investigación
¿Qué zonas del Cauca se iluminaron entre 2014 y 2026 y cuáles siguen a oscuras? Sirve como una primera lectura territorial para orientar trabajo de campo.

## 2. Unidad de análisis
Un píxel de cerca de 1 km². En un segundo paso, el municipio (suma o promedio de sus píxeles).

## 3. Familia de machine learning
- Hoy: comparación directa entre dos años (todavía no es un modelo).
- Agrupar píxeles o municipios por su trayectoria de luz: **no supervisado** (K-Means), porque nadie ha dicho qué es «se encendió».
- Estimar pobreza desde la luz usando encuestas como respuesta conocida: **supervisado**.

## 4. Criterios
- Comparar los mismos meses (enero a mayo) en ambos años para no mezclar temporadas.
- Reportar el umbral usado para «luz clara» (más de 1 nW/cm²/sr).
- No leer la luz como desarrollo: es un indicador.
- No inventar datos faltantes.
- Decir lo que no es concluyente.

## 5. Cómo verifico
- Contrastar con conocimiento de campo y con datos de cobertura eléctrica y población.
- Caso de control: Popayán debe aparecer iluminada en ambos años.
- Revisar el centro de Popayán, que parece perder luz: una hipótesis es el cambio a luminarias LED, que el sensor capta peor.

## 6. Variables y estado del dato
- radiancia_2014: luz nocturna media de enero a mayo de 2014 (número, nW/cm²/sr).
- radiancia_2026: lo mismo para 2026 (número).
- límite departamental (polígono).
- Estado: dato duro y limpio (compuesto mensual, negativos llevados a 0), **sin etiqueta**.

## 7. Herramienta
Google Earth Engine para descargar los compuestos; notebook `04_imagenes_luces_cauca.ipynb` en Google Colab para comparar y agrupar.

*Fuente: NOAA VIIRS DNB, compuestos mensuales vía Google Earth Engine. Límite: Marco Geoestadístico Nacional, DANE. Elaboración propia.*
