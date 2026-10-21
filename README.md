[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=23212806-debug/MSFP2)
# Práctica 2: Modelado y control del sistema cardiovascular mediante el modelo Windkessel

## Información del estudiante

Pedro Damian Martinez Lozano \ 23212806 ; 23212806@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo ; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México.

## Descripción de la práctica

El modelado del sistema cardiovascular es una herramienta importante en Ingeniería Biomédica, ya que permite comprender el comportamiento de la circulación sanguínea mediante representaciones matemáticas y circuitos eléctricos equivalentes. Estos modelos ayudan a analizar cómo interactúan la presión arterial, el flujo sanguíneo y las propiedades mecánicas de los vasos sanguíneos, así como los cambios que se presentan bajo diferentes condiciones fisiológicas.

En esta práctica se utiliza el **modelo Windkessel de cuatro elementos**, el cual representa el comportamiento dinámico del sistema arterial mediante una impedancia característica (Z), una resistencia periférica (R), una distensibilidad arterial (C) y una inertancia (L). Cada uno de estos elementos permite describir una propiedad del sistema cardiovascular y establecer una relación entre su funcionamiento fisiológico y el comportamiento de un circuito eléctrico.

A partir de este modelo se estudian tres condiciones cardiovasculares: **hipotensión, normotensión e hipertensión**, modificando la distensibilidad arterial para observar su influencia sobre la respuesta de presión. La condición normotensa se utiliza como referencia para identificar y comparar las diferencias en el comportamiento de los otros dos casos.

Para desarrollar el análisis se emplean herramientas computacionales como **MATLAB y Simulink**, mediante las cuales se formulan las ecuaciones diferenciales del sistema, se obtienen las funciones de transferencia y se realizan simulaciones que permiten visualizar las respuestas de los modelos. También se estudian características como la estabilidad, el comportamiento transitorio y el error en estado estacionario.

Finalmente, la práctica contempla el diseño e implementación de **controladores PID**, con el propósito de reducir las diferencias entre las respuestas de los modelos hipotenso e hipertenso respecto a la condición normotensa. De esta manera, se integran conocimientos de fisiología cardiovascular, circuitos eléctricos, modelado matemático y teoría de control para comprender cómo estas herramientas pueden utilizarse en el análisis y la simulación de sistemas fisiológicos.

## Objetivos

1. Comprender el funcionamiento del modelo Windkessel de cuatro elementos y su relación con el sistema cardiovascular.
2. Formular las ecuaciones diferenciales y obtener la representación matemática del sistema.
3. Determinar las funciones de transferencia para las condiciones hipotensa, normotensa e hipertensa.
4. Simular y comparar las respuestas cardiovasculares mediante MATLAB y Simulink.
5. Analizar el comportamiento dinámico y la estabilidad de los modelos.
6. Diseñar y evaluar controladores PID para reducir el error respecto a la respuesta normotensa.

## Descripción del sistema

El modelo Windkessel de cuatro elementos representa las principales propiedades hemodinámicas del sistema arterial mediante un circuito eléctrico equivalente.

Sus componentes son:

- **Z:** Impedancia característica de la región proximal del sistema arterial.
- **L:** Inertancia asociada al movimiento y aceleración de la sangre.
- **R:** Resistencia periférica al flujo sanguíneo.
- **C:** Distensibilidad arterial, que representa la capacidad de las arterias para almacenar volumen sanguíneo.

Para comparar las tres condiciones cardiovasculares se modifica únicamente el valor de la distensibilidad arterial (C), manteniendo constantes los demás parámetros.

| Parámetro | Hipotenso | Normotenso | Hipertenso |
|---|---|---|---|
| Z | 0.01  | 0.01  | 0.010 |
| L | 0.01  | 1.000 | 1.000 |
| R | 1.000 | 0.001 | 0.001 |
| C | 0.001 | 1.500 | 1.000 |

Una mayor distensibilidad permite amortiguar las variaciones de presión, mientras que una menor distensibilidad produce respuestas de presión más pronunciadas.

El modelo normotenso se utiliza como referencia para evaluar las diferencias entre las tres condiciones.

**Palabras clave:** Modelo Windkessel; Sistema cardiovascular; Presión arterial; Circuito RLC; MATLAB/Simulink; Control PID.

## Archivos del repositorio

1. Cuaderno computacional de MATLAB [.mlx y .pdf].
2. Modelo de Simulink [.slx].
3. Archivo de Python [.py].
4. Imágenes con los parámetros de los controladores PID (2).
5. Figuras de las simulaciones en Python (3) y MATLAB (4) [.pdf].
6. Archivo con la señal de entrada [.xlsx].
7. Desarrollo del análisis matemático [.pdf].
8. Diagrama biológico elaborado en BioRender [.jpeg].
9. Archivos README.md, CITATION.cff y LICENSE.

## Referencias

[1] P. A. Valle, *Syllabus para Modelado de Sistemas Fisiológicos*, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2026. https://biomath.xyz/course/

[2] M. C. Khoo, *Physiological Control Systems: Analysis, Simulation, and Estimation*, 2nd ed., IEEE Press, 2018.

[3] J. E. Hall, *Guyton and Hall Textbook of Medical Physiology*, 14th ed., Elsevier, 2021.

[4] N. S. Nise, *Control Systems Engineering*, 8th ed., John Wiley & Sons, 2020.
