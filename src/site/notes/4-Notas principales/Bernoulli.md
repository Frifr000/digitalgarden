---
{"dg-publish":true,"permalink":"/4-Notas principales/Bernoulli/"}
---

Las ecuaciones diferenciales se puede resolver con Bernoulli si tiene la estructura:

$$
y{^,}+P(x)y=Q(x).y{{^n}}
$$
Si n=0, entonces es una ecuación lineal y si n=1 es una variables separables. Entonces lo que se desprende es todo esto es que en realidad los métodos de variables separables y lineal son casos particulares de Bernoulli. De todas formas todos los ejemplos que vamos a ver acá son ecuaciones donde n no es ni 0 ni 1. 
Para resolver estas ecuaciones primero dividimos la ecuación por $y{{^n}}$.

$$
y{^,}y{^{-n}}+P(x)y{^{1-n}}=Q(x)
$$
Quedándonos con esta estructura.
Ahora establecemos una sustitución de variables donde 
$$
y{^{1-n}}=z
$$
Por lo cual :
$$
(1-n)y{^{-n}}.y{^,}=z{^,}
$$
$$
y{{^{-n}}y{^,}=\frac{z{^,}}{1-n}}
$$
Y ahora remplazamos 
$$
\frac{z{^,}}{1-n}+P(x)z=Q(x)
$$
y si multiplicamos por 1-n

$$
{z{^,}}+P(x)z.(1-n)=Q(x).(1-n)
$$
Nos queda una ecuación que se puede resolver por variables separables o como lineal.

Ejemplo:

$$
y{^,}-\frac{1}{x}y=\frac{3}{x}y{^3}
$$
Dividiendo por y^3 

$$
y{^,}y{^{-3}}-\frac{1}{x}y{{^{-2}}}=\frac{3}{x}
$$
Ahora remplazando por z

$$
z=y{^{-2}}
$$
$$
\frac{z{^,}}{-2}-\frac{1}{x}z=\frac{3}{x}
$$
Y multiplicamos por -2

$$
{z{^,}}+\frac{2}{x}z=-\frac{6}{x}
$$
Queda una ecuación lineal con variables x y z:

P(x)=2/x
Q(x)=-6/X

$$
z=u.v
$$
$$
u=e{{^{-2\int 1/x.dx}}}=x{{^{^-2}}}
$$
$$
v=\int x{^2}.-\frac{6}{x}.dx=-\int 6x.dx=-3x{^2}
$$

$$
z=x{{^{-2}}}.[-3x{^2}.C]
$$
y remplazamos z al final:
$$
y{{^{-2}}}=x{{^{-2}}}.[-3x{^2}.C]
$$
Simplificando la expresión:

$$
y{{^{-2}}}=-3+C.x{^{-2}}
$$
Otros ejemplos:

Guía Venturini ej 3)

$$
xy{^,}-y=y{^3}
$$
Lo llevamos a la estructura de Bernoulli:

$$
xy{^,}=y+y{^3}
$$
$$
y{^,}=\frac{y}{x}+\frac{y{^3}}{x}
$$
$$
y{^,}-\frac{y}{x}=\frac{y{^3}}{x}
$$
Dividimos todo por y^3

$$
y{^,}.y{^-3}-\frac{1}{x}y{^{-2}}=\frac{1}{x}
$$
Remplazamos por z=y^-2
$$
\frac{z{^,}}{-2}-\frac{1}{x}z=\frac{1}{x}
$$
y multiplicamos por -2
$$
z{^,}+\frac{2}{x}z=-\frac{2}{x}
$$
Queda una lineal

P(X)=2/x
Q(x)=-2/x

$$
u=e{^{-2\int 1/x.dx }}=x{^{-2}}
$$
$$
v=\int x{^2}. -\frac{2}{x} .dx=-\int 2x.dx=-x{^2}
$$
Solucion General:

$$
y{{^{-2}}}=x{{^{-2}}}.[-x{^2}.C]
$$
$$
y{{^{-2}}}=-1+C.x{^{-2}}
$$

Ej 8)

$$
xy{{^,}+y=-xy{^2}}
$$
Pasamos a estructura de Bernoulli:

$$
y{^,}=-y{^2}-\frac{1}{x}y
$$
$$
y{^{{^,}}}+\frac{1}{x}y=y{^2}
$$
Dividimos por y^2

$$
y{^,}y{{{^{-2}}}}+\frac{1}{x}y{{^{-1}}}=1
$$
Remplazamos por z
$$
\frac{z{{^,}}}{-1}+\frac{1}{x}z=1
$$
Multiplicamos por -1

$$
z{^,}-\frac{1}{x}z=-1
$$
Queda una lineal:

$$
u=e{{^{-\int -1/x dx}}}=x
$$
$$
v=\int x{{^{-1}}}.1 .dx=\ln x
$$
Solución General:

$$
y{^{-1}}=x[\ln x.C]
$$
