<h1 align="center">Universidad Nacional de Lomas de Zamora - Facultad de Ingeniería</h1>

![Logo Institucional](https://github.com/JonatanBogadoUNLZ/PPS-Jonatan-Bogado/blob/9952aac097aca83a1aadfc26679fc7ec57369d82/LOGO%20AZUL%20HORIZONTAL%20-%20fondo%20transparente.png)


<h1 align="center">HoverRobot ESP32</h1>


![Prueba de balanceo](Multimedia/robot_path.gif)

## Introducción / Objetivo

La **Facultad de Ingeniería de la Universidad Nacional de Lomas de Zamora** impulsa proyectos orientados a la robótica, control y automatización.  
Este repositorio corresponde al **Proyecto Final de Ingeniería Mecatrónica**, cuyo desarrollo se centra en un robot de balanceo autónomo, denominado **HoverRobot ESP32**.

El objetivo principal es **diseñar, modificar e integrar la estructura de un hoverboard como plataforma de locomoción**, incorporando:

- Un **sistema de control dinámico** basado en un **ESP32**.  
- Un **sensor inercial** para el equilibrio del robot.  
- Un módulo de **visión artificial con cámara estéreo PS5 y Raspberry Pi 5**.  
- Una **aplicación móvil** para control manual.  

El proyecto busca explorar la interacción entre **control de estabilidad**, **procesamiento visual en tiempo real**, y **navegación autónoma** mediante ROS 2.


## Índice

- [Descripción](#descripción)  
- [Instrucciones de Uso](#instrucciones-de-uso)  
- [Tecnologías Utilizadas](#tecnologías-utilizadas)  
- [Listado de Componentes](#listado-de-componentes)  
- [Esquemáticos](#esquemáticos)  
- [Fotos / Videos](#fotos--videos)  
- [Autor](#autor)  
- [Repositorios Relacionados](#repositorios-relacionados)  

## Descripción

HoverRobot ESP32 es un **robot autoequilibrado** basado en la electrónica de potencia de un hoverboard.  

El sistema utiliza:

- Una **placa ESP32 personalizada** para ejecutar el control de balanceo.  
- Un **IMU MPU6050**, encargado de medir aceleraciones y velocidades angulares del chasis.  
- Los **motores brushless originales** del hoverboard, controlados mediante el firmware reprogramado de su controladora.  
- Un módulo de visión artificial compuesto por una **cámara estéreo PS5** y una **Raspberry Pi 5**, desde donde se ejecutan los nodos de **ROS 2** encargados de navegación y procesamiento de imágenes.

Además, el robot cuenta con:

- **Una aplicación móvil** desarrollada en **Kotlin** para operar el robot manualmente.  
- **Comunicación TCP** entre la Raspberry Pi, la app y la placa principal ESP32.  

El proyecto integra áreas clave de la mecatrónica: **electrónica**, **control**, **procesamiento visual**, **automatización** y **robótica móvil**.


## Instrucciones de Uso

1. Clonar este repositorio general y los repositorios relacionados.  
2. Montar el hardware de acuerdo a los planos en la carpeta `PLANOS`.  
3. Cargar el firmware del ESP32 desde el repositorio [Mainboard](https://github.com/patoGarces/HoverRobot-ESP32).  
4. Instalar y ejecutar la aplicación móvil desde [HoverRobotApp](https://github.com/patoGarces/HoverRobotApp-balancing-robot/).  
5. Ejecutar el stack de navegación en ROS 2 desde [HoverRobotNavigation](https://github.com/patoGarces/HoverRobotNavigation).  
6. Realizar pruebas en entorno controlado y luego en entornos reales.  

---

## Tecnologías Utilizadas

- **Control y Robótica**: ESP32, controladora hoverboard, motores brushless  
- **Sensado**: IMU MPU6050, cámara estéreo PS5  
- **Computación / Procesamiento**: Raspberry Pi 5, Python, C, Kotlin  
- **Frameworks**: ROS 2 (Jazzy), OpenCV  
- **Comunicación**: TCP sockets, UART  
- **Visión Artificial**: extracción de características, flujo estéreo, navegación basada en percepción  

---

## Listado de Componentes  

- **Placa ESP32 custom** – microcontrolador principal  
- **IMU MPU6050** – medición de aceleración y giroscopio para balanceo  
- **Motores brushless** – tracción principal, controlados mediante la controladora original del hoverboard  
- **Cámara estéreo PS5** – captura del entorno para visión artificial  
- **Raspberry Pi 5** – procesamiento de visión y ejecución de ROS 2  

---

## Esquemáticos

📌 Pendiente de agregar. 

---

## Fotos / Videos

En carpeta 'Multimedia'

---

## Autor

Proyecto realizado por **Patricio Garcés** como Trabajo Final de la carrera **Ingeniería Mecatrónica**,  
Facultad de Ingeniería – Universidad Nacional de Lomas de Zamora.

---


## Repositorios Relacionados  

- **Mainboard (ESP32)** → [HoverRobot-ESP32](https://github.com/patoGarces/HoverRobot-ESP32)  
- **Aplicación móvil (Kotlin)** → [HoverRobotApp-balancing-robot](https://github.com/patoGarces/HoverRobotApp-balancing-robot/)  
- **Navegación en ROS 2** → [HoverRobotNavigation](https://github.com/patoGarces/HoverRobotNavigation)
- **Firmware de la controladora (fork modificado)** → [hoverrobot-firmware-hack-FOC](https://github.com/patoGarces/hoverrobot-firmware-hack-FOC) 
