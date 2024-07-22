+++
title      = "Mediciones"
tags       = [ "Tiinnitus-HiFi" ]
categories = [ "Tinnitus-HiFi" ]
date       = 2024-07-06T21:07:46-06:00
draft      = false
+++

![](/img/thf/mediciones/soporte-0.jpg)

Aqui se muestra el equipo, especificaciones y metodo de medicion del "proyecto
**Tinnitus HiFi**"

La configuracion, metodologia y espacio de las mediciones no son ideales ni
acordes a ninguna especificacion conocida y solo son comparables (en el mejor de los
casos) con otras publicadas por Tinnitus HiFi

Mi agradecimineto a **Mark Ryan** (Super*Review) por el sitio [squig.link](https://squig.link),
ademas del mantenimiento, revisiones y mejoras de la herramineta [CrinGraph](https://github.com/mlochbaum/CrinGraph)
originalmente creada por **Mlochbaum** con la aportacion de [**Rohsa**](https://gitlab.com/rohsa/graphtool)
que incorporo [AutoEq](https://github.com/jaakkopasanen/AutoEq) de **Jaakko Pasanen**
y a [**Crinacle**](https://crinacle.com/) por dar inicio a la idea

## Equipo

Acoplador compatible 711 60318-4 Type E810A

Pinna compatible 45ca (oreja)

Soporte DIY de acoplador y pinna

Computador dedicado con W11 sin conexion a internet

- mother Asus B350M-E
- 8GB DDR4 3200
- AMD A6-9500

Amplificador Aiyima H1

Amplificador Douk U3

Fiio K11

## Metodo

Se utiliza un muestreo de 96KHz con longuitud de 512k, calibrando el nivel de
entrada a 75 decibeles SPL con ruido rosa

El microfono del acoplador se conecta directamente a la placa madre
ajustando la entrada al 90% en los ajustes de sonido de windows

La salida jack 3.5 de la placa se conecta al amplificador Aiyima H1

En caso de problemas con la amplificacion se prueba con el amplificador douk U3
y finalmente con el DAC/AMP Fiio K11

No cuento con un microfono calibrado, asi que se utilizo una aplicacion de
sonometro en un celular alineando el microfono con el borde de la almohadilla de
un audifono hasta alcanzar 75 decibeles SPL y con ello se calibro el nivel de entrada

Al realizar el loop de calibracion la respuesta se mantiene plana en el rango de
20-20KHz, haciendo pruebas tanto si hay establecido un archivo de calibracion
como si no, no hay variaciones visibles en el resultado, asi que no se utiliza

Algo igual sucede con el achivo de calibracion del microfono, tanto si se
establece como si no, el resultado no varia, sin embargo en este caso se
conserva por si acaso...

En este momento solo se cuenta con la pinna derecha, solo se publican mediciones
de ambos lados de audifonos que son exactamente iguales en el lado derecho e
izquierdo sin ninguna angulacion o geometria especifica

Tanto en Over Ears como In Ears se busca un sello perfecto

En iems el grado de insercion se hace coincidir (si es posible) con una resonancia a 8KHz
y se realiza un par de mediciones para descarcar cualquier error, aunque solo
una se publica

En Over Ears siempre que se mantenga el sello se realizan 4 mediciones modificando la
posicion partiendo de una colocacion "ideal" y luego 3 cambios de posicion para
generar un promedio

Para los On Ears Se busca una posicion ideal aunque esta no siempre consiga un
buen sello

Se descartan las mediciones "extrañas" o con demaciada divergencia

El promedio de estas mediciones se alinea en 500 Hz a 60 SPL sin suavizado
en un rango de 20-20KHz

La medicion o premedio (segun el caso) se exporta como un txt en rango de
20-20Khz con una resolucion de 48PPO delimitado por tabuladores

En squig la medicion se presenta con alineacion a 60dB 500Hz con un suavizado `5`
que se puede ajustar a voluntad

![](/img/thf/mediciones/squig.png)
