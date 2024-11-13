---
{"dg-publish":true,"permalink":"/4-Notas principales/Intervalos de confianza/"}
---

Parte de :[[3-Links o indices/Estadística\|Estadística]]

# Intervalos de confianza
Los intervalos de confianza son un método para estimar parámetros dentro de un intervalo determinado , acorde a un grado de confianza especifico (por eso el nombre no),

La estructura general  de resolución de ejercicios de  intervalos de confianza siempre es la misma, pero las formulas especificas varían acorde a la consigna. 

# Intervalos de confianza para la media 
## 1er caso: Población normal y desvió típico conocido: 

En estos casos la muestra $X_{1},X_{2},X_{3}\dots Xn$ , al ser una muestra de una población normal es en si misma una variable normal, por lo tanto (por propiedad de las variables normales) su media aritmética (x̅) es también una variable con distribución normal que sigue la estructura :

x̅~$N(\mu;\left( \sqrt{\frac{\sigma}{N}} \right)$

El desvió sale de que x̅ $=\frac{X_{1}+X_{2}+X_3\dots Xn}{n}$ , por lo cual su varianza será

$$
Var\left( \frac{X_{1}+X_{2}+X_3\dots Xn}{n} \right)=\frac{1}{n{{^2}}}(varx_{1}+varx_{2}+varx_{3}\dots var_{xn})
$$
Que queda

$$
\frac{1}{n{{^2}}}.n\sigma{{^2}}=\frac{\sigma{{^2}}}{n}
$$
Con todo esto, pasamos al intervalo propiamente dicho, que tendrá la forma:

$$
[ z_{1}<\sqrt{ n }\left( \frac{x̅-\mu}{\sigma} \right)<z_{2}] =1-a
$$
Donde a el área total que buscamos el grafico de densidad , el cual varia acorde al grado de exactitud que buscamos (ej: si el grado es 95%, a es 0.05)

y Z1 y Z2 son

![Pasted image 20241111230250.png](/img/user/0-Imagenes/Pasted%20image%2020241111230250.png)

-z y z de esta imagen respectivamente

Despejando Mu;


$$
x̅-Z\left( \frac{\sigma}{\sqrt{ n }} \right)<\mu <x̅+Z\left( \frac{\sigma}{\sqrt{ n }} \right)
 $$
Ejemplo(no lo voy a copiar todo esto): 

 ![Pasted image 20241111225941.png](/img/user/0-Imagenes/Pasted%20image%2020241111225941.png)
 <font size=2>¿Por qué confiamos? Yo también me pregunto eso a veces la verdad </font>

## 2do caso: Población normal y desvió típico desconocido: 

En el caso que no conozcamos el desvió poblacional, podemos usar el desvió muestral (S) , aunque corremos el riesgo de ser mas inexactos. Para entender esto mejor vamos a ver la ecuación del recorrido total de un intervalo de confianza:

$$
2[Z\left( \frac{\sigma}{\sqrt{ n }} \right)]
$$
En el cual el termino entre corchetes representa el error ($\epsilon$). Por la forma de la fracción , mientras mayor sea nuestra población, menor será nuestro error.  Entonces , en poblaciones mayores a 30 podremos decir que la distribución de la población es aproximadamente normal, por lo cual podemos resolver como en el caso anterior, remplazando sigma por S. En el caso que la muestra sea menor a 30 , debemos usar el siguiente intervalo de confianza:

$$
[ t_{1}<\sqrt{ n }\left( \frac{x̅-\mu}{S} \right)<t_{2}] =a
$$

La principal diferencia es que usamos el desvió típico en vez del poblacional y que en vez de usar las z1 y z2 de la distribución normal, usamos la t1 y t2 de la distribución de student. La distribución de student es una distribución simétrica como la normal, con la función de densidad:


![Pasted image 20241111232615.png](/img/user/0-Imagenes/Pasted%20image%2020241111232615.png)
<font size=2>Ni siquiera voy a INTENTAR copiar eso</font>

La resolución es igual a la anterior, solo que en vez de usar la distribución normal de la app se usa la distribución de student. 

Entonces despejando Mu queda

$$
x̅-t_{1}\left( \frac{S}{\sqrt{ n }} \right)<\mu <x̅+t_{2}\left( \frac{S}{\sqrt{ n }} \right)
 $$


Ejemplo:


![Pasted image 20241111232933.png](/img/user/0-Imagenes/Pasted%20image%2020241111232933.png)


### Como obtener una muestra determinada para una longitud fijada:

En algunos ejercicios pueden pedir determinar el tamaño de muestra necesario para un intervalo de confianza con longitud ya fijada. La forma de resolver esos ejercicios es igualando la funcion de longitud a la longitud que nos pide la consigna (L) y despejando n :

$$
2Z\left( \frac{\sigma}{\sqrt{ n }} \right)=L
$$

Quedando:

$$
(\frac{2Z\sigma}{L}){{^2}}=N
$$
Ejemplo:


![Pasted image 20241112031909.png](/img/user/0-Imagenes/Pasted%20image%2020241112031909.png)

# Intervalos de confianza para la varianza en poblaciones normales


En el caso de la varianza , el procedimiento es parecido, pero ahora utilizamos el intervalo:

$$
P{\left[ X_{1-\frac{a}{2}}{^2}<(n-1)\left( \frac{S{{^2}}}{\sigma{{^2}}} \right)<X{{^2}_{_{\frac{a}{2}}}} \right]}=1-a
$$
Donde 

$(n-1)\left( \frac{S{{^2}}}{\sigma{{^2}}} \right)$ ~ X^2 con n-1 grafos de libertad. X^2 en este caso no es la variable elevado al cuadrado, sino que representa a la distribución Chi cuadrado, que es una distribución ==**no simétrica**==,por lo cual las x de cada lado van a ser completamente distintas en vez de solo varia en signo cómo antes.  La función de densidad de la distribución Chi cuadrado es :

![Pasted image 20241111234950.png](/img/user/0-Imagenes/Pasted%20image%2020241111234950.png)

Despejando sigma en el intervalo anterior nos queda :


$$
P\left[ \frac{(n-1)S{{^2}}}{X{^2}_{{\frac{a}{2}}}}<\sigma{{^2}}<\frac{(n-1)S{{^2}}}{X{^2}_{{{1-\left( \frac{a}{2} \right)}}}} \right]
$$
Ojo con que las X cambiaron de lugar, la mas grande ahora esta a la izquierda y la mas chica a la derecha(Se volvió fascista).

Ejemplo:


![Pasted image 20241111235537.png](/img/user/0-Imagenes/Pasted%20image%2020241111235537.png)
<font size=2>Gracias a dios que no tengo que copiar todo esto</font>

# IC para proporcion

Si el ejercicio nos pide calcular una proporción en vez de una media , entonces la estructura es 

$$
P{{^-}}-Z.\sqrt{ \frac{PQ}{\sqrt{ n }} }<p<P{{^-}}+Z.\sqrt{ \frac{PQ}{\sqrt{ n }} }
$$
Donde 
$$
P{{^{-}}=\frac{Numerodexitos}{n} }
$$
EJ:

![Pasted image 20241112030628.png](/img/user/0-Imagenes/Pasted%20image%2020241112030628.png)
<font size=2>Gallegos de Mierda</font>
# IC para diferencia de medias 

En el caso que un ejercicio pida un IC para la diferencia de medias, la estructura a seguir es :

Siendo $W{{^-}}$ y $X{{^-}}$ estimadores muestrales de las medias $\mu_{w}$ y $\mu_{x}$

Entonces el intervalo es (si n≥30)

$$
P[(W{{^-}-X{{^-})}}-Z_{1}.\sqrt{ \frac{S_{w}^{2}}{n_{w}}+\frac{S_{x}^{2}}{n_{x}} }<\mu_{w}-\mu _{x}<(W{{^-}-X{{^-})}}+Z_{1}.\sqrt{ \frac{S_{w}^{2}}{n_{w}}+\frac{S_{x}^{2}}{n_{x}} }]
$$

Si el IC cubre el 0, entonces se puede concluir que no hay demasiada diferencia entre las las medias.

Y si n<30, se cambia z por t de student:

$P[(W{{^-}-X{{^-})}}-t.\sqrt{ \frac{S_{w}^{2}}{n_{w}}+\frac{S_{x}^{2}}{n_{x}} }<\mu_{w}-\mu _{x}<(W{{^-}-X{{^-})}}+t.\sqrt{ \frac{S_{w}^{2}}{n_{w}}+\frac{S_{x}^{2}}{n_{x}} }]$

, pero además hay una dificultad agregada, ya que si no sabemos si los desvíos poblacionales son iguales, entonces los grados de libertad de los student tiene que ser calculados con la aproximación de Welch , el cual consiste en esta hermosa formula:


![Pasted image 20241112025537.png](/img/user/0-Imagenes/Pasted%20image%2020241112025537.png)
<font size=2>Ni en pedo copio eso saludos</font>

Ejemplo:
![Pasted image 20241112025626.png](/img/user/0-Imagenes/Pasted%20image%2020241112025626.png)
Como ven la aproximación de Welch dio 29 acá, así que en este ejercicio la t de student tiene 29 grados de libertad. Resolviéndose así :


![Pasted image 20241112025802.png](/img/user/0-Imagenes/Pasted%20image%2020241112025802.png)

Si se conocen las varianzas, entonces remplazan a las cuasi varianzas y si no se conocen pero si se puede asumir iguales entre si entonces el IC es el siguiente  

$$
P[(W{{^-}-X{{^-})}}-t.\sigma\sqrt{ \frac{1}{n_{w}}+\frac{1}{n_{x}} }<\mu_{w}-\mu _{x}<(W{{^-}-X{{^-})}}+t.\sigma\sqrt{ \frac{1}{n_{w}}+\frac{1}{n_{x}} }]
$$
que es un Student con nx+nw-2 grados de libertad. 

¿Cómo sabemos si los desvíos son iguales o no? Para eso podemos establecer un IC del cociente entre los cuasi desvíos que tiene la forma :

$$
I\left( \frac{\sigma{^2_{1}}}{\sigma{{^2}}_{2}} \right)=\left[ \frac{\frac{S{{{^2}_{1}}}}{S_{2}{^2}}}{F_{a/2;d_{1};d_{2}}};\frac{\frac{S{{{^2}_{1}}}}{S_{2}{^2}}}{F_{1-a/2;d_{1};d_{2}}}\right]
$$
Esto se llama prueba de Homocedasticidad y consiste en un intervalo de confianza el cual nos podrá decir si los desvíos son iguales o no. 


¿Qué distribución es F? No tengo ni la menor puta idea, probablemente falte esa clase, pero lo que importa es que aparece en la aplicación como F y se calcula muy parecido a las otras. En esta d1 y d2 son $n_{1}-1$ y $n_{2}-1$ respectivamente. Si el IC cubre uno, entonces se puede decir que los desvíos son iguales.


Ejemplo:
![Pasted image 20241112024308.png](/img/user/0-Imagenes/Pasted%20image%2020241112024308.png)

# Resumen:

En resumen , las resoluciones quedan como:


Intervalos para la media:

| $\sigma$    | n    |                                                                                                  |     |
| ----------- | ---- | ------------------------------------------------------------------------------------------------ | --- |
| Conocida    | -    | $x̅-Z\left( \frac{\sigma}{\sqrt{ n }} \right)<\mu <x̅+Z\left( \frac{\sigma}{\sqrt{ n }} \right)$ | 1   |
| Desconocida | n≥30 | $x̅-Z\left( \frac{S}{\sqrt{ n }} \right)<\mu <x̅+Z\left( \frac{S}{\sqrt{ n }} \right)$           | 2   |
| Desconocida | n<30 | $x̅-t_{1}\left( \frac{S}{\sqrt{ n }} \right)<\mu <x̅+t_{2}\left( \frac{S}{\sqrt{ n }} \right)$   | 3   |


En caso que la distribución no sea normal pero n>30, por Teorema central del limite se puede aproximar a una normal, se usa el intervalo 2. Si no es normal y n<30, entonces se debe utilizar el tercer intervalo.

Intervalo para la varianza

$\left[ \sqrt{(\frac{(n-1)S{{^2}}}{X{^2}_{{\frac{a}{2}}}}}<\sigma{}<\sqrt{\frac{(n-1)S{{^2}}}{X{^2}_{{{1-\left( \frac{a}{2} \right)}}}}} \right]$

IC para proporcion:

$$
P{{^-}}-Z.\sqrt{ \frac{PQ}{\sqrt{ n }} }<p<P{{^-}}+Z.\sqrt{ \frac{PQ}{\sqrt{ n }} }
$$


Diferencia de medias:

| $\sigma$                            | n    |                                                                                                                                                                                                             |     |
| ----------------------------------- | ---- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --- |
| Conocida                            | -    | $P[(W{{^-}-X{{^-})}}-Z_{1}.\sqrt{ \frac{\sigma_{w}^{2}}{n_{w}}+\frac{\sigma_{x}^{2}}{n_{x}} }<\mu_{w}-\mu _{x}<(W{{^-}-X{{^-})}}+Z_{1}.\sqrt{ \frac{\sigma_{w}^{2}}{n_{w}}+\frac{\sigma_{x}^{2}}{n_{x}} }]$ | 1   |
| Desconocida                         | n≥30 | $P[(W{{^-}-X{{^-})}}-Z_{1}.\sqrt{ \frac{S_{w}^{2}}{n_{w}}+\frac{S_{x}^{2}}{n_{x}} }<\mu_{w}-\mu _{x}<(W{{^-}-X{{^-})}}+Z_{1}.\sqrt{ \frac{S_{w}^{2}}{n_{w}}+\frac{S_{x}^{2}}{n_{x}} }]$                     | 2   |
| Desconocida                         | n<30 | $P[(W{{^-}-X{{^-})}}-t.\sqrt{ \frac{S_{w}^{2}}{n_{w}}+\frac{S_{x}^{2}}{n_{x}} }<\mu_{w}-\mu _{x}<(W{{^-}-X{{^-})}}+t.\sqrt{ \frac{S_{w}^{2}}{n_{w}}+\frac{S_{x}^{2}}{n_{x}} }]$                             | 3   |
| Desconocidas pero se asumen iguales | -    | $P[(W{{^-}-X{{^-})}}-t.\sigma\sqrt{ \frac{1}{n_{w}}+\frac{1}{n_{x}} }<\mu_{w}-\mu _{x}<(W{{^-}-X{{^-})}}+t.\sigma\sqrt{ \frac{1}{n_{w}}+\frac{1}{n_{x}} }]$                                                 | 4   |

Aproximacion de Welch (Necesaria para grados de libertad del caso 3)


 ![Pasted image 20241112025929.png](/img/user/0-Imagenes/Pasted%20image%2020241112025929.png)
 
 
 Si te aparece una diferente a cualquiera de estos casos, matate.

# Teorema central del limite:


El teorema central del limite es el teorema que sostiene que la suma de variables aleatorias independientes ($S_{n}$) con media y varianza finitas se aproxima a una distribución normal a medida que se acerca a +$\infty$ , siempre y cuando la suma de estas variables aleatorias sea lo suficientemente grande (≥30).

Pasándolo todo en limpio el teorema consiste en:

Si $X_{1}+X_{2}+X_{3}\dots Xn$ son muestras aleatorias de una población independientes e idénticamente distribuidas y $S_{n}$  su sumatoria,  con $E(Xi)$ convergiendo en $\mu$ y Var(Xi) convergiendo en $\sigma$ , ambas siendo finitas,  entonces se define que la función 

$Z_{n}=\frac{S_{n}-n\mu}{\sigma \sqrt{ n }}$

La cual  a medida que n---> +$\infty$  converge a la función de distribución estándar N(0;1) para cada numero real z ; o en otras palabras

$$
\\lim_{ n \to \infty } P\left( \frac{S_{n}-n\mu}{\sigma \sqrt{ n }}≤z \right)=\int_{-\infty}^{z} \frac{1}{\sqrt{ 2\pi }}e^{-x{{^2}}/2}dx  
$$
siempre y cuando n≥30. 



### Fuentes y Referencias:
<font size=6>Yo</font>
TCL:https://web.archive.org/web/20100602111757/http://www.math.csusb.edu/faculty/stanton/probstat/clt.html
Apuntes IC: https://economicasuba.sharepoint.com/sites/Matematica/AULA-199153/Material%20teoria/Apunte%20Intervalos%20de%20Confianza.pdf
Mis sueños


Es increíble como los únicos apuntes buenos son los que no escribió este tipo 