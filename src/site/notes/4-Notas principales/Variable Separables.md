---
{"dg-publish":true,"permalink":"/4-Notas principales/Variable Separables/"}
---

## Variables separables 
Este es el método mas fácil , siendo aquel en el cual los diferenciables se pueden separar en cada parte de la ecuación con sus respectivas variables para así integrar todo. La ecuación que vimos arriba es una de variables separables por ejemplo. Su solución genérica es:

$$
y{^,}=P(x).Q(y) -\to \frac{dy}{dx}=P(x).Q(Y)\to \frac{dy}{Q(y)}=P(x).dx-\to \int \frac{1}{Q(y)}.dy=\int P(x).dx
$$
Acostúmbrense a ver este tipo de notación para todas las soluciones genéricas, porque la voy a usar mucho (en realidad es la que usa el libro pero bue). 

Ejemplos:

$$
3xy{^,}-x{^2}y=0\to 3xy{^,}=x{^2}y\to y{^,}=\frac{x{^2y}}{3x}\to \frac{dy}{dx}=\frac{x{^2y}}{3x}\to \frac{1}{y}dy=\frac{x{^2}}{3x}dx
$$

Continuado acá:

$$
\int \frac{1}{y}dy=\int \frac{x}{3}dx\to \ln (y)=\frac{1}{3}.\frac{x{^2}}{2}\to [\ln(y)=\frac{x{{^2}}}{6}+C]
$$
La solución general la voy a poner entre corchetes siempre. Es lo mismo de que lado pongan la constante.

Otros ejemplos:

EJ 3 de la guía de Venturini , sección variables separables:

$$
y.y{{^,}}=k\to y.\frac{dy}{dx}=k-\to dy.y=k.dx\to \int y.dy=\int k.dx\to [\frac{y{^2}}{2}=kx+C]
$$
EJ 7 de la misma sección:

$$
(3+x{^2})dy-2xy.dx=0\to(3+x{^2})dy=2xy.dx\to \frac{1}{y}.dy=\frac{2x}{3+x{^2}}.dx
$$
Queda la integral:
$$
\int \frac{1}{y}dy=\int \frac{2x}{3+x{^2}}.dx
$$
$$
Sustitución
$$
$t=3+x{^2}$    $dt=2x.dx$      $dx=\frac{1}{2x}.dt$ 

$$
\int \frac{2x}{3+x{^2}}.dx-\to \int \frac{dt}{t}\to \ln(t)\to \ln(3+x{^2})
$$
 $$
--
$$
$$
[\ln(y)=\ln(3+x{^2})+C]
$$
Se puede simplificar aun mas la respuesta si aplicamos propiedades de logaritmos

$$
\ln(y)=\ln(3+x{^2})+\ln C
$$
$$
\ln(y)=\ln[C.(3+x{^2})]
$$
$$
e{{^{\ln(y)}}}=e{{^{\ln[C.(3+x{^2})]}}}
$$
$$
y=C(3+x{^2})
$$
