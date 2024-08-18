+++
title      = "Mediciones"
tags       = [ "" ]
categories = [ "thf" ]
date       = 2024-07-27T03:20:59-06:00
draft      = false
+++

![](/img/thf/mediciones/soporte-0.jpg)

Aqui se muestra el equipo, especificaciones y metodo de medicion del "proyecto
**Tinnitus HiFi**" publicadas en [squig](https://tinnitus-hifi.squig.link/)

La configuracion, metodologia y espacio de las mediciones no son ideales, solo
son comparables (en el mejor de los casos) con otras publicadas por Tinnitus
HiFi

Mi agradecimineto a **Mark Ryan** (Super*Review) por el sitio [squig.link](https://squig.link),
ademas del mantenimiento, revisiones y mejoras de la herramineta [CrinGraph](https://github.com/mlochbaum/CrinGraph)
(https://github.com/MRSallee/CrinGraph) originalmente creada por **Mlochbaum** con la aportacion de [**Rohsa**](https://gitlab.com/rohsa/graphtool)
que incorporo [AutoEq](https://github.com/jaakkopasanen/AutoEq) de **Jaakko Pasanen**
y a [**Crinacle**](https://crinacle.com/) por dar inicio a la idea

Un agradecimiento especial a Gustavo Gonzáles ([Auriculares Argentina](https://www.youtube.com/c/AuricularesArgentina))
por su ardua labor y esfuerzo al divulgar en español la necesidad de mediciones.

Tambien a [Darkeniel](https://www.youtube.com/@Darkeniel) por aportar desinteresadamente el DAC/AMP Fiio K11
y mostrar personalmente el uso de REW

## Equipo

Acoplador compatible 711 60318-4 Type E810A

![](/img/thf/mediciones/c-2.jpg)

Pinna (oreja) compatible 45ca

![](/img/thf/mediciones/a.jpg)

Soporte DIY de acoplador y pinna

Computador dedicado con W11 sin conexion a internet

- mother Asus B350M-E
- 8GB DDR4 3200
- AMD A6-9500

Amplificador Aiyima H1 (Principal)

Amplificador Douk U3

Fiio K11

## Metodo

En REW se utiliza un muestreo de 44.1KHz con longuitud de 512k, calibrando el
nivel de entrada a 95 decibeles SPL con onda sinusoidal a 1Khz

El controlador dedicado realtek proporcionado por asus se establecio en 44.1KHz
con 24Bits de profundidad

El microfono del acoplador se conecta directamente a la placa madre
ajustando la entrada al 90% en los ajustes de sonido de windows

La salida jack 3.5 de la placa se conecta al amplificador Aiyima H1

En caso de problemas con la amplificacion se prueba con el amplificador douk U3
y finalmente con el DAC/AMP Fiio K11

![](/img/thf/mediciones/lab_cal.jpg)

Como medio de calibracion se utilizo de referencia el iem *WG T-One* conectado
al amplificador AIYIMA H1 a 0.100V con una frecuencia de 1Khz calibrando el
nivel de entrada como 105dB

![](/img/thf/mediciones/wg_t-one.jpg)

![](/img/thf/mediciones/wg_t-one-specs.jpg)

Se verifico la calibracion con otros dos iems, el *CCA CXS*

![](/img/thf/mediciones/cxs-specs.jpg)

que marcaba

![](/img/thf/mediciones/cxs.jpg)

y el *KZ PR3*

![](/img/thf/mediciones/pr3-specs.jpg)

que marcaba

![](/img/thf/mediciones/pr3.jpg)

Al realizar el loop de calibracion la respuesta se mantiene plana en el rango de
20-20KHz, haciendo pruebas tanto si hay establecido un archivo de calibracion
como si no, no hay variaciones visibles en el resultado, asi que no se utiliza

Algo igual sucede con el achivo de calibracion del microfono, tanto si se
establece como si no, el resultado no varia, sin embargo en este caso se
conserva por si acaso...

En este momento solo se cuenta con la pinna derecha, solo se publican mediciones
de ambos lados de audifonos que son exactamente iguales en el lado derecho e
izquierdo sin ninguna angulacion o geometria especifica

![](/img/thf/mediciones/em-00.jpg)

La medicion de earbuds en esta plataforma a mi parecer no representa
apropiadamente como se persive el sonido, aun asi se cree que agrega valor a
modo de registro y comparacion sobre el propio sistema y para sistemas similares

La naturaleza propia de los earbuds no favorece un sello perfecto, por ello en
su mayoria se colocan sobre la oreja sin espumas, a menos que no se mantengan
por si mismos en una posicion estable. Se quita y recoloca con pequeños ajustes
para realizar al menos 4 mediciones en total y con ellas generar un promedio

Tanto en Over Ears como In Ears se busca un sello perfecto

En iems el grado de insercion se hace coincidir (si es posible) con una
resonancia a 8KHz. Solo y unicamente se publica una medicion para cada lado
(R y L)

En Over Ears siempre que se mantenga el sello se realizan al menos 4 mediciones
modificando la posicion partiendo de una colocacion "ideal" y luego 3 cambios de
posicion para generar un promedio

Para los On Ears Se busca una posicion ideal aunque esta no siempre consiga un
buen sello

Para todas las mediciones Se descartan las mediciones "extrañas" o con demaciada divergencia

La medicion o premedio  **sin suavizado** (segun el caso) se exporta como un txt en rango de
20-20Khz con una resolucion de 48PPO delimitado por tabuladores

En squig la medicion se presenta con alineacion a 60dB 1KHz con un suavizado `5`
que se puede ajustar a voluntad

![](/img/thf/mediciones/squig.png)

## Comparaciones

Aunque se menciono la falta de rigor de nuestras mediciones y mas fuera del
mismo sistema, no esta de mas satisfacer el morbo y ver que tanto divergen con
otras

![](/img/thf/mediciones/mele.png)

![](/img/thf/mediciones/ba8.png)

![](/img/thf/mediciones/400SE.png)


La descarga de los datos esta habilitada para su comodidad, asi que puede hacer
todas las comparaciones que desee

Disfrut!
