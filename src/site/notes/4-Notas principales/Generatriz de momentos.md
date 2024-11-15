---
{"dg-publish":true,"permalink":"/4-Notas principales/Generatriz de momentos/"}
---

La función generadora de momentos de una variable aleatoria es una función a valores reales $M(t)$ (es decir que es en función de un numero real t y no x) que se calcula como el valor esperado de $e{{^{tX}}}$ , o en otras palabras:

SI x es discreta:

$$
M_{x}(t)=E(e{{^{tx}}})=\sum e{{^{tx}}p_{x}(x)}
$$

Si x es continua:

$$
M_{x}(t)=E(e{{^{tx}}})=\int {e{{^{tx}}}f_{x}(x)dx}
$$
siempre y cuando $t\in(-h,h),h>0$ (por lo que puede no existir la fgm), lo que es lo mismo que decir que Mx(t) sea diferenciable en 0 ( por si fuera poco ahora Hernández para a romper las bolas tmb).

Su nombre viene de que todos los momentos de X pueden ser obtenidos al derivar la funcion e igualar la derivada a 0.

![Pasted image 20241113150426.png](/img/user/0-Imagenes/Pasted%20image%2020241113150426.png)
<font size=2>Gracias por las imagenes legibles pelado pelotudo </font>

Demostración de condicion suficiente: 
![Pasted image 20241113150509.png](/img/user/0-Imagenes/Pasted%20image%2020241113150509.png)
<font size=2>Yo tampoco entiendo una sopa de esto pero peor caso se puede copiar asi como esta si lo pregunta </font>

Resolucion generatriz de una binomial:

![Pasted image 20241113150756.png](/img/user/0-Imagenes/Pasted%20image%2020241113150756.png)

Generatriz Poisson:
![Pasted image 20241113151247.png](/img/user/0-Imagenes/Pasted%20image%2020241113151247.png)
fgm exponencial:
![Pasted image 20241113151922.png](/img/user/0-Imagenes/Pasted%20image%2020241113151922.png)
fgm binomial negativa:

![Pasted image 20241113151318.png](/img/user/0-Imagenes/Pasted%20image%2020241113151318.png)
<font size=2>Cada vez mas alta calidad las imagenes </font>
FGM normal estandard:
![Pasted image 20241113151406.png](/img/user/0-Imagenes/Pasted%20image%2020241113151406.png)
Propiedades de la fmg:

![Pasted image 20241113151731.png](/img/user/0-Imagenes/Pasted%20image%2020241113151731.png)
![Pasted image 20241113151809.png](/img/user/0-Imagenes/Pasted%20image%2020241113151809.png)

Tabla general:
![Pasted image 20241113152907.png](/img/user/0-Imagenes/Pasted%20image%2020241113152907.png)

En caso de que pida calcular un momento en algun tipo de variable , se puede sacar de esta tabla , derivar y remplazar.

Coeficiente de asimetría de Fisher
Mide que tan asimétrica es una v.a y se calcula como:


$$
A_{s}=\frac{\mu{^3}}{\sigma{^3}}
$$
As>0 es asimetrica hacia la derecha
K<0 es asimetrica hacia la izquierda  
K=0 no es asimetrica 
## Curtosis:

La curtosis mide la concentración alrededor de la media de una v.a y  se calcula como 


$$
K=\frac{\mu{^4}}{\sigma{^4}}
$$


Donde 

K>3 es una distribución leptocurtica (mayor distribución que una normal)
K<3 es una distribución platocurtica  (menor distribución que una normal)
K=3 es una distribucion mesocurtica (misma distribución que la normal)