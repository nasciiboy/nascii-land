+++
title      = "COSMOFONO"
tags       = [ "fonos", "cli" ]
categories = [ "post" ]
date       = 2024-06-29T02:13:20-06:00
draft      = false
+++

![](/img/post/cosmofono/AbbeyZilla.jpeg)

## o... como organizar tu audioteca digital manualmente...

Encuentro molesta la complejidad de los sofisticados y potentes reproductores
musicales, llenos de botoncillos que van a su bola recopilando metadatos de cada
una de las pistas que encuentre, cuando lo unico que necesito es que reprodusca
las pistas de una carpeta que ya tengo dispuesta como un album

Asi las cosas les comparto mi sencillo sistema para organizar los miles de
albums en mi personal coleccion

La carpeta principal en la raiz del usuario `~/Música` la renombre como
`~/fonos` para hacer mas facil teclear la ruta...

![](/img/post/cosmofono/cosmofono-01.png)

En esta carpeta `fonos` habitan los nombres de toda agrupacion que tenga mas de
un produccion o se gane tal honor con un solo lanzamiento. Asi pues encontraran
a **Sonic Youth**, **Led Zepellin**, **The Beatles**, **Electric Light
Orchestra**, **Neil Young**, **Taeko Ohnuki**, **Supertramp**, **Archive**,
**Fishmans**, etc.


Estas carpetas siempre estan organizadas en orden alfabetico y dentro de ellas
**cada album escuchado** se antepone de la siguiente forma

    =19XX= nombre album (informacion especial)

donde `=19XX=` es el año de lanzamiento siempre y unicamente con cuatro digitos
en medio de dos signos igual (`=`), luego el nombre del album y al final
(opcionalmente) alguna informacion especial, por ejemplo `(2006)` que seria si
corresponde a alguna reedicion del 2006, `(Bonus Disc)`, `(POCH-1640)` numero de
catalogo si se tiene varias versiones del album del mismo añø, `(mp3)` o lo que
se considere revelante

![](/img/post/cosmofono/cosmofono-02.png)

obviamente si un album aun no ha sido escuchado o su procedencia y calidad es
seriamente dudosa no recive este tratamiento

Motivos para ignorar albums son:

- contiene pistas con errores (corroborados). En ocaciones simplemente son
  asi... en cualquier formato y version y no hay mas que aceptarlos

- la fuente de audio es un vinil no oficial y existe su contraparte digital sin mierdas

- la fuente de audio es un sucio y asqueroso vinil muy dañado de algun loco aficionado

- es un asqueroso vinil con sobremuestreo "24/192"

- si, es un vinil

**Cuidado** siempre con esos archivos mas alla del *16/44*, aunque adquieras
archivos de forma digital y legal **PUEDE SER UN ASQUEROSO VINIL**. Je, je, si no
existe la grabacion sin ruiditos molestos o por que no existe otra fuente mas
que un vinil se soporta, pero siempre huye del vinil

Bueno, bueno, regresando al tema el sistema `=XXXX=` es facil de llevar y
aunque olvides si has escuchado o no un album estara la marca para despejar dudas

y si aplicas algunos comandos linuxeros, por ejemplo en un terminal (con
interprete `fish`), puedes contabilizar cuantas pistas tienes en total y cuantas
de ellas has escuchado, tal que asi

    # total de albums escuchados (carpetas principales)
    find -type d | grep -P '/(=[0-9]{4}=|=DONE=)[^/]*$' | wc -l
    # total de pistas escuchadas
    find (find -type d | grep -P '/(=[0-9]{4}=|=DONE=)[^/]*$') | grep -P '(flac|alac|m4a|aac|wav|mp3|ogg|ape|aiff)$' | wc -l
    # total de pistas
    tree | grep -P '(flac|alac|m4a|aac|wav|mp3|ogg|ape|aiff)$' | wc -l

en mi maquina arroja lo siguiente

![](/img/post/cosmofono/cosmofono-03.png)

*2149* Albums escuchados, *31,150* pistas reproducidas y *76,748* en total. Nada
mal, me falta mas de la mitad, hace como un año tenia mas o menos 24k/70k

## Consideraciones especiales

Cuando un album no me importa demaciado o no encuentro la informacion de
lanzamiento en lugar de fecha lo etiqueto asi

    =DONE= album (cosas)

Si por alguna razon la que fuera existe una pista escandalosamente defectuosa o
que asi parece y no puedo comprobar si es asi, antepongo un "balaso" al nombre
del album

    =DONE= ¤ album (cosas)

y dentro del album al nombre de la pista

    05. ¤ pista-sospechosa

Los albums ripeados por gente seria, tienen sumas de chequeo para revisar la
integridad de las pistas... pero en mi maquina hippiosa aun no tengo nada de
eso...

## Carpetas especiales

Tengo unas cuantas carpetas para disminuir la abultada cantidad de material,
primero

- `~/fonos/7empura` Todos los discos acumulados que no se ni que son, ni han sido oidos (muchos, muchos)

- `~/fonos/0CD` Mis CD's ripeados esperando a ser escuchados

- `~/fonos/1CD` Mis CD's escuchados que no se donde poner... o no quiero buscarles lugar

- `~/fonos/2tuB` oggs de yutuve...

- `~/fonos/4k` Los sountracks de anime, peliculas, videojuegos y series

inician con un numero por conveniencia, para tenerlos a la mano

- `~/fonos/one` Aqui van discos solitarios o sin mucho interes que no son tan
   malos como para borrarlos

Los discos solitarios se pueden nombrar de la siguiente forma

    =19XX= agrupacion – album (cosas)

## Programas

En el sistema del ñu, utilizo [moc](http://moc.daper.net/) (Music on Console)
porque... funciona, es sencillo y me gusta, todo teclado, busquedas inmediatas,
reproduccion como carpeta de serie y amplia compativilidad de formatos
(No DSD)

![](/img/post/cosmofono/cosmofono-04.png)

En android utilizaba *SciMu* desde el repositorio de f-droid y anque era bastante
fan, un dia note que el efecto estereo (por no se que razon) no era muy preciso en
los paneos

![](/img/post/cosmofono/cosmofono-07.jpg)

asi que principalmente ocupo VLC

![](/img/post/cosmofono/cosmofono-18.jpg)

por las dudas y cuentos audiofilos, tambien tengo instalado USB Audio Player
aunque por su lentitud, consumo y engorro rara es la vez lo ocupo. Ademas, los
dongles y modos exclusivos son un fastidio, ja, ja, ja

ya que mucha musica no puedo transoportar, en el movil coloco los discos sin mas,
muy raramente ninguna discografia entera

Disfrut!
