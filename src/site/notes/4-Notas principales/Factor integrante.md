---
{"dg-publish":true,"permalink":"/4-Notas principales/Factor integrante/"}
---

En el caso que una ecuación exacta no cumpla la condición de simetría, el procedimiento sigue siendo mayormente el mismo pero con unos pasos agregados. Si no se cumple la condición de simetría, entonces debemos buscar un factor integrante que al multiplicarlo por toda la ecuación la transforme en una ecuación exacta. 

Entonces si tenemos la ecuación  
$$
P(x;y).dx+Q(x;y).dy=0
$$
Tenemos que encontrar un factor integrante $u$ (que puede depender de x, y o los 2) tal que 


$$
u.P(x;y).dx=M(x;y) 
$$
$$
u.Q(x;y)=N(x;y)
$$
y 

$$
N{^,}_{x}=M{^,}_{y}
$$
Como dije antes, el factor integrante puede depender de x, y o (x;y). El procedimiento para $u(x)$ y $u(y)$ es muy parecido y últimamente da el mismo resultado, así que es una cuestión de cual prefieren hacer. Por temas de simpleza yo lo voy  a hacer todo con $u(x)$. Aunque en el libro también explican brevemente como se haría con y.  Factor integrante de $u(x;y)$ es mucho mas complicado de hacer por lo que no se toma en Análisis Matemático II. 

Entonces para encontrar el factor integrante con respecto a x tenemos que plantear la ecuación:

$$
\frac{P{^,_{y}}-Q{^,}_{x}}{Q}
$$
Si queda una función que depende exclusivamente de x, entonces existe $u(x)$. Si la función no depende solo de x ( en la  guía casi nunca pasa esto pero lo agrego por si acaso) , se calcula con
$$
$$
$$%
\frac{Q{^,_{x}}-P{^,}_{y}}{P}
$$
Si queda una función que depende exclusivamente de y, entonces existe $u(y)$.

Volviendo al ejemplo de $u(x)$ , una vez que calculamos $\frac{P{^,_{y}}-Q{^,}_{x}}{Q}$ y verificamos que depende solo de x, ahí calculamos el factor integrante en si mismo, que se calcula como:

$$
u=e{{^{\int\frac{P{^,_{y}}-Q{^,}_{x}}{Q}dx}}}
$$
En caso de u(y) es lo mismo pero se usa $\frac{Q{^,_{x}}-P{^,}_{y}}{P}$. Una vez que encontramos el factor integrante, multiplicamos a la función por u(x) y resolvemos como si fuera una exacta normal. 

Ej: Resolver
$$
(y+\ln x).dx-x.dy=0
$$
Primero verificamos simetría:

$$
P{^,}_{y}=1
$$
$$
Q{^,}_{x}=-1
$$
No se verifica, sacamos factor integrante:

$$
\frac{P{^,_{y}}-Q{^,}_{x}}{Q}=\frac{1+1}{-x}=\frac{2}{-x}
$$

La función depende solo de x, existe factor integrante. 

$$
u(x)=e{{^{-2\int \frac{1}{x}dx}}}=e{^{-2\ln x}}=x{^{-2}}
$$
El factor integrante es entonces x^2. 

Multiplicamos por factor:

$$
\left( \frac{y}{x{^2}}+\frac{\ln x}{x{^2}} \right).dx-\frac{1}{x}.dy=0
$$
verificamos simetría:

$$
P{^,}_{y}=\frac{1}{x{^2}}
$$$$
Q{^,}_{x}=\frac{1}{x{^2}}
$$
Se verifica. Despejamos U

$$
\int \left( \frac{y}{x{^2}}+\frac{\ln x}{x{^2}} \right) dx=-\frac{y}{x}-\frac{\ln x+1}{x}+a(y)
$$
$$
\int\left( \frac{1}{-x} \right)dy=-\frac{y}{x}
$$
Solución general:


$$
-\frac{y}{x}-\frac{\ln x+1}{x}=C
$$
Otro ejemplo:

Guia venturni parte generales ej 2

$$
(x{^2}+y{^2+x})dx+xy.dy=0
$$
$$
P{^,_{y}}=2y
$$
$$
Q{^,_{x}}=y
$$
No se verifica. Sacamos factor integrante segun x

$$
\frac{2y-y}{xy}=\frac{1}{x}
$$
Existe factor integrante según x
$$
u(x)=e{{^{\int1/x.dx}}}=e{{{{^{\ln x}}}}}=x
$$
Multiplicamos por x

$$
$$
$$
(x{^3}+xy{^2+x{^2}})dx+x{^2}y.dy=0
$$

$$
P{^,_{y}}=2yx
$$
$$
Q{^,_{x}}=2xy
$$
Se verifica simetria:

$$
\int(x{^3}+xy{^2+x{^2}}).dx=\frac{x{^4}}{4}+\frac{x{^2}y{^2}}{2}+\frac{x{^3}}{3}
$$
$$
\int x{^2}y.dy =\frac{x{^2}y{^2}}{2}
$$
Solución general:

$$
\frac{x{^4}}{4}+\frac{x{^2}y{^2}}{2}+\frac{x{^3}}{3}=C
$$
