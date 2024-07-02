+++
title      = "Artillery Z Mod"
tags       = [ "Artillery", "Genius", "Mod", "OpenScad" ]
categories = [ "3DP" ]
date       = 2022-12-11T18:35:26-06:00
draft      = false
+++

![](/img/3dp/z-mod/zm-02.jpg)

[Modelos 3D](https://www.printables.com/es/model/338016-artillery-z-mod)

## Intro

Aunque las impresoras de la marca Artillery tienen en general buenas cualidades
y considerando el precio de venta se optiene lo que se paga, es innegable que
presenta varios defectos sobretodo en sus primeros modelos

Este es un intento de corregir uno de ellos, el *Bamboleo* (wobble) y "juego"
del eje z. Para ello se ha diseñado un nuevo carro y conseguido algunas piezas
variadas con la esperanza de que "por mera coincidencia" se comporten correctamente

Ciertamente, no estamos ante tecnologia de punta y es (se cree) que basta
un poco de sentido comun para dar con la respuesta

Para este proyecto se conto con hartas influencias, la primera fue una
modificacion de [Way2Do](https://www.thingiverse.com/thing:5268713) a un modelo
"abandonado" por [Ctr3D](https://www.thingiverse.com/thing:4344699), aunque
nunca se llego a imprimir

El otro proyecto que literalmente sirvio de plantilla fue realizado por parte de
[EnDiMa](https://www.printables.com/es/model/137175-artillery-genius-z-mod).

Este diseño no se adaptaba a lo que tenia en mente, ni contaba con un fichero para poder
realizar modificaciones como la gente, asi que se creo hechando mano de
OpenScad.

Dicho modelo si fue impreso, en caso de que el mio fallara

![](/img/3dp/z-mod/zm-01.jpg)

Sin embargo cuando se probo sobre el marco, ocurrio que la distancia a la que
estan colocadas las ruedas en este modelo (como en el de Way2Do) quedan en exceso
ajustadas, con un error aproximado de .6mm, ja, ja

Aun asi, el diseño es sencillo y facil de reproducir, por lo que se utilizo como "plantilla"

Creo que la primer influencia es el video que enlaza en por [aca](https://www.thingiverse.com/thing:4853171)

{{< youtube id="mqSQhwqSzvg" >}}

A decir verdad, encuentro la propuesta exagerada y el sistema de imanes "poco
confiable", ademas que no muestran la "diferencia" en forma de impresiones. Pese
a ello, es un video muy ilustrativo con ideas (para mi) nuevas

y adicionalmente

{{< youtube id="s8-e9McOoFA" >}}

La conclusion de lo anterior fue... 4 ruedas, acoplador oldham, tuerca T POM
antiretroceso y acoplador flexible

### Carro

El carro original puesto por Artillery no cuenta con ninguna forma de ajustar
las ruedas y al menos con el uso que he hecho de la impresora, no deberia
haber ninguna razon para que tenga un mal funcionamiento, aunque ocacionalmente
podria presenta un poco de juego

![](/img/3dp/z-mod/ZNC.jpg)

Quien no reconece las miticas ["tapitas"](https://www.thingiverse.com/thing:4444589)
que intentan corregir algunos inconvenientes de este carro?

![](/img/3dp/z-mod/z-upgrade.jpg)

realizando algunas pruebas, realmente no encontre algun cambio reseñable, pero
al menos dan paz mental a quien las coloca...

Dispuesto pues a la labor, por que no colocar 4 ruedas? Desconosco la razon de por que la mayoria
de impresoras monta carros de 3 ruedas, quiza sea solo por ahorrar(?) o es quiza
que en un eje con movimiento horizontal sea inecesario? Bueno, el eje Y cuenta
con un carro con 4 ruedas y no le va mal...

![](/img/3dp/z-mod/zm-09.jpg)

Al igual que en el carro Y, para poder ajustar la tencion en las ruedas se
colocaron dos tuercas exentricas

En un principio se contemplo el uso de tuercas de seguridad para mantener simpre
fijas las ruedas, pero al intentar ajustar junto a las tuercas cuadradas que van
en la extrusion 2040v, por alguna razon pense que era demaciado complejo
hacer coincidir el ajuste de ambas y que quedaran seguras. Por ello la opcion
por defecto es no contar con tuercas de seguridad, aunque es una caracteristica
aun presente en el modelo. Si elije esta opcion, tal como en el diseño de
*EnDiMa* se cuenta con un par de orificios extra a cada lado exclusivamente
para el ajuste de las tuercas T

Otra modificacion necesaria fue elevar el punto de union del carro con la tuerca
T y el acoplador oldham

![](/img/3dp/z-mod/zm-14.jpg)

Es *IMPORTANTE* reseñar que este carro no es compatible con "los cuadrados
azules" del carro incluidos por artillery. Si eso es lo que necesita, mida y
agregue un hueco en dicho espacio en el modelo

## OpenScad

Sinceramente, me da pereza escribir mucho del tema por aqui, si tiene necesidad
de modificar el diseño, al estar realizado en openscad tiene casi todo el
trabajo hecho, ja, ja

Hace mucho que no tocaba un programa "programable". Este esta lejos de ser motivo de horgullo,
y la pereza, junto a gastar 1KG de filamento en continuas iteraciones deberian
estas plasmadas en el, je, je, aun asi, me he divertido al escribirlo

## Impresion

Tenga correctamente calibrada la impresora, asegurese que ademas de los
perimetros externos los orificios internos tienen la medida correcta (dentro de
lo posible)

En mi Artillery Genius tengo configurado el valor de "Expansion Horizontal de
orificios" en `.25mm`. Este Ajuste ocacionalmente es problematico en conjuncion
con otros como lo son las correcciones de maya o las paredes delgadas, en este
modelo dichos parametros no afectan en nada, pero simpre revise la vista previa
de impresion...

Recomendo no imprimir ambas piezas directamente. Pruebe antes imprimir uno de los lados
con una configuracion "de prueba" (1 pared, 2 superior/inferior 5-15% de
relleno) y revise el ajuste de los componentes o... acorde a ellos y el
resultado de la impresion, realize las modificaciones pertinentes

Mi impresion final la realice con 4 paredes, 4 superior/inferior, 20% giroide
con lineas de relleno conectadas y un borde de 4mm. PETG, boquilla .4 altura .2

Sospecho que es una configuracion un poco excesiva, quiza con 3
paredes/inferior/superior y un 15% de relleno sencillo es suficiente, pero por
que escatimar?

Debido al "warping" (deformacion) en esquinas "puntiagudas"
recomiendo encarecidamente que coloque soportes en el "puente de union" (nombre
inventado). En mis impresiones, las piezas podian salir sin necesidad de ningun
soporte o... podia presentarse deformacion y desfasar un poco las capas o
provocar que la pieza se despegase, tomelo en cuenta

Esta es el area donde recomiendo soportes

![](/img/3dp/z-mod/p.png)

Por cierto, durante las pruebas utilice un modelo impreso de la extrucion 2040
V-Slot, puede encontrar ese y otros modelos interesantes aqui -&gt;
[https://www.thingiverse.com/thing:3973787](https://www.thingiverse.com/thing:3973787)

<h2 id="materiales">Materiales</h2>

![](/img/3dp/z-mod/zm-06.jpg)

Los enlaces son de afiliado a los materiales que he utilizado. Heche mano de su
propio criterio y guiese por la reputacion, comentarios y experiencia en compras
por aliexpress. Si puede o conoce mejores componentes no escatime en gastos.

Si decide comprar en esos sitios estara apoyando a este que escribe (y bla, bla,
bla). Si encuentra algun inconveniente, queja, el envio tarda 2 meses en llegar
o algo por el estilo, *NO JODA...*

- 8 Tornillo M5x40mm, 8 tornillo M3x12mm  ([https://s.click.aliexpress.com/e/_DCkvj0B](https://s.click.aliexpress.com/e/_DCkvj0B))
- 8 Tuerca M3 con nylon ([https://s.click.aliexpress.com/e/_DdRRKuF](https://s.click.aliexpress.com/e/_DdRRKuF))
- 8 Tuerca Cuadrada en T M5x10mmx10mm ([https://s.click.aliexpress.com/e/_DC4EheT](https://s.click.aliexpress.com/e/_DC4EheT))
- 8 Rueda de Polea 5x24x11 ([https://s.click.aliexpress.com/e/_DB1UCPt](https://s.click.aliexpress.com/e/_DB1UCPt))
- 2 Truecas T antiretroceso 8mm (Thread/Pitch/Lead 2) ([https://s.click.aliexpress.com/e/_DeZ8k19](https://s.click.aliexpress.com/e/_DeZ8k19))
- 2 Coples Oldham 1204 ([https://s.click.aliexpress.com/e/_DkF316j](https://s.click.aliexpress.com/e/_DkF316j))
- 4 Tuerca excentrica (7 diametro x 5mm internos x 6mm tuerca, en enlace "tipo B") ([https://s.click.aliexpress.com/e/_DBoMTYn](https://s.click.aliexpress.com/e/_DBoMTYn))

![](/img/3dp/z-mod/zm-03.jpg)

*ACTUALIZACION [18-12-22]*

Si bien el funcionamiento era correcto, tras una semana se retiraron los
acopladores flexibles para recolocar los "rigidos" originales.

Aparentemente se hiso un poco mas uniforme la apariencia entre capas

![](/img/3dp/z-mod/zm-03.jpg)

## Armado

(si la vuelvo a desmontar, prometo tomar fotografias, realmente es un poco
inutil detallar el proceso sin ellas, asi que unos pocos consejos. Pero... mejor mire
el siguiente video que al menos explica algunas cosas)

{{< youtube id="Y7AGsfoA3Kw" >}}

Para colocar los coples, utilice este [centrador](https://www.thingiverse.com/thing:3934158)

Para colocar y apretar los acopladores oldham utilice su ingenio, no es tan
complicado... *No los deje caer*, son muy, muy delicados, un pequeño golpe
puede fastidiarlos

Coloque los nuevos carros sin apretar las tuercas cuadradas

El ajuste en las tuercas exentricas debe ser uniforme en todas ellas, tambien
debe ser solo lo suficiente para evitar algun juego en el eje x, no los apriete
al limite

Para alinear el eje X, recoloque el "marco" de plastico, apriete los 4 tornillos
y suba el eje X al limite (quitando de en medio el cable del sensor de
filamento). Esto se hace con los las barillas roscadas y coples apretados **sin
la banda de sincronizacion superior**. Hay otros metodos, pero este me
funciono...

En este momento apriete las tuercas cuadradas

Una vez alineado con el tope libere los tornillos del lado izquierdo del marco
(los que lo unen con la impresora), baje la altura de la cama con las ruedas de
ajuste, encienda la maquina y realice un home en z. Apriete de nuevo los
tornillos del marco de lado izquierdo

Mueva el eje z por todo el recorrido y asegure que no se escucha ningun
"crujido" y todo el recorrido es suave

Revise todos los movimientos de las varillas y componentes, rehaga cualquier
paso las veces que sea necesaria

## Conclucion

![](/img/3dp/z-mod/ppr-01.jpg)

La impresion superior fue la que motivo toda esta modificacion. Segun mis
teorias, tenia un excesivo desgaste en la tuerca T de laton que en conjunto con
el propio diseño del carro, ocacionalmente tras los "saltos en Z" el extrusor no
regresaba a la altura correcta

![](/img/3dp/z-mod/zm-19.jpg)
![](/img/3dp/z-mod/zm-20.jpg)

Realice algunas impresiones de piezas mas pequeñas, pero realmente no encontre
ninguna diferencia destacable al estado de la maquina en buen funcionamiento

En muchos aspectos, las "modificaciones" afectan de forma insignificante (cuando
no inapreciable) las impresiones, pero como pasa en el mundo de la modificacion
de automoviles (supongo...), esto es una parte muy importante del pasatiempo. A
veces es necesaria, a veses desquisiante y ocacionalmente divertida

B-u-e-n-o... tenia ese problema que termino por hacer fragil e inservible la
impresion del pez koi

![](/img/3dp/z-mod/pr-11.jpg)

Puedo decir con alegria y cierto horgullo, que al menos la modificacion no
afecto para mal la impresora y de hecho soluciono el problema

![](/img/3dp/z-mod/pr-02.jpg)
![](/img/3dp/z-mod/pr-03.jpg)
![](/img/3dp/z-mod/pr-04.jpg)

Con esto de las fotografias muchas veces se pueden hacer tomas para disimular
las imperfecciones, pero he realizado lo mejor posible para exponer todos los detalles

![](/img/3dp/z-mod/pr-05.jpg)
![](/img/3dp/z-mod/pr-06.jpg)
![](/img/3dp/z-mod/pr-07.jpg)

Valio la pena? Se corrigio el problema "a mi manera", asi que si!

![](/img/3dp/z-mod/zm-15.jpg)

El filamento blanco y tamben el natural, son excelentes si se quieren disimular imperfecciones

![](/img/3dp/z-mod/pr-13.jpg)
![](/img/3dp/z-mod/pr-14.jpg)
![](/img/3dp/z-mod/pr-15.jpg)
![](/img/3dp/z-mod/pr-17.jpg)

... pero en negro tampoco queda nada mal

![](/img/3dp/z-mod/pr-21.jpg)
![](/img/3dp/z-mod/pr-20.jpg)

disfrut!

![](/img/3dp/z-mod/zm-13.jpg)
