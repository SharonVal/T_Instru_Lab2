## Instituto Tecnológico de Costa Rica

## Escuela de Ingeniería Electrónica
### Taller de Instrumentación

# Investigación Previa Lab. 2 (Parte I)

### Integrantes:
- Oscar Andrés Rojas Fonseca
- Sharon Valverde Jiménez
- Sebastián Vega Cerdas 

### Profesor:
MSc. Ing. Kaleb Alfaro Badilla


# Investigación Previa
## Laboratorio 2 (Parte I)

### 1. ¿Cuales son los tipos de sensores de temperatura más populares? ¿Cuáles son sus ventajas y desventajas en función de los requisitos del diseño?

RESPUESTA

### 2. ¿Cuales son los tipos de termocuplas? ¿Cuales son sus rangos de temperatura y tensión?

RESPUESTA

### 3. ¿Qué es una señal balanceada y una no balanceada? ¿Qué aplicación tiene el uso de señales balanceadas?

RESPUESTA

### 4. ¿Qué es el aislamiento eléctrico entre dos tierras? ¿En los diseños electrónicos que ventajas tiene el aislamiento entre señales?

RESPUESTA

### 5. Investigue diseños electrónicos para aislar eléctricamente señales DC o de baja frecuencia (<100Hz).

RESPUESTA

### 6. Investigue diseños de amplificadores con ganancia programable.

RESPUESTA

### 7. Investigue como se mide el rechazo de modo común para una señal diferencial, y el rechazo de crosstalk entre dos canales.

RESPUESTA




# Lo copié de por ahí para tenerlo de referencia y ver como se hacen algunas cosas...

- Method 3 uses the FFT to analyse for a fundamental frequency. It assumes that the input is a sinusoidal signal, the system adds noise and can contain weak non-linearities.
- Methos 4 is here mostly for reference and is mostly suited for DC signals (not audio signals)

## Basic Definition
A discrete time signal, $x_s(n)$ exists. Through some process, noise $x_n(n)$ and harmonics of $x$ are added, resulting in a new signal, $y(n)$ that therefore contains noise and distortion.

The main idea is to make a *ratio* between signal power to noise power. 


$$ SNR = \frac{P_{signal}}{P_{noise}} $$

So we need to measure the *power* $P(x)$ of a signal $x(n)$,  via:

$$P(x)=1/N \cdot \displaystyle\sum_{n=0}^{N-1}x(n)^2$$

## Prueba de insertar imagen

![Descripción de la imagen](/images/perro.jpeg "Leyenda de la imagen")



