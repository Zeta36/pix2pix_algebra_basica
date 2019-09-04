##### Copyright 2019 Samuel Graván (https://github.com/Zeta36).

Licensed under the Apache License, Version 2.0 (the "License");

##### Scope del proyecto

El siguiente proyecto ha sido desarrollado para participar en el reto creado por Dot CSV (https://www.youtube.com/watch?v=BNgAaCK920E): "¡Gana una NVidia RTX 2080 SUPER con el Reto DotCSV!" 

En concreto, se ha hecho uso de la tecnología Pix2Pix para desarrollar un modelo capaz de "ver" una imagen con una expresión algebraica sencilla; por ejemplo: 5 - 2, y que sea capaz de generar otra imagen donde se imprima la respuesta. En el caso de ejemplo, una imagen con el número "3"

##### Otra información de interés

Este modelo no utiliza un dataset estático, sino que en cada iteración de entrenamiento genera una expresión algebraica aleatoria (que posteriormente se transforma en una imagen). Para conseguir dataset de pruebas (test) con expresiones no vistas durante el entrenamiento, se restringe la generación de estas expresiones para que no generen entradas con ciertos valores concretos.

El modelo es funcional y parece que generaliza bien a expresiones no vistas durante el entrenamiento.

También sería fácil ampliar este desarrollo añadiendo nuevos tipos de letras, fuentes, tamaños, orientaciones, ruido, etc., de modo que el modelo pudiese realmente computar estas expresiones algebraicas sencillas simplemente tras un "vistazo" a una imagen de entrada que incluya una expresión matemática de este estilo. 
