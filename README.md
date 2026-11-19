# Machine Learning: herramientas para trabajar con datos

Material de la **Sesión 8 de Investigación Aumentada** (jueves 19 de noviembre de 2026).
Andrez Felipe Guerrero Torres.

Este repositorio acompaña la sesión: una ficha en markdown que se llena en vivo, una guía de Teachable Machine y ocho notebooks, uno por ejemplo, listos para correr en Google Colab sin instalar nada. Todas las cifras de la presentación salen de estos notebooks.

## Cuaderno de la sesión

[**Descargar el cuaderno en PDF**](cuaderno/cuaderno_sesion8_machine_learning.pdf): conceptos, los cinco casos con su tip, herramientas por tipo de dato, la ficha completa, la skill, prompts para copiar y glosario.

## Cómo usarlo

1. Abre un notebook con el botón **Abrir en Colab**.
2. En Colab: menú **Entorno de ejecución → Ejecutar todas**.
3. Lee las celdas de texto: cada notebook dice qué hace, cómo funciona la técnica y deja un tip para tu investigación.

| # | Notebook | Tipo de dato | Familia | Abrir |
|---|---|---|---|---|
| 01 | Árbol de decisión: ¿quién sobrevivió al Titanic? | Datos duros | Supervisado | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/01_supervisado_arbol_titanic.ipynb) |
| 02 | K-Means: ¿existen tipos de países? | Datos duros | No supervisado | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/02_no_supervisado_kmeans_paises.ipynb) |
| 03 | Limpieza de nombres e Isolation Forest | Datos crudos | No supervisado | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/03_datos_crudos_nombres.ipynb) |
| 04 | Luces nocturnas del Cauca, 2014 y 2026 | Imágenes de satélite | Comparación y no supervisado | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/04_imagenes_luces_cauca.ipynb) |
| 05 | Pronóstico del tráfico aéreo con ARIMA | Serie de tiempo | Supervisado | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/05_series_tiempo_trafico_aereo.ipynb) |
| 06 | Codificar textos con pocos ejemplos | Texto | Mixto (semi-supervisado) | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/06_texto_semisupervisado.ipynb) |
| 07 | Una red neuronal que lee dígitos (y se equivoca) | Imágenes | Supervisado | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/07_red_neuronal_digitos.ipynb) |
| 08 | Medir un modelo: dividir los datos, ecuación de Mincer y focalización tipo Sisbén (accuracy, precision, recall, F1, AUC-ROC) | Datos duros (simulados) | Supervisado | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/08_metricas_mincer_sisben.ipynb) |

## Qué hay aquí

```
cuaderno/
  cuaderno_sesion8_machine_learning.pdf   todo el contenido de la sesión en PDF
prompts.md                prompts para copiar, para usar junto con la ficha
ficha/
  ficha_en_vivo.md        plantilla que se llena durante la sesión, bloque a bloque
  ficha_luces_cauca.md    la misma ficha, completa, para el caso del Cauca
  libro_de_codigos.md     libro de códigos para el ejercicio de texto
skill/
  SKILL.md                la ficha convertida en skill para un asistente de IA
teachable_machine.md      guía para entrenar un clasificador de imágenes sin código
notebooks/                ocho notebooks para Google Colab
datos/                    los datos que usan los notebooks
```

## La sesión en dos partes

**Parte 1 · Conceptos y ejemplos:** bases del machine learning (vocabulario, familias, siete tareas, la ecuación de Mincer); datos, medición y límites (dividir en entrenamiento, validación y prueba; preparar, optimizar, remuestrear, bootstrap; accuracy, precision, recall, F1 y AUC-ROC con un ejemplo tipo Sisbén); tipos de datos y tres proyectos reales. Mientras avanza, cada asistente escribe su skill de ML en un bloc de notas (`mi-skill-ml.md`).
**Parte 2 · Aplicación con IA:** archivos .md y la ficha en vivo, Teachable Machine, niveles de delegación, herramientas y notebooks, y la skill.

## La ficha en vivo

Se llena en el bloque 5 con el caso de las luces nocturnas del Cauca. Cada sección aplica un concepto de la parte 1:

| Sección de la ficha | Concepto de la parte 1 |
|---|---|
| Pregunta de investigación | La pregunta define la familia |
| Unidad de análisis | Tipos de datos |
| Familia de ML | Supervisado, no supervisado y mixto |
| Criterios | Capacidad y límites |
| Cómo verifico | Datos de prueba |
| Variables y estado del dato | Duros, crudos, sin etiqueta |
| Herramienta | Herramientas por tipo de dato |

## Fuentes de los datos

- `titanic3.csv`: Vanderbilt University, Department of Biostatistics.
- `desarrollo_paises_real.csv`: Banco Mundial (WDI y Worldwide Governance Indicators) y PNUD (IDH).
- `cauca_viirs_2014.tif`, `cauca_viirs_2026.tif`: NOAA VIIRS DNB, compuestos mensuales de enero a mayo vía Google Earth Engine, recortados al Cauca.
- `cauca_limite.geojson`: Marco Geoestadístico Nacional, DANE.
- `tsa_trafico_diario.csv`: TSA (Transportation Security Administration, EE. UU.), pasajeros diarios en controles de seguridad publicados en tsa.gov.
- Dígitos (notebook 07): Optical Recognition of Handwritten Digits, UCI Machine Learning Repository, incluido en scikit-learn.
- `nombres_ejemplo.csv` y `fragmentos_practica.csv`: **ficticios**, construidos para la práctica.

Procesamiento y notebooks: elaboración propia.
