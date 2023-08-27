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

Los tipos de termocuplas se identifican con nombres basados en letras y sus diferencias se caracterizan especialmente en sus rangos de operación y sensibilidad a los cambios que presentan.
Se cuenta con termocuplas:
- Tipo B: Requiere protección contra contaminación. Rango aproximado de $[0,1700] °C$ con un máximo de tensión de $13.814 mV$. 
- Tipo C: No cuenta con protección contra oxidación. Soporta hasta $2315 °C$ con uso en vacío.
- Tipo E: Se trata del tipo con mayor rango de tensión por temperatura, con rango aproximado a $900 °C$ y una tensión máxima de $80 mV$.
- Tipo J: Compuesto de hierro y con rango de operación de $[-180,750] °C$ y tensión máxima de $42.2 mV$.
- Tipo K: Basado en niquel-aluminio y con rango de operación de $[-180,1372] °C$ y tensión máxima de $54.8 mV$. 
- Tipo N: Para uso general, basado en niquel y buen funcionamiento a altas temperaturas, cuenta con rango hasta $1260 °C$.
- Tipo R: Basado en platino y rango de operación de $[0,1760] °C$ aproximado. Además, tensión máxima de $21.09 mV$.
- Tipo S: También basado en platino, se trata del estandar de laboratorio con rango de $[0,1760] °C$ y tensión máxima de $18.68 mV$.
- Tipo T: Compuesto de cobre, rango de $[-250,400] °C$ y tensión máxima $20.8 mV$.
A manera de resumen de algunos de estos tipos de termocuplas, se siguiente figura.

<img src="/images/termocupla.PNG" alt="Gráfico de tensión eléctrica contra temperatura de termocuplas" style="width:25%;" />

### 3. ¿Qué es una señal balanceada y una no balanceada? ¿Qué aplicación tiene el uso de señales balanceadas?

Una *señal balanceada* se trata de una señal que es transmitida de manera simétrica por medio de dos conductores (cable balanceado) en donde la copia es enviada en contrafase o invertida, lo cual permite que una interferencia o ruido captado por la señal sea cancelado al llegar al destino y reinvertir la copia de la señal y sumarlas, obteniendo el doble del mensaje original recuperado.

**Aplicación:** Su aplicación sobresale en los casos de transferencia de señales a largas distancias o ambientes complicados (ruido/interferencia), donde el objetivo es la calidad de la señal. Así, se encuentran casos como las comunicaciones, instrumentación delicada (mediciones), audio profesional, entre otras.

<img src="/images/senal_balanceada.png" alt="Ejemplo de presencia de interferencia en señal balanceada" style="width:35%;" />

Una *señal no balanceada* se trata de una mensaje enviado de manera más simple, ya que solo se cuenta con un medio vivo y referencia (tierra), de manera que dicho conductor de referencia protege con mallado la línea con el mensaje. Dichas señales suelen verse en conexiones de instrumentos musicales o equipos de buen desempeño.

### 4. ¿Qué es el aislamiento eléctrico entre dos tierras? ¿En los diseños electrónicos que ventajas tiene el aislamiento entre señales?

RESPUESTA

### 5. Investigue diseños electrónicos para aislar eléctricamente señales DC o de baja frecuencia (<100Hz).

RESPUESTA

### 6. Investigue diseños de amplificadores con ganancia programable.

RESPUESTA

### 7. Investigue como se mide el rechazo de modo común para una señal diferencial, y el rechazo de crosstalk entre dos canales.

Para medir el **CMR** o **CMRR** de una señal diferencial primero se debe medir la ganancia diferencial ($A_d$) de manera que se logre apreciar la diferencia entre los das dos entradas al dispositivo.

Luego se tiene la ganancia de modo común ($A_c$), la cual afecta directamente a las tensiones continuas que se encuentren en la entrada del dispositivo.

FALTA ...

## Referencias
- Problema 2
- https://www.emb.cl/electroindustria/articulo.mvc?xid=1502&ni=termocuplas-fundamentos-y-recomendaciones
- https://catedra.ing.unlp.edu.ar/electrotecnia/cys//DI/termocuplas.pdf
- https://www.watlow.com/resources-and-support/engineering-tools/reference-data/thermocouple-types
- Problema 3
- http://telcoavi.es/blog/senal-balanceada-vs-senal-no-balanceada/
- https://www.thomann.de/blog/es/cable-balanceado-y-no-balanceado-en-que-se-diferencian/
- Problema 4
- a
- a
- a
- a
- a
- a
- 
- a
- a



# Lo copié de por ahí para tenerlo de referencia y ver como se hacen algunas cosas...

- Method 3 uses the FFT to analyse for a fundamental frequency. It assumes that the input is a sinusoidal signal, the system adds noise and can contain weak non-linearities.
- Methos 4 is here mostly for reference and is mostly suited for DC signals (not audio signals)

## Basic Definition
A discrete time signal, $x_s(n)$ exists. Through some process, noise $x_n(n)$ and harmonics of $x$ are added, resulting in a new signal, $y(n)$ that therefore contains noise and distortion.

The main idea is to make a *ratio* between signal power to noise power. 


$$ SNR = \frac{P_{signal}}{P_{noise}} $$

So we need to measure the *power* $P(x)$ of a signal $x(n)$,  via:

$$P(x)=1/N \cdot \displaystyle\sum_{n=0}^{N-1}x(n)^2$$

## Prueba de insertar imagen 1

![Descripción de la imagen](/images/perro.jpeg "Leyenda de la imagen")

## Prueba de insertar imagen 2

<img src="/images/perro.jpeg" alt="Descripción de la imagen" style="width:25%;" />


