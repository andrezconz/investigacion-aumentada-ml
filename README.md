# Machine Learning: herramientas para trabajar con datos

Material de la **Sesión 8 de Investigación Aumentada** (jueves 19 de noviembre de 2026).
Andrez Felipe Guerrero Torres.

Este repositorio acompaña la sesión: una ficha en markdown que se llena en vivo, una guía de Teachable Machine y un notebook por cada ejemplo, listos para correr en Google Colab sin instalar nada.

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
| 05 | Pronóstico de El Niño con ARIMA | Serie de tiempo | Supervisado | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/05_series_tiempo_el_nino.ipynb) |
| 06 | Codificar textos con pocos ejemplos | Texto | Mixto (semi-supervisado) | [![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/andrezconz/investigacion-aumentada-ml/blob/main/notebooks/06_texto_semisupervisado.ipynb) |

## Qué hay aquí

```
ficha/
  ficha_en_vivo.md        plantilla que se llena durante la sesión, bloque a bloque
  ficha_luces_cauca.md    la misma ficha, completa, para el caso del Cauca
  libro_de_codigos.md     libro de códigos para el ejercicio de texto
skill/
  SKILL.md                la ficha convertida en skill para un asistente de IA
teachable_machine.md      guía para entrenar un clasificador de imágenes sin código
notebooks/                seis notebooks para Google Colab
datos/                    los datos que usan los notebooks
```

## La ficha en vivo

| Bloque | Qué llenamos |
|---|---|
| 1 · Preparar el terreno con IA | Pregunta y unidad de análisis |
| 2 · Qué es machine learning | Familia de ML |
| 3 · Capacidad y agencia | Criterios y cómo verifico |
| 4 · Tipos de datos | Variables y estado del dato |
| 5 · Colombia vista con datos | Herramienta |
| 6 · Cierre | Convertirla en skill |

## Fuentes de los datos

- `titanic3.csv`: Vanderbilt University, Department of Biostatistics.
- `desarrollo_paises_real.csv`: Banco Mundial (WDI y Worldwide Governance Indicators) y PNUD (IDH).
- `cauca_viirs_2014.tif`, `cauca_viirs_2026.tif`: NOAA VIIRS DNB, compuestos mensuales de enero a mayo vía Google Earth Engine, recortados al Cauca.
- `cauca_limite.geojson`: Marco Geoestadístico Nacional, DANE.
- El Niño (notebook 05): NOAA Physical Sciences Laboratory, Oceanic Niño Index. Se descarga al correr el notebook.
- `nombres_ejemplo.csv` y `fragmentos_practica.csv`: **ficticios**, construidos para la práctica.

Procesamiento y notebooks: elaboración propia.
