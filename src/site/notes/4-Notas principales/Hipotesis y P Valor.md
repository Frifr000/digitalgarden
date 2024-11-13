---
{"dg-publish":true,"permalink":"/4-Notas principales/Hipotesis y P Valor/"}
---

Parte de : [[3-Links o indices/Estadística\|Estadística]]
--
# Prueba de Hipótesis 


En este curso, las hipótesis estadísticas son suposiciones sobre atributos paramétricos de una población determinada  (EJ:$\mu$ de una población es igual a cierto valor). Nunca podremos saber con plena certeza la veracidad de una hipótesis , a menos que examinemos la población entera. 

La estructura general de estos ejercicios consiste en plantear 2 hipótesis , una nula $(H_{0})$ y una alternativa $(H_{1})$. $H_{0}$ será la hipótesis que sostenga el enunciado principal del ejercicio(la cual deberá ser rechazada o confirmada), mientras que $H_{1}$ será la hipótesis que quedara verificada si $H_{0}$ es rechazada.

Ejemplo: se necesita decidir si una máquina de llenado de botellas de gaseosa debe ser
apartada para mandarla a arreglar o no. Se la apartará en caso de que la media real de llenado
sea diferente a 2,25 litros.

En este caso las hipótesis serian:

$H_{0}$=La media es igual a 2,25 litros
$H_{1}$=La media no es igual a 2,25 litros.

## Errores

Ya que nunca tendremos plena certeza acerca de la veracidad de $H_{0}$ ,podemos cometer ciertos errores al decidir erróneamente:

**Error tipo 1:**

Este es el error cometido cuando se rechaza $H_{0}$, siento esta realmente verdadera. La probabilidad de cometer un error tipo 1 (llamada error de significación) esta dada por la ecuación: 

$$
a=P(Error_{1})=P(RechazarH_{0}/H_{0}escierta)
$$
Entonces la probabilidad de error tipo 1 pasa a ser la a que titulizábamos en intervalo de confianza, la cual también en estos casos será fijada por el investigador. 

**Error tipo 2:**

El error tipo 2 es el inverso del tipo uno, siendo este :

$$
\beta=P(Error_{2})=P(ConfirmarH_{0}/H_{0}esfalsa)
$$

**Potencia:**

Se define como la potencia de la prueba al complemento de $\beta$ , es decir $1-\beta=Potencia$, la cual básicamente mide la efectividad de la prueba.

Idealmente, conviene que ambos tipos de erros sean lo mas pequeños posible, ahora bien, muchas veces si uno quiere disminuir la chance de un error, deberá aumentar la chance del otro. La única forma de verdaderamente disminuir la chance de ambos erros es aumentando $n$. 

(Esto copiado directo de la biblio)

Entonces al formular $H_{0}$ y $H_{1}$ se deben tener en cuenta 3 afirmaciones generales:

1) La hipótesis nula es la hipótesis de "no diferencia". En términos prácticos esto quedará
explicitado en la afirmación de que la igualdad forma parte de H0.
2) Se ha de procurar detectar o fundamentar la hipótesis alternativa. Es por esto que se
denomina a la afirmación hecha bajo la Ha “hipótesis de investigación”.
3) Las hipótesis estadísticas se formulan siempre con la esperanza de que sea posible rechazar
H0. De modo que la prueba de hipótesis tendrá dos resultados posibles que son
mutuamente excluyentes:
a) Rechazar H0. con probabilidad α de hacerlo cuando H0 es cierta.
b) No rechazar H0.
# Resolución propiamente dicha de estos ejercicios:


Entonces en todos estos ejercicios los enunciados nos van a marcar cuales son los tipos de hipótesis que tenemos que establecer, existiendo 3 estructuras generales para estas:

### Planteo de cola por izquierda: 

Estos planteos se hacen en ejercicios como :

Un fabricante de galletas produce paquetes en los cuales el peso impreso en los paquetes es
de 500 gramos. Pero el contenido real en gramos es una variable aleatoria normal con desvío
de 5gr. El fabricante, afirma que la media de esa variable peso de cada paquete es μ=500
gramos con un desvío estándar de 5 gramos. Se desconfía de la afirmación del fabricante
acerca de que μ=500 gramos. Se quiere analizar si en realidad el peso promedio de los
paquetes ==es inferior== a 500 gramos.

Acá entonces el planteo de nuestras hipótesis tendrá la estructura:

$$
H_{0}:\mu=500
$$
$$
H_{1}=\mu<500
$$
Resolución:

Acá la consigna no nos da ningún tipo de error de significación, por lo cual vamos a fijarlo nosotros, decidiendo arbitrariamente que $a$=5% (usualmente cualquier valor entre 10% y 1% esta bien). 

El ejercicio sostiene que la variable aleatoria será  es una normal con desvió de 5, por lo cual tendrá la forma:

$$
\frac{X^{-}-\mu}{\frac{\sigma}{\sqrt{ n }}}  
$$
Esta aproximándose a la normal estándar a medida que n se acerca a +$\infty$ gracias al TCL.

Remplazando ahora con los valores de la consigna:

$$
\frac{X^{-}-500}{\frac{5}{\sqrt{ 100 }}}  
$$
Como ven cambiamos $\mu$ por 500, ya que lo que estamos buscando es verificar si $H_{0}$ ($\mu$ =500) es verdadera. Para eso entonces tendremos que comparar la función de prueba con  un intervalo real que determinara los valores para los cuales $H_{0}$ es falsa, el cual llamaremos region critica. La estructura de la region critica varia acorde a la hipótesis alternativa. En este caso (Cola por izquierda) la region critica tendrá la estructura: 

$$
(-\infty;z_{c})  
$$
Siendo Zc la region de la variable normal estándar que acumula un área $a$ (en este caso 0.05) a su izquierda, viéndose gráficamente como :

![Pasted image 20241112175643.png](/img/user/0-Imagenes/Pasted%20image%2020241112175643.png)


Si lo calculamos en la app nos da que $Zc=-1.64485$ , por lo cual nuestra zona de rechazo queda como 

$$
(-\infty;-164485)  
$$
Suponiendo ahora que 𝑋̅ = 497,3 (nos lo da la consigna el dato), entonces remplazamos en la f de distribucion:


$$
\frac{497.3-500}{\frac{5}{\sqrt{ 100 }}}  
$$

Si esta fracción da un numero que esa entre $(-\infty;-164485)$ , entonces $H_{0}$ queda rechazada, caso contrario, $h_{0}$ se considera valida con la información disponible. Resolviendo:

$$
\frac{497.3-500}{\frac{5}{\sqrt{ 100 }}}  =-5,4
$$


Ya que $-5,4\in(-\infty;-164485)$ , $H_{0}$ queda rechazada a 5% de significacion.

### Planteo de cola por derecha:

El resto de los procedimientos son los mismo, salvo que varia nuestra region critica:

Se estudiaron 40 observaciones de aceite crudo de determinado proveedor con el fin de
detectar la presencia del níquel. Si en 5 de dichas muestras se observó la presencia de níquel
¿podemos creer al proveedor cuando asegura que a lo sumo el 8% de las veces encontraremos
níquel?
Este caso es uno de proporción, en el cual ahora tenemos que acercarnos por derecha a la region critica. Las hipótesis serán:

$H_{0}:p=0.08$
$H_{1}:P>0.08$

Ya que es proporción se calcula de la misma forma que la media pero remplazando en la ecuación:

$$
\frac{{P^{-}-P}}{\sqrt{ \frac{PQ}{n} }}  \notin (Z_{c};+\infty)
$$
Y ya que N>30, podemos aproximarla a una normal por TCL. Debido a que este planteo de cola por derecha , la region critica quedara inversa al ejercicio anterior, Zc calculándose gráficamente así 
![Pasted image 20241112181604.png](/img/user/0-Imagenes/Pasted%20image%2020241112181604.png)
<font size=2>Otra vez usamos a=5 porque no lo especifica la consigna</font>

Y si remplazamos todo queda :
$$
\frac{0,125-0,08}{\sqrt{ \frac{0,08.0,92}{40} }}=1.049\notin(1,645;+\infty) 
$$
Por lo cual $H_{0}$ no puede ser rechazada con un 5% de significación. 

# Hipótesis de 2 colas: 
Estas suelen ser las mas comunes.

Se desea contrastar con un nivel de significación del 5 % la hipótesis de que la talla media de
los hombres de 18 de un país es igual a180. Suponiendo que la talla sigue ley normal con
desviación de las tallas en la población vale 4. Formular las hipótesis y realizar la prueba a
partir de la siguiente muestra de n=15 hombres seleccionados al azar, cuyas alturas son:167
167 168 168 168 169 171 172 173 175 175 175 177 182 195.

$H_{0}=\mu=180$
$H_{1}:\mu≠180$

Si 𝑋̅ = 173,47, la ecuación planteada queda como (Para que $H_{0}$ no sea rechazada)

$$
\frac{173,47-180}{\sqrt{ \frac{4}{15} }}\notin (-\infty;-Zc)U(Zc;\infty)
$$
Entonces se resuelve igual que los otros ejercicios , salvo que el intervalo queda con la forma 
![Pasted image 20241112182826.png](/img/user/0-Imagenes/Pasted%20image%2020241112182826.png)
<font size=2>ACEPTO</font>

Si resolvemos queda :

$$
-6,32\in (-\infty;-1,96)U(1,96;\infty)
$$

Ya que -6,32 es parte de este intervalo, $H_{0}$ queda rechazada al 5% de significación. 


*Nota: En todos estos ejs la resolución fue con una distribución normal, pero si en algún ejercicio piden verificar una hipótesis de una variable con distribución desconocida o normal y n<30, entonces se resuelve con un student.*

# P Valor 

El P valor se define como la probabilidad de que un valor estadístico calculado sea posible dada una $H_{0}$ cierta. Si P valor es menor a $a$ , se rechaza $H_{0}$, en caso contrario no se rechaza. 
![Pasted image 20241112193624.png](/img/user/0-Imagenes/Pasted%20image%2020241112193624.png)

Ejemplo:
Una empresa de neumático s afirma que uno de sus productos dura en promedio al menos
28000km. Las pruebas con 64 neumáticos dan como resultado una duración media de
27.800km,con una desviación estándar de 1.000km. Bajo la normalidad de la duración de los
neumáticos, sé pide:
a) Comprobar si hay evidencia suficiente para rechazar la afirmación de la empresa, a un nivel
de significación del 5%
b) ¿Cuál es el p‐valor?
La formula del P-valor es 

P valor =P[Rechazar el estadístico muestral/H0 es cierta]

Y en este ejemplo las formulas quedan como

$$
H_{0}=\mu≥2800
$$
$$
H_{1}=\mu <2800
$$
Entonces el p valor se puede sacar como:

$$
P[\frac{X{{^-}}-28000}{125}<\frac{27800-28000}{125}]
$$
Lo que se reduce a 
$$
P[z<-1.6]=0.0548
$$
Entonces ya que el p valor es mayor a nuestras significación (0.05), no se puede rechazar la hipótesis nula. El P valor básicamente funciona como una forma alternativa para corroborar hipótesis, donde en vez de poner z1 y z2 en la app, ponemos z< numero que de la ecuación que verifica H0.

En casos donde se siga un modelo de 2 colas. se hace el mismo procedimiento pero con modulo

queda 

$$
Pvalor:2pr(z>|(\frac {X{{^{-}}-\mu}}{\sigma/\sqrt{ n }}|)
$$
![Pasted image 20241112203545.png](/img/user/0-Imagenes/Pasted%20image%2020241112203545.png)
<font size=2>Resumen para los 3 casos</font>

# Pruebas de hipótesis para diferencia de medias y varianza:

#### Poblaciones normalmente distribuidas e independientes con varianza conocida: 

Estos problemas siguen la estructura genérica de distribución:

$$
\frac{X{{^-}}-Y{{^-}}-\delta_{0}}{\sqrt{ \frac{S_{w}^{2}}{n_{w}}+\frac{S_{x}^{2}}{n_{x}} }}
$$
Donde Delta 0 es la constante a la que se igualan las medias según proponga $H_{0}$, la cual tranquilamente puede ser 0.

Ejemplo:

![Pasted image 20241112204616.png](/img/user/0-Imagenes/Pasted%20image%2020241112204616.png)
![Pasted image 20241112204641.png](/img/user/0-Imagenes/Pasted%20image%2020241112204641.png)

 
