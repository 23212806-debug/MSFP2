
# Práctica 2: Modelado y control del sistema cardiovascular mediante el modelo Windkessel

## Información del estudiante

**Nombre:** Martínez Lozano Pedro Damián  
**Número de control:** 23212806  
**Correo institucional:** 23212806@tectijuana.edu.mx  
**Asignatura:** Modelado de Sistemas Fisiológicos  
**Carrera:** Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo  
paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México.

## Descripción de la práctica

El modelado del sistema cardiovascular permite estudiar el comportamiento de la presión arterial y del flujo sanguíneo mediante modelos matemáticos basados en circuitos eléctricos equivalentes.

En esta práctica se utiliza el modelo Windkessel de cuatro elementos para representar la dinámica del sistema arterial y comparar tres condiciones cardiovasculares: hipotensión, normotensión e hipertensión. A través de MATLAB y Simulink se analiza cómo las variaciones en la distensibilidad arterial modifican la respuesta del sistema.

Además, se plantea el uso de controladores PID para reducir las diferencias entre las respuestas de los modelos hipotenso e hipertenso respecto al modelo normotenso, utilizado como referencia.

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
| Z | 0.010 | 0.010 | 0.010 |
| L | 0.001 | 0.001 | 0.001 |
| R | 1.000 | 1.000 | 1.000 |
| C | 3.500 | 1.500 | 1.000 |

Una mayor distensibilidad permite amortiguar las variaciones de presión, mientras que una menor distensibilidad produce respuestas de presión más pronunciadas.

El modelo normotenso se utiliza como referencia para evaluar las diferencias entre las tres condiciones.

**Palabras clave:** Modelo Windkessel; Sistema cardiovascular; Presión arterial; Circuito RLC; MATLAB/Simulink; Control PID.

## Archivos del repositorio

1. Cuaderno computacional de MATLAB (`.mlx`).
2. Modelo de simulación en Simulink (`.slx`).
3. Funciones utilizadas para resolver las ecuaciones diferenciales.
4. Gráficas de las respuestas cardiovasculares.
5. Resultados de las simulaciones para los tres casos.
6. Archivos complementarios de análisis y control, según su implementación.

## Referencias

[1] P. A. Valle, *Syllabus para Modelado de Sistemas Fisiológicos*, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2026. https://biomath.xyz/course/

[2] M. C. Khoo, *Physiological Control Systems: Analysis, Simulation, and Estimation*, 2nd ed., IEEE Press, 2018.

[3] J. E. Hall, *Guyton and Hall Textbook of Medical Physiology*, 14th ed., Elsevier, 2021.

[4] N. S. Nise, *Control Systems Engineering*, 8th ed., John Wiley & Sons, 2020.
