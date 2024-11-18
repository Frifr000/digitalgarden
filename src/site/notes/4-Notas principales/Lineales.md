---
{"dg-publish":true,"permalink":"/4-Notas principales/Lineales/"}
---

Estas parecen jodidas en la explicación pero en la practica terminan siendo bastante facilongas, solo hay que acordarse un par de formulas. 

Tienen la estructura

$$
y{^,}+P(x)y=Q(x)
$$
Donde P(X) y Q(x) son funciones continuas de x. La solución de estas ecuaciones tiene la forma de y=f(x), siendo estas todas las funciones posibles que satisfagan la ecuación. Lo que hacemos es sustituir $y=u.v$ donde U y V son funciones de x.
Entonces:
$y=u.v\to y{^,}=u{^,}.v+u.v{^,}$
y queda
$$
u{^,}.v+u.v{^,}+P(x)u.v=Q(x)
$$
Sacando factor común:
$$
v.[u{^,}+P(x).u]+u.v{^,}=Q(x) ----Ecuacion(1)
$$
y ahora buscamos una U(X) tal que el termino entre corchetes iguale a 0.

$$
u{^,}+P(x).u=0\to \frac{du}{dx}=-P(x).u\to \frac{1}{u}.du=-P(x).dx\to \int \frac{1}{u}du=-\int P(x).dx
$$
<font size=1>Cont.</font>
$$
\ln u=-\int P(x).dx\to u=e{^{-\int P(x).dx}}
$$
Ya que en este despeje  $v.[u{^,}+P(x).u]=0$ la ecuación (1) nos queda como

$$
v.[0]+u.v{^,=Q(x)\to u.v{^,}}=Q(x)
$$
Y ahora remplazamos u y despejamos v
$$
e{^{-\int P(x).dx}}.v{^,}=Q(x)\to e{^{-\int P(x).dx}}.\frac{dv}{dx}=Q(x)\to dv=e{^{\int P(x).dx}.Q(x).dx}
$$
<font size=1>Cont.</font>
$$
 \int dv=\int e{^{\int P(x).dx}.Q(x).dx}\to v=\int e{^{\int P(x).dx}.Q(x).dx}
$$
y ya que al principio de la ecuación nos planteamos que y=u.v , entonces la solucion general quedara como:

$$
y=u.v\to y=e{^{-\int P(x).dx}}.[\int e{^{\int P(x).dx}.Q(x).dx}+C]
$$
Y ahora se preguntan si hace falta hacer todo este lio de sustitución cada vez resolvemos una lineal, la respuesta es no. Con acordarse la formula de u y v y después multiplicarlas ya es suficiente. Entonces, para resolver estos ejercicios lo único que hace falta acordarse es que  

$u=e{^{-\int P(x).dx}}$
$v=\int e{^{\int P(x).dx}.Q(x).dx}$ o $v=\int u{^{-1}}.Q(x).dx$
Como se ve ahora en los ejemplos estos se resuelven bastante facil si solo reconocemos cual es cual:

Ejemplo:

Resolver 

$$
y{^,+x.y}=2x
$$
Acá claramente P(X)=x y Q(X)=2x así que si remplazamos

$$
u=e{{^{-\int x.dx}}}\to u=e{^{-x{^2}/2}}
$$
y ahora remplazamos en v

$$
v=\int e{^{x{^2}/2}}.2x.dx
$$
Calculo auxiliar integral


$$
Sustitucion
$$
$t=\frac{x{^2}}{2}$ $dt=x.dx$  $dx=\frac{1}{x}dt$

$$
\int e{^{x{^2}/2}}.2x.dx=\int e{^t}.2x.\frac{1}{x}dt=\int 2e{^t}dt=2\int e{^t}=2e{^t}
$$

$$
---
$$
Entonces 

$v=\int e{^{x{^2}/2}}.2x.dx=2e{^\frac{x{^2}}{2}}$


Ahora que tenemos v y u solo queda poner nuestras solución general :


$$
y=e{^{-x{^2}/2}}.(2e{^\frac{x{^2}}{2}} +C)
$$
No se si es necesario pero el libro siempre pone la constante en el paréntesis con v así que hagan eso tmb.

Otros ejemplos:

Venturini sección lineles ej 4

$$
y{^,}+\frac{3}{x}.y=x{^2}-x
$$
P(X)=$\frac{3}{x}$ 
Q(x)=$x{^2}-x$

$$
u=e{^{-\int 3/x.dx}}\to u=e{^{-3\int 1/x.dx}}\to u=e{^{-3\ln x}}\to u=x{{^{-3}}}
$$
$$
v=\int x{^{3}}.(x{^2}-x) .dx\to v=\int x{^{5}}-x{{^{4}}} .dx= \frac{x{^6}}{6}+\frac{x{^5}}{5}
$$
Solución general:

$$
y=x{{^{-3}}}.[\frac{x{^6}}{6}+\frac{x{^5}}{5}+C]
$$
Ej 8)

$$
y{^,}+5y=e{^{5x}}
$$
P(X)=5
Q(X)=$e{^{5x}}$

$$
u=e{^{-\int 5dx}}\to u=e{^{-5x}}
$$
$$
v=\int e{^{5x}}.e{^{5x}} dx\to \int e{{^{10x}}dx}\to \frac{e{{^{10x}}}}{10}
$$
S.G:

$$
y=e{^{-5x}}.\left( \frac{e{{^{10x}}}}{10}+C \right)
$$
