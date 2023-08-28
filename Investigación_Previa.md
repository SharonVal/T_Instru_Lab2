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

- Resistencias térmicas: Son sensores que se basan en el cambio de resistencia eléctrica de un material conductor o semiconductor cuando varía su temperatura.
        Ventajas: Miden entre -200°C y 850°C, son precisos, lineales y estables.
        Desventajas: Tienen un alto costo, un tiempo de respuesta lento y son sensibles a las interferencias electromagnéticas.

- Sensores infrarrojos: Son sensores que se basan en la detección de la radiación infrarroja emitida por un cuerpo u objeto debido a su temperatura.
        Ventajas: No necesitan contacto con el objeto a medir, tienen una alta velocidad de respuesta y una buena precisión.
        Desventajas: Tienen un alto costo, son sensibles a las condiciones ambientales y requieren de una calibración periódica

- Termopares: Son sensores que se basan en el efecto Seebeck, que consiste en la generación de una diferencia de potencial eléctrico entre dos metales diferentes unidos en un extremo cuando se someten a una diferencia de temperatura.
        Ventajas: Son económicos, de fácil instalación y con un amplio rango de medición. Miden desde -200°C hasta 1800°C, dependiendo del tipo de termopar.
        Desventajas: Tienen una baja precisión, una mala linealidad y requieren de un dispositivo de referencia para compensar la temperatura ambiente.

- Termistores: Son sensores que se basan en el cambio de resistencia eléctrica de un material semiconductor cuando varía su temperatura.
        Ventajas: Son muy sensibles, con un tiempo de respuesta rápido y un bajo costo.
        Desventajas: Tienen una baja linealidad, una alta dependencia del voltaje y un rango de medición limitado, que suele estar entre los -50°C y los 150°C.


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
<p align="center">
<img src="/images/termocupla.PNG" alt="Gráfico de tensión eléctrica contra temperatura de termocuplas" style="width:25%;" />
</p>
### 3. ¿Qué es una señal balanceada y una no balanceada? ¿Qué aplicación tiene el uso de señales balanceadas?

Una *señal balanceada* se trata de una señal que es transmitida de manera simétrica por medio de dos conductores (cable balanceado) en donde la copia es enviada en contrafase o invertida, lo cual permite que una interferencia o ruido captado por la señal sea cancelado al llegar al destino y reinvertir la copia de la señal y sumarlas, obteniendo el doble del mensaje original recuperado.

**Aplicación:** Su aplicación sobresale en los casos de transferencia de señales a largas distancias o ambientes complicados (ruido/interferencia), donde el objetivo es la calidad de la señal. Así, se encuentran casos como las comunicaciones, instrumentación delicada (mediciones), audio profesional, entre otras.
<p align="center">
<img src="/images/senal_balanceada.png" alt="Ejemplo de presencia de interferencia en señal balanceada" style="width:35%;" />
</p>
Una *señal no balanceada* se trata de una mensaje enviado de manera más simple, ya que solo se cuenta con un medio vivo y referencia (tierra), de manera que dicho conductor de referencia protege con mallado la línea con el mensaje. Dichas señales suelen verse en conexiones de instrumentos musicales o equipos de buen desempeño.

### 4. ¿Qué es el aislamiento eléctrico entre dos tierras? ¿En los diseños electrónicos que ventajas tiene el aislamiento entre señales?

El aislamiento eléctrico entre dos tierras se refiere a la capacidad de impedir el paso de corriente eléctrica entre dos puntos que están en potenciales eléctricos diferentes, es decir, en tierras distintas. Para lograr el aislamiento eléctrico entre dos tierras se puede emplear materiales aislantes en forma de recubrimiento o separación entre los conductores que están en contacto con la tierra.

La ventaja que tiene el aislamiento entre señales es que previene que se produzcan cortocircuitos, inteferencias electromagnéticas o daños en el equipo.


### 5. Investigue diseños electrónicos para aislar eléctricamente señales DC o de baja frecuencia (<100Hz).

RESPUESTA

### 6. Investigue diseños de amplificadores con ganancia programable.

1. Amplificador operacional con divisor resistivo.

<p align="center">
  <img src="/images/ganancia_potenciometro" alt="Circuito con amplificador operacional y potenciómetro" style="width:30%;" />
</p>

2. 

### 7. Investigue como se mide el rechazo de modo común para una señal diferencial, y el rechazo de crosstalk entre dos canales.

Para medir el **CMR** o **CMRR** de una señal diferencial primero se debe medir la ganancia diferencial ($A_d$) de manera que se logre apreciar la diferencia entre los das dos entradas al dispositivo.

Luego se tiene la ganancia de modo común ($A_c$), la cual afecta directamente a las tensiones continuas que se encuentren en la entrada del dispositivo. Así, se calcula el valor del CMRR en decibeles con la siguiente fórmula:

$$CMRR = 20\cdot log \left(\frac{A_d}{A_c}\right)$$

Para realizar estas mediciones se puede utilizar el método de resistencias de precisión, como se observa en la figura, donde se aplica una señal a las entradas y se mide su diferencia con la salida, en este punto una variación del $0.1\%$ corresponde en CMR a aproximadamente $66$ $dB$.
<p align="center">
  <img src="/images/CMRR_resistencias.PNG" alt="Circuito de medición para CMRR con resistencias de presición" style="width:30%;" />
</p>


Otro método se realiza al aplicarle diferentes tensiones conmutadas a un circuito un mayor cantidad de componentes, entre esos un amplificador extra que este bien definido en sus características, entre las cuales se encuentra una alta ganancia. Ejemplo en la figura siguiente.
<p align="center">
<img src="/images/CMRR_conmutadas.PNG" alt="Circuito de medición para CMRR con conmutación de fuentes" style="width:35%;" />
</p>
La medición del **rechazo de crosstalk** se mide al obtener la relación señal a crosstalk, donde la señal se mide de manera directa, pero el crosstalk se mide al aplicar un tono a una entrada y medir la salida del otro canal, permitiendo observar el crosstalk resultante. En la siguiente ilustración se muestra un diagrama de ejemplo con capacitores modelando el crosstalk.
<p align="center">
<img src="/images/crosstalk.PNG" alt="Circuito de medición para crosstalk" style="width:35%;" />
</p>
De esta manera, se aplica la fórmula de relación señal a crosstalk en decibeles:

$$SCT = 10\cdot log \left(\frac{P_{señal}}{P_{crosstalk}}\right)$$


## Referencias
- Problema 1
- https://pirometriatecnica.com/sensores-de-temperatura-tipos-caracteristicas-y-aplicaciones/
- https://srcsl.com/tipos-sensores-temperatura/
- https://guide.directindustry.com/es/que-sensor-de-temperatura-elegir/
- Problema 2
- https://www.emb.cl/electroindustria/articulo.mvc?xid=1502&ni=termocuplas-fundamentos-y-recomendaciones
- https://catedra.ing.unlp.edu.ar/electrotecnia/cys//DI/termocuplas.pdf
- https://www.watlow.com/resources-and-support/engineering-tools/reference-data/thermocouple-types
- Problema 3
- http://telcoavi.es/blog/senal-balanceada-vs-senal-no-balanceada/
- https://www.thomann.de/blog/es/cable-balanceado-y-no-balanceado-en-que-se-diferencian/
- a
- a
- a
- a
- a
- a
- a
- Problema 7
- https://electrositio.com/relacion-de-rechazo-en-modo-comun-cmrr-y-el-amplificador-operacional/
- https://www.tsc.uc3m.es/~fran/docencia/SyCT/Tema6_sesion1.pdf
- https://www.youtube.com/watch?v=Cv5zNkC4-ao




# Lo copié de por ahí para tenerlo de referencia y ver como se hacen algunas cosas...
AAAAAAAAAAAAA
$$P(x)=1/N \cdot \displaystyle\sum_{n=0}^{N-1}x(n)^2$$




