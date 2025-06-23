# Sistema de Monitoreo y Riego Automático con ESP32

Se propone el desarrollo de un sistema automatizado basado en el microcontrolador ESP32 y programado en MicroPython, diseñado para monitorear variables ambientales clave como la humedad del suelo, la temperatura y la luminosidad. El sistema no solo toma decisiones de riego de forma autónoma, sino que también presenta los datos recolectados a través de una interfaz web local accesible desde cualquier dispositivo conectado a la misma red Wi-Fi.

## Descripción general

Este sistema está orientado a facilitar el mantenimiento de huertas caseras mediante la automatización del riego, basándose en condiciones ambientales reales. A través de sensores específicos, se recopilan datos sobre humedad del suelo, temperatura ambiental y nivel de luz, que luego son procesados por el ESP32 para determinar cuándo activar el sistema de riego.

El microcontrolador actúa tanto como unidad de control como servidor web, alojando una interfaz ligera que permite visualizar en tiempo real el estado del entorno y el funcionamiento del sistema. Esta solución combina principios de electrónica aplicada, programación embebida y diseño web, con el fin de ofrecer una alternativa práctica, escalable y de bajo costo para el riego inteligente en entornos urbanos o domésticos.

## Objetivos

### Objetivo general
Diseñar e implementar un sistema automatizado de monitoreo y riego inteligente para huertas caseras, utilizando un ESP32 como plataforma principal y una interfaz web de visualización local.

### Objetivos específicos
- Integrar sensores ambientales (humedad del suelo, temperatura y luminosidad) al microcontrolador ESP32.
- Programar una lógica de control en MicroPython para la toma de decisiones en tiempo real.
- Desarrollar una interfaz web alojada localmente para el monitoreo continuo del sistema.
- Validar el funcionamiento del sistema mediante pruebas en un entorno controlado.

## Componentes a utilizar

### Hardware
- Placa de desarrollo ESP32
- Sensor de humedad del suelo (capacitivo o resistivo)
- Sensor de temperatura y humedad (DHT11 o DHT22)
- Sensor de luz (LDR o BH1750)
- Módulo de relé de 1 canal
- Bomba de agua o válvula solenoide
- Protoboard y cableado
- Fuente de alimentación (dependiendo del actuador: 5V o 12V)

### Software
- MicroPython (firmware del ESP32)
- Thonny IDE o uPyCraft (entorno de desarrollo)
- HTML, CSS y JavaScript (interfaz web)
- Servidor web embebido en el ESP32

## Diseño del producto

El sistema se divide en tres módulos funcionales:

### 1. Adquisición de datos
Los sensores conectados al ESP32 realizan lecturas periódicas de las variables ambientales. Los valores obtenidos son procesados para su análisis y posterior visualización.

### 2. Lógica de control y toma de decisiones
Mediante programación en MicroPython, se establece una lógica de control que determina cuándo activar el sistema de riego. Si la humedad del suelo está por debajo de un umbral definido, se activa el actuador (bomba o válvula) durante un intervalo de tiempo preestablecido. Esta lógica puede extenderse para considerar también la temperatura y luminosidad, si se desea optimizar aún más el uso del agua.

### 3. Visualización mediante interfaz web
La ESP32 aloja un servidor web simple que presenta una interfaz gráfica donde el usuario puede:
- Visualizar en tiempo real los valores de los sensores.
- Conocer el estado actual del sistema de riego.
- Activar manualmente el riego desde la interfaz (opcional).

Esta interfaz es accesible desde cualquier dispositivo conectado a la misma red local, sin necesidad de aplicaciones externas ni conexión a Internet.

---

## Autores
- Ian Nicolás Bolívar Fonseca  
- Miller Esteban Bohorquez Novoa  
- Andrés Camilo Guana Cadena
