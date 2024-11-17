---
{"dg-publish":true,"permalink":"/4-Notas principales/Homogeneas/"}
---


## Ecuaciones diferenciales homogéneas:
Estas yo las odio con una pasión.  Es muy fácil comerse un signo y que te arruine todo el procedimiento.

Estas son ecuaciones diferenciales con la estructura:

$$
P(x;y)dx+Q(x;y)dy=0
$$
Donde P y Q son homogéneas del mismo grado. En estos casos hacemos un cambio de variables para hacerlas separables.

Primero dividimos toda la ecuación por $X{^n}$, siendo n el grado de homogeneidad. Queda entonces

$$
P\left( \frac{y}{x} \right).dx+Q_{1}\left( \frac{y}{x} \right)dy=0
$$
Establecemos una sustitución de variables:

$$
\frac{y}{x}=v\to y=x.v
$$ 
Aplicando diferenciales:
$$
dy=x.dv+v.dx
$$
y remplazando en la ecuación:

$$
P(v).dx+Q_{1}(v)(x.dv+v.dx)=0
$$
$$
[P(v)+Q_{1}(v)].dx+Q_{1}(v).x.dv=0
$$
$$
[P(v)+Q_{1}(v)].dx=-Q_{1}(v).x.dv
$$
$$
\frac{1}{x}dx=-\frac{Q_{1}(v)}{[P(v)+Q_{1}(v)]} dv
$$
$$
\int \frac{1}{x}dx=-\int \frac{Q_{1}(v)}{[P(v)+Q_{1}(v)]} dv
$$
y de ahí resolvemos (con muchos pasos salteados por el libro pero lo vamos a ver mejor en los ejemplos). 
$$
x.C=e{{^{-\int \frac{Q_{1}(v)}{[P(v)+Q_{1}(v)]} dv}}}
$$
Que es la solución general de estas ecuaciones. 

Ejemplo:
$$
(x{^{2}+y{^2}}).dx+xy.dy=0
$$
Esta claramente es homogénea grado 2, así que dividimos por x^2

$$
( \frac{x{^2}}{x{^2}}+\frac{y{^2}}{x{^2}}).dx+\frac{xy}{x{^2}}.dy=0
$$
Simplificando y efectuando remplazos:

$$
\frac{y}{x}=v\to y=x.v
$$
$$
dy=x.dv+v.dx
$$

$$
(1+v{^2}).dx+v.(x.dv+v.dx)
$$
$$
(1+v{^2}+v{^2})dx+vx.dv=0
$$
<font size=2>Extraño cuando la matematica eran solo numeros loco </font>

$$
(1+2v{^2})dx=-vx.dv
$$
$$
\frac{1}{x}dx=-\frac{v}{(1+2v{^2})}dv\to \int \frac{1}{x}dx = -\int \frac{v}{(1+2v{^2})}dv
$$

$$
---
$$
Calculo auxiliar integral de la derecha:

$$
-\int \frac{v}{(1+2v{^2})}dv
$$
Multiplicando y dividendo por 4
$$
-\frac{1}{4}\int \frac{4v}{(1+2v{^2})}dv
$$
$$
Sustitucion
$$
$1+2v{^2}=t$ $dt=4v.dv$
$$
-\frac{1}{4}\int \frac{1}tdt\to-\frac{1}{4}.\ln(1+2v{^2})
$$
$$
---
$$
$$
\ln(x)+C=-\frac{1}{4}\ln(1+2v{^2})\to \ln (x)+\ln C=\ln\left[ (1+2v{^2}){^{-\frac{1}{4}}} \right]\to e{{^{\ln (x.C)}}}=e{{^{\frac{1}{{{^4}}\sqrt{}{ 1+2v{^2} }}}}}
$$
Queda

$$
[x.C=\frac{1}{{{^4}\sqrt{ 1+2v{^2} }}}]
$$
y Ahora volvemos a valores originales (no se olviden de hacer esto siempre)

$$
[x.C=\frac{1}{{{^4}\sqrt{ 1+2\frac{y{^2}}{x{^2}} }}}]
$$



En los próximos ejs esta ultima parte de despejar logaritmos la salteo porque ya esta demostrada acá ( si no se acuerdan fíjense propiedades de logaritmos).

Otros ejemplos:
 Ej 1 guía Venturini sección homogéneas:

$$
y{^2}-x{^2}=2xy.\left( \frac{dy}{dx} \right)
$$
La ecuación es claramente homogénea grado 2. Pasando el otro diferencial:

$$
(\frac{y{^2}}{x{^2}}-1).dx=\frac{2y}{x}dy
$$

sustituyendo 


$$
(v{^2}-1)dx=2v(x.dv+v.dx)\to(v{^2}-1)dx-2v(x.dv+v.dx)=0\to(v{^2-1-2v{^2}})dx-2vx.dv=0
$$


$$
-(v{^2+1})dx=2vx.dv\to -\frac{1}{x}dx=\frac{2v}{v{^2+1}}dv\to -\int \frac{1}{x}dx=\int \frac{2v}{v{^2}{+1}}dv
$$

$$
---
$$
Calculo auxiliar integral de la derecha:




$$
Sustitucion
$$
$t=v{^2}+1$   $dt=v{^2}.dv$

$$
\int \frac{1}{t}dt
$$

$$
\ln(v{^2+1})
$$
$$
---
$$

$$
-\ln(x)+C=\ln(v{^2+1})
$$

Que simplificando queda como 

$$
x{^{-1}}.C=v{^2+1}
$$
y volviendo a valores originales:

$$
[x{^{-1}}.C={(\frac{y}{x})^{2}+1}]
$$
Ej 5 guía Venturini sección homogéneas:

$$
(y{^2-x{^2}}).y{{^,}}+2xy=0
$$

$$
(y{^2-x{^2}}).y{{^,}}+2xy=0\to(y{^2-x{^2}}).\frac{dy}{dx}+2xy=0\to(y{^2-x{^2}}).\frac{dy}{dx}=-2xy\to(y{^2-x{^2}}){dy}=-2xy.dx
$$


Ahora que tenemos la función re armada

$$
(y{^2-x{^2}}){dy}=-2xy.dx
$$
Es homogénea grado 2

$$
(v{^2}-1).(x.dv+v.dx)=-2v.dx
$$
$$
(v{^2-1})xdv+(v{^3}-v)dx=-2v.dx
$$
$$
(v{^2-1})xdv=-2v.dx-(v{^3-v})dx
$$
$$
(v{^2-1})xdv=(-2v+v-v{^3})dx
$$
$$
(v{^2-1})xdv=-(v+v{^3})dx
$$

$$
-\frac{v{^2-1}}{v+v{^3}}dv=\frac{1}{x}dx
$$
$$
-\int \frac{v{^2-1}}{v+v{^3}}dv=\int\frac{1}{x}dx
$$
$$
---
$$
Calculo auxiliar integral de la izquierda:
$$
Fracciones 
$$

$$
\frac{v{^2-1}}{v+v{^3}}\to\frac{v{^2-1}}{v.({1+v{^2}})}\to \frac{A}{v}+\frac{Bv+C}{v{^2+1}}\to \frac{A.(v{^2+1})+(Bv+C)v}{v.(v{^2+1})}\to\frac{Av{^2+A+Bv{^2}+Cv}}{v.(v{^2+1})}
$$


$$
\frac{v{^2-1}}{v+v{^3}}=\frac{{(A+B)v^2+A+Cv}}{v.(v{^2+1})}
$$
Por lo tanto 

$A+B=1$ 
$A=-1$
$C=0$
$-1+B=1\to B=2$

Por lo cual la integral se puede re armar como 

$$
\frac{v{^2-1}}{v+v{^3}}=\frac{-1}{v}+\frac{2v}{v{^2+1}}
$$

Entonces 
$$
\int \frac{v{^2-1}}{v+v{^3}}dv=\int-\frac{1}{v}+\int \frac{2v}{v{^2+1}}
$$
Que queda

$$
-\ln(v)+\ln(v{^2+1})
$$
$$
---
$$

$$
-(-\ln(v)+\ln(v{^2+1}))=\ln x
$$
$$
\ln(v)-\ln(v{^2+1})=\ln x
$$
$$
\ln \left( \frac{v}{v{^2+1}} \right)=\ln x+C
$$
Que queda como

$$
\frac{v}{v{^2}{^+1}}=x.C
$$
y volviendo a valor original:

$$
\frac{y/x}{(y/x){^2}+1}=x.C
$$
$$
\frac{\frac{y}{x}}{\left( \frac{y+x}{x} \right){^2}}=x.C
$$
Por propiedad de fracciones 

$$
\frac{y.x{^2}}{(y+x){^2}.x}=x.C
$$
$$
\frac{y.x{^2}}{(y+x){^2}.x}.\left( \frac{1}{x} \right)=C
$$
$$
\frac{y}{y{^2}+x{^2}}=C
$$
