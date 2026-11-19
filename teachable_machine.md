# Teachable Machine: entrenar un clasificador sin código

[teachablemachine.withgoogle.com](https://teachablemachine.withgoogle.com) es una herramienta gratuita de Google para entrenar un modelo **supervisado** desde el navegador, con la cámara o con imágenes propias.

## En la sesión (bloque 2)

1. Entra a la página y escoge **Proyecto de imagen → Modelo de imagen estándar**.
2. Crea dos o tres clases. Por ejemplo: «taza», «libro» y «nada».
3. Con la cámara, toma unas 30 imágenes por clase.
4. Pulsa **Entrenar modelo** y prueba con objetos que no vio.

**¿Qué familia es?** Supervisado: cada imagen llegó con su etiqueta, que es la respuesta conocida.

## En el bloque 3: hacerlo fallar

- Cambia el fondo, la luz o la distancia y mira cómo cambia la predicción.
- Muestra un objeto que no está en ninguna clase: el modelo igual escoge una.

Si falla con otro fondo es porque aprendió del fondo y no solo del objeto. Es el mismo problema del sesgo de datos: el modelo aprende lo que hay en los ejemplos, incluido lo que no querías enseñarle.

## Para llevarlo a la investigación

- **Tip:** varía fondos, luces y ángulos en los ejemplos de entrenamiento.
- Imágenes de campo (cultivos, viviendas, estados de vías) se pueden clasificar igual, subiendo carpetas de fotos en lugar de usar la cámara.
- Usa siempre fotos que el modelo no vio para probarlo, y anota en tu ficha .md cuántas acertó.
- El modelo se puede exportar desde el botón **Exportar modelo**.
