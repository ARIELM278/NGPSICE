#Trabajo Extra  NGSPICE


<div align="center">

# UNIVERSIDAD DE LAS FUERZAS ARMADAS ESPE

AUTORES

Ariel Santiago Munoz Pallo

NRC
  
5412

INGENIERO

Ing. Darwin Omar Alulema Flores

# PRÁCTICA CIRCUITO EN NGSPICE
  
</div>

# 1 OBJETIVOS

**1.1. OBJETIVO DE LA PRÁCTICA**

1.1.1. Objetivo general

En este caso tendremos la capacidad de entender como funciona un programa que nos ayudara a resolver circuitos sin necesidad de calcular. Obtendremos una mejor visualización de un circuito sin necesidad de graficar ya que este programa solo nos solicita nodo fuentes voltajes, etc en el mismo. Lograremos aprender un nuevo sistema de código para este programa y saber cuál implementarlo según nuestras necesidades.


1.1.2. Objetivos específicos

•	Aprender a descargarse el programa de una manera correcta.

•	Conocer las grandes posibilidades que se pueden usar por este medio.

•	Realización de un ejemplo con un circuito con 2 voltajes además ejecutarlo en el programa.

**1.2. REQUISITOS PREVIOS**

Investigue Sobre como descargar el Programa además visualizar videos para saber cual es su funcionalidad por medio de este link 

http://ngspice.sourceforge.net/download.html




**1.3. INFORMACIÓN GENERAL**

<div align="center">
  
**NGSPICE**


[![1.jpg](https://i.postimg.cc/6Qmj3rQK/1.jpg)](https://postimg.cc/8FLBXrWX)


</div>


# 2 MARCO TEÓRICO

<div align="center">
  


**2.1.¿Que es NGPSICE y cual es su funcionalidad?**
Ngspice (Next Generation Simulation Program with Integrated Circuits Emphasis ) es un programa para la simulación de circuitos electrónicos lineales y no lineales con propósito general.
Ngspice soporta una gran cantidad de elementos como resistencias, condensadores, bobinas, bobinas acopladas, fuentes de tensión y de corriente tanto independientes como independientes, líneas de transmisión con y sin pérdidas, interruptores controlados por tensión o por corriente.
Además, se pueden encapsular subcircuitos, y usar ecuaciones en los parámetros de los componentes, y usar estructuras de control, tales como while, dowhile, if, goto, etc, etc. y por si fuese poco, también se pueden añadir componentes escritos en Verilog.

Ngspice soporta las siguientes simulaciones:

•	Análisis en corriente continua
•	Análisis de pequeña señal en corriente alterna
•	Análisis temporal
•	Análisis de polos y ceros
•	Análisis de distorsión en pequeña señal
•	Análisis de ruidos

**2.2¿Qué se puede hacer en NGSPICE?**
ANÁLISIS EN TRANSITORIO Análisis temporal de variables de salida: Se pueden especificar distintas excitaciones: pulsos, exponenciales, sinusoidales, etc.
  Análisis de Fourier: Distintas componentes de Fourier de la salida para una entrada sinusoidal (.FOUR) ANÁLISIS A DIFERENTES TEMPERATURAS 
 Las resistencias y algunos parámetros de los dispositivos semiconductores varían con la temperatura (.TEMP) (por defecto es 27oC)

ANÁLISIS EN AC : Respuesta frecuencial en pequeña señal: Circuito linealizado alrededor del punto de trabajo y considerando entrada sinusoidal (.AC) 
  
 Análisis de ruido: Las fuentes de ruido se calculan automáticamente (.NOISE)
  
Análisis de distorsión: Se superponen en la entrada una o varias señales de distintas frecuencias (.DISTO)
  
  
**2.3¿Cómo cambiar el circuito de NGSPICE a sintaxis de texto block de nota?**


Para lograr cambiar es necesario ver como nuestro circuito esta formado ahora según la sintaxis de NGSPICE es necesario saber que el programa identifica según la primera inicial por ejemplo resistencia el programa espera que comienze con R asi sucesivamente.
  
[![8.jpg](https://i.postimg.cc/zX1F7J2T/8.jpg)](https://postimg.cc/4nBcNTg3)
  
  En la siguiente imagen podemos notar la sintaxis que usamos en el bloc de notas  para que el programa puede reconocer los comandos inicializado mediante un texto plano.
  
[![12.jpg](https://i.postimg.cc/CxCf3mNc/12.jpg)](https://postimg.cc/w1vvJ5nN)



</div>

# 3.0.0Interface de NGSPICE

[![2.jpg](https://i.postimg.cc/nrt6F4dz/2.jpg)](https://postimg.cc/9RJx17H5)


Han incorporado una capa de abstracción visual, donde los componentes se usan por su símbolo gráfico, ngspice se sigue usando en modo texto, y aunque esta característica pueda parecer una desventaja, lo cierto es que si se llega a dominar, ngspice puede llegar a ser la herramienta de simulación más potente de todas.

No obstante, tanto en aplicaciones privativas como en las interfases gráficas para ngspice, es casi seguro que tendremos que añadir manualmente alguna línea de spice, o editar los parámetros de algún componente, por lo que sea cual fuere la solución que se vaya a usar, siempre que esté basada en spice3f5, conviene saber cómo se escriben los archivos de nodos, y cuáles son sus principales directrices.



Además, adjuntamos algunos comandos mayormente utilizados por los usuarios al ejecutar el programa.

[![13.jpg](https://i.postimg.cc/d04Z13gd/13.jpg)](https://postimg.cc/rdRwZVVF)



  
</div>

# 4 EXPLICACIÓN DEL PROCEDIMIENTO

**4.5 PROCEDIMIENTO**

**4.5.1. Creación de Circuito en NGSPICE**

<div align="center">


Para comenzar descargamos nuestro programa de internet como zip y lo ejecutamos descargando los ficheros cen nuestra PC

[![3.jpg](https://i.postimg.cc/28kK08MP/3.jpg)](https://postimg.cc/w3r2vH6V)

Abrimos lo descargado y verificamos si se encuentra el archivo ejecutable ya que algunas descargas no es posible descargar aquello

[![4.jpg](https://i.postimg.cc/HLJMHKPp/4.jpg)](https://postimg.cc/mcskydsq)


Ahora sabiendo que nuestro programa si va a correr relizaremos un circuito con varias voltajes según lo que nosotros veamos convenientes además lo graficaremos el circuito usando alguna interfaz preferid  en preferido por que es necesario visualizar todas sus partes.

[![5.jpg](https://i.postimg.cc/dV3kmpF8/5.jpg)](https://postimg.cc/9D3QcxrM)


Hecho ya el circuito con los voltajes requeridos y necesarios para cumplir con su funcionalidad verificaremos sus parte es decir vamos a ver voltaje , nodos , corrientes , resistores,etc.

[![7.jpg](https://i.postimg.cc/D07mWY54/7.jpg)](https://postimg.cc/WFfsC8Bs)
  
  
Ahora abriremos el block de notas para poder hacer una sintaxis de nuestro circuito en modo texto para esto se necesita saber la información de arriba para saber cómo colocar el el block de notas.
Ahora se guardara tipo cir para que el programa lo pueda encontrar 


[![9.jpg](https://i.postimg.cc/nhbgvbBW/9.jpg)](https://postimg.cc/tYkBjcrd)



Ahora se guardara tipo cir para que el programa lo pueda encontrar 
Posteriormente abriremos nuestro programa y iniciaremos con source -------- (nomobre del Programa); y el codifo OP para poder ver si no cuenta con errores.

[![Whats-App-Image-2021-09-17-at-11-39-01-AM.jpg](https://i.postimg.cc/prN8TZ5g/Whats-App-Image-2021-09-17-at-11-39-01-AM.jpg)](https://postimg.cc/34BWf2BB)

  
Ahora podremos realizar mediante condigos ejercicios es decir vamos a comprobar primero con listing si nuestro circuito esta completo y luego usaremos print all para ver el resultados de los nodos 
  

[![11.jpg](https://i.postimg.cc/qMxnJ2J5/11.jpg)](https://postimg.cc/kBDDw6tQ)

Y listo tenemos nuestro programa para calcular sin necesidad de graficar.

</div>

# 5 VIDEO 

# 6 CONCLUSIONES 

Concluimos con éxito lo solicitado para poder entender como se forma un circuito por medio de este programa además personalmente me interezo mucho ya que contamos con las herramientas para formar un circuito y ademas por medio de este programa podemos resoverlo sin necesidad de cálculos es increíble como la tecnología nos lleva a crear programas que nos facilitan a vida hasta en cálculos.

# 7 BIBLIOGRAFÍAS

https://www.circuitlab.com/editor/#?id=7pq5wm&from=homepage

http://ngspice.sourceforge.net/

https://en.wikipedia.org/wiki/Ngspice
