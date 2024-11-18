---
{"dg-publish":true,"permalink":"/4-Notas principales/Exactas/"}
---

Estas son bastante fáciles. 

Una ecuación diferencial con la estructura $P(x;y).dx+Q(x;y).dy=0$ es exacta si existe una función U(x;y) tal que su diferencial iguale a la ecuación ($P(x;y).dx+Q(x;y).dy=dU$). Entonces, la solución de la función diferencial se puede expresar como 

$$
\int dU=C \to U(x;y)=C
$$
Por lo tanto, para solucionar ecuaciones con esta estructura hay que encontrar la función potencial U, si esta existe. 

Para verificar su existencia probamos con la condición de simetría que dice :

si $P(x;y).dx+Q(x;y).dy=dU$ entonces lógicamente $U{^,}_{x}=P$ y $U{^,}_{y}=Q$ (acuérdense que $dz=z{^,}_{x}.dx+z{^,}_{y}.dy$ ). Entonces partiendo de eso las derivadas cruzadas serán:

$$
U{^{,,}}_{xy}=P{^,}_{y} 
$$
$$
U{^{,,}}_{yx}=Q{^,}_{x}
$$
Así que para que se cumpla la condición de simetría 
$$
Q{^,}_{x}=P{^,}_{y}
$$
Una vez que se verifica(si no se verifica entonces se resuelve como [[4-Notas principales/Factor integrante\|Factor integrante]]) la condición de simetría, calculamos U:

$$
U{^,}_{x}=P\to \frac{dU}{dx}=P\to \int dU=\int P(x;y)\to U=\int P(x;y) dx
$$
Ahora tenemos que tener cuidado con algo acá, ya que estamos integrando una función que depende de (x,y) simultáneamente, pero solo la integramos con respecto a x(solo hay un diferencial). Entonces, la integral a demás  de tener la función resultante del calculo de la integral también va a tener una constante con respecto a y, quedando así. 

$$
\int P(x;y) dx=f(x;y)+\alpha(y)
$$
y lógicamente si despejamos de la misma forma $U{^,}_{y}=Q$  nos va a dar que 

$$
\int Q(x;y) dy=f(x;y)+\beta(x)
$$
y U nos quedara como 
$$
U=f(x;y)+\alpha(y)+\beta(x) =C
$$

En otras palabras, para despejar U vamos a tener que integrar P y Q y fijarnos por comparación cual es alfa y cual es beta. Esto se ve mejor en ejemplos:

Ejemplo:

Resolver
$$
(2x{^3}+y)dx+(x+2y{^2})dy=0
$$

$(2x{^3}+y)=P(x;y)$
$(x+2y{^2})=Q(x;y)$

Primero verificamos condición de simetría 
$$
P{^,}_{y}=1
$$
$$
Q{^,}_{x}=1
$$
Se verifica la condición, existe U.

$$
\int P=\int (2x{^3}+y).dx=\frac{x{^4}}{2}+xy +\alpha(y)
$$
$$
\int Q=\int (x+2y{^2})dy=xy+\frac{2y{^3}}{3} +\beta(x)
$$
Como vemos las 2 integrales comparte en termino xy por lo cual esa es nuestra f(x;y), mientras que la integral de p tiene una función que solo depende de x ($\frac{x{^4}}{2}$), por lo cual podemos inferir que esa es la constate de x que falta en la integral de Q ($\frac{x{^4}}{2}=\beta(x)$) y lo mismo pasa con la función que depende solo de y en la integral de Q ($\frac{2y{^3}}{3}=\alpha(y)$).
Entonces la solución general será :

$$
U=C\to xy+\frac{2y{^3}}{3}+\frac{x{^4}}{2}=C
$$

Otros ejemplos:
Guia Venturini sección exactas ej 2

$$
(2x-y)+(y{^2}-x).\frac{dy}{dx}=0
$$
Primero la llevamos a la estructura de una exacta:

$(y{^2}-x).\frac{dy}{dx}=-(2x-y)\to(y{^2}-x){dy}=-(2x-y)dx\to(2x-y)dx+(y{^2}-x)dy=0$

P(X)=2x-y
Q(X)=$y{^2}-x$
Verificamos simetría:


$$
P{^,}_{y}=-1
$$
$$
Q{^,}_{x}=-1
$$
Se verifica.
Despejamos U:

$$
\int(2x-y) dx= \frac{2x{^2}}{2}-xy
$$

$$
\int (y{^2}-x)dy=\frac{y{^3}}{3}-xy
$$

Solución general:

$$
-xy+{x{^2}}+\frac{y{^3}}{3}=C
$$
EJ 3)

$$
y{^,}=\frac{2xy}{y{^2}-x{^2}}
$$
$$
\frac{dy}{dx}=\frac{2xy}{y{^2}-x{^2}}
$$
$$
(y{^2-x{^2})dy}=(2xy)dx\to(-2xy)dx+(y{^2-x{^2})dy}=0
$$

P(X)=$-2xy$
Q(X)=$y{^2-x{^2}}$

Verificamos simetría:

$$
P{^,}_{y}=-2x
$$
$$
Q{^,}_{x}=-2x
$$
Se verifica simetría.  Despejamos U

$$
-\int 2xy. dx= -x{^2y}
$$
$$
\int (y{^2}-x{^2}).dy=\frac{y{^3}}{3}-x{^2y}
$$

Solución general:

$$
-x{^2y}+\frac{y{^3}}{3}=C
$$

