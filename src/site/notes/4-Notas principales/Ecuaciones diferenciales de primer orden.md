---
{"dg-publish":true,"permalink":"/4-Notas principales/Ecuaciones diferenciales de primer orden/"}
---

# Introducción

Bueno este es el tema mas jodido, por bastante. No es un tema difícil per se, sino que es increíblemente largo (re lindo que lo dieron en las ultimas 3 clases) y cuya única forma de asimilar bien básicamente es haciendo ejercicios (a menos que podamos usar el celu en el examen xd). Este tema también es  casi todo lo que vamos a hacer en matemática para economistas (o como se llame ahora) por lo que tengo entendido, así que es bueno aprenderlo bien para después.  Por eso mismo todos los ejercicios que ponga acá para explicar van a venir de la guía de Venturini, que suele ser mas difícil y además esta toda resuelta paso a paso [acá](https://ncuba.duckdns.org/index.php/s/KEzjBifcT5oAEjB) . Para llegar a la parte de Ecuaciones diferenciales abran el menú a la izquierda del documento, pongan el modo donde les muestra todos los capítulos y búsquenlo ahí. 

![Pasted image 20241117011455.png](/img/user/0-Imagenes/Pasted%20image%2020241117011455.png)
<font size=2>Asi se ve </font>

Voy a poner cada método que este en el libro salvo algunos casos de nicho, porque en primer lugar no se que métodos dieron en clase y segundo es que ya lo conocemos a Hernández por tomar temas que no dio nadie.  En cada parte lo que voy a hacer es primero poner el ejemplo que se usa en el libro de Venturini para explicar y después voy a poner otro de la guía para reforzar un poco. Al final voy a poner un par de ejercicios de la guía para que en primer lugar podamos testear que tan bien podemos reconocer el método adecuado según cada estructura y segundo para practicar un poco las resoluciones que también son importantes. Consejo mío, no se confíen pensado que con solo leer lo entendieron todo y caigan así al parcial, porque sin practica es muy fácil confundirse en la resolución.  Con todo esto dicho, pónganse un poco de música de fondo o lo que los ayude a hacer este choclo un poco mas llevadero y vamos a ver este lio.

# Ecuaciones diferenciales

Las ecuaciones diferenciales son aquellas ecuaciones en las cuales se encuentran las derivadas de una/s  variable de la ecuación respecto a alguna de las otras variables presentes.  En criollo , son ecuaciones en las cuales hay derivadas , como por ejemplo:


$$
y{^,}-2xy=2y
$$

Acá es **fundamental** acordarse que las derivadas pueden ser re expresadas como los cocientes entre los diferenciales de las variables, o es decir:

$$
y{^,}=\frac{dy}{dx}
$$
Por lo cual estas son ecuaciones en las cuales al encontrarse las derivadas de las variables, también se encuentran sus diferenciales, por lo cual de ahí sale el nombre. 
Entonces la ecuación del principio se puede re expresar como:

$$
\frac{dy}{dx}-2xy=2y
$$
Suele ser conveniente hacer este cambio para resolver mas fácilmente los ejercicios , pero igual vamos a verlo mas detalladamente en cada caso.

Otros ejemplos de ecuaciones diferenciales:

$$
\frac{dy}{dx}=3xy 
$$
$$
y{{^,}}-2xy=3

$$
*Estas son ecuaciones diferenciales de primer orden y grado.*

Todas estas son ecuaciones diferenciales de primer **orden** porque aparece la derivada primera, si apareciera la derivada segunda, son  diferenciales de segundo orden, las cuales se resuelven de una manera completamente diferente (tranqui no hay tantos métodos para esas) y voy a poner en otro archivo porque este se haría muy extenso sino.  También son de primer **grado** porque la derivada de mayor orden están todas elevadas a la uno. 


$$
y{{^{,,}}}-2xy=3

$$
*Esta es una ecuación diferencial de primer grado* y segundo orden


$$
y{{^,{{^3}}}}-2xy=3

$$
Esta es una ecuación diferencial de tercer grado y primer orden

# Soluciones de ecuaciones diferenciales
<font size =2>Aca empieza lo groso</font> 

A diferencia de las funciones hechas por personas mas o menos cuerdas, las ecuaciones diferenciales no son numero, sino que son otras funciones. Lo que estamos buscando son todas las funciones cuyas derivadas cumplan la ecuación. Por ejemplo:

$$
y{^,}=x$$
Acá tenemos que encontrar todas las funciones cuyas derivadas sean x.
Su solución es 
$$
\frac{dy}{dx}=x
$$
$$
dy=x.dx
$$
$$
\int dy=\int x.dx
$$
$$
y=\frac{x{^2}}{2} +C
$$
Como ven en todos estos casos vamos a tener que integrar para despejar los diferenciales, lo que significa que las soluciones van a ir con una constante al fina. ==Acuérdense de poner la constante en la solución.==

A veces en vez de pedirnos la solución general (como la que esta arriba) nos van a pedir una solución particular, que es lo mismo pero con la constante evaluada en un punto. Tenemos que evaluar la función en el punto y despejar la constante. Por ejemplo. el caso anterior en (1;1) es:
$$
1=\frac{1}{2}+C
$$
$$
\frac{1}{2}=C
$$
Así que la solución particular en (1;1) queda como :

$$
y=\frac{x{^2}}{2}+\frac{1}{2}
$$
Solo tienen que poner el valor particular de las constante, el resto queda igual en su expresión genérica. 

Ahora que sabemos la estructura de las soluciones, vamos a ver lo métodos. 

[[4-Notas principales/Variable Separables\|Variable Separables]]

[[4-Notas principales/Homogeneas\|Homogeneas]]

[[4-Notas principales/Lineales\|Lineales]] 

[[4-Notas principales/Exactas\|Exactas]]

[[4-Notas principales/Factor integrante\|Factor integrante]]

[[4-Notas principales/Bernoulli\|Bernoulli]]

Tip: Todas las funciones que se pueden resolver como homogéneas también se pueden resolver como exactas/factor integrante, así que suele mejor resolverlas así porque las homogéneas son un dolor en el orto. Igual diría practicar un poquito de homogéneas por si acaso.

Estuve viendo parciales viejos y prácticamente lo único que toma Hernandez son ecuaciones lineales, así que si están cortos de tiempo quizás conviene solo estudiar esas, aunque se arriesgan a que si toma otra cosa están en bolas. 


Ahora si se fijaron todas las ecuaciones acá dejo ecuaciones diferenciales generales para practicar un poco (no las voy  a hacer acá). Es bueno acordarse que la mayoria se puede solucionar por varios métodos. Todas salen de la sección de generales de la guia de Venturini. Estos ejs seguramente sean de igual dificultad o mas difíciles que los que tomen en el parcial: 

1)
$$
y{^,}+2xy=4x
$$
5)
$$
\frac{dy}{dx}=\frac{1+y{^2}}{(1+x{^2})xy}
$$
6)
$$
y{^,}=\frac{\ln(x{^2}+1)}{y{^3}}
$$
10)

$$
(3xy{^2}+8x{^2})dx+2x{^2}y.dy
$$
14)
$$
(x{^4}+y{^4})dx-xy{{^3}dy=0}
$$


