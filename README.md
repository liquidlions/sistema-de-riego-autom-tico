# sistema-de-riego-autom-tico
 Se propone el desarrollo de un sistema automatizado basado en el microcontrolador ESP32 y programado en MicroPython, el cual permitirá monitorear variables ambientales clave como la humedad del suelo, la temperatura y la luz. Este sistema activará de forma automática el riego de una huerta casera.
 
# Sistema de Monitoreo y Riego Automático con ESP32

Este proyecto consiste en el desarrollo de un sistema automatizado basado en el microcontrolador ESP32 y programado en MicroPython, que permite monitorear variables ambientales clave como la humedad del suelo, la temperatura y la luz. El sistema activa automáticamente el riego de una huerta casera y muestra los datos recolectados en una interfaz web local accesible desde cualquier dispositivo conectado a la misma red.

## Descripción completa

Este sistema busca facilitar el cuidado de huertas caseras mediante la automatización del riego basado en condiciones ambientales reales. Utiliza sensores para medir la humedad del suelo, la temperatura y la luminosidad, y toma decisiones sobre el riego en base a estos datos. El ESP32 funciona como el núcleo del sistema, encargándose tanto del control como de la visualización de los datos vía web local.

La interfaz web permite visualizar el estado de la huerta en tiempo real y conocer cuándo se activa el riego, promoviendo un uso eficiente del agua y facilitando el monitoreo sin necesidad de intervención constante. Este proyecto combina electrónica básica, lógica de control automatizado y desarrollo web embebido para ofrecer una solución accesible y práctica de agricultura urbana.

## Objetivos

### Objetivo general

Diseñar e implementar un sistema automatizado de monitoreo y riego inteligente para huertas caseras, utilizando sensores ambientales conectados a un microcontrolador ESP32 y una interfaz web local.

### Objetivos específicos

- Integrar sensores de humedad del suelo, temperatura y luz al ESP32.
- Programar la lógica de riego automático en MicroPython.
- Desarrollar una interfaz web local accesible desde la red Wi-Fi.
- Probar el sistema en un entorno de huerta casera simulado.

## 🔧 Componentes a utilizar

### Hardware

- ESP32
- Sensor de humedad del suelo (capacitivo o resistivo)
- Sensor de temperatura y humedad (DHT11 o DHT22)
- Sensor de luz (LDR o BH1750)
- Módulo de relé de 1 canal
- Bomba de agua o válvula solenoide
- Protoboard y cables
- Fuente de alimentación (5V o 12V según el actuador)

### Software

- MicroPython
- Thonny IDE o uPyCraft
- HTML/CSS/JavaScript para la interfaz web
- Servidor web embebido en ESP32

## Diseño del producto

### 1. Adquisición de datos

Los sensores leen periódicamente valores de humedad, temperatura y luz. Estas lecturas se obtienen mediante los pines analógicos/digitales del ESP32.

### 2. Toma de decisiones

Se programa una lógica de control que activa el riego cuando la humedad del suelo está por debajo de un umbral predefinido. El riego se mantiene activo durante un tiempo corto y luego se apaga automáticamente.

### 3. Visualización web

El ESP32 aloja un servidor web básico accesible desde la red local. En esta interfaz se muestran los valores actuales de los sensores y el estado del riego. Se puede incluir un botón para activación manual del riego como función adicional.

---

*Autores:*  
Ian Nicolás Bolívar Fonseca  
Miller Esteban Bohorquez Novoa  
Andrés Camilo Guana Cadena
