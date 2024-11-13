---
{"dg-publish":true,"permalink":"/4-Notas principales/Regresión Lineal/"}
---

-Decimos que hay una relación lineal entre las variables independientes x e y  si en un diagrama de puntos dispersos las observaciones conjuntas de ambas variables tienden a estar concentradas alrededor de una linea recta.  Para medir la fuerza de la relación lineal de una muestral, una medida descriptiva útil es el coeficiente de correlación muestral, el cual tiene la estructura:

$$
r=\frac{S_{xy}}{S_{x}S_{y}}
$$
donde $Sxy$ :

$$
Sxy=\frac{\sum (x_{i}-x{{^-}})(y_{i}-y{{^-}})}{n-1}
$$
Esta función también sirve para contrastar la hipótesis de que no existe una relacion lineal en la población entre variables aleatorias , o en otras palabras 

$H_{0}=\rho=o$

Entonces esta hipótesis sostiene que NO hay una relación lineal entre las variables. Se puede demostrar (pero no lo voy a hacer acá ) que cuando $H_{0}$ es nula  y las variables aleatorias siguen una distribución normal conjunta, la variable aleatoria:

$$
t=\frac{r\sqrt{ (n-2) }}{\sqrt{ (1-r{{^2}}) }}
$$
sigue una distribución student con t-2 gl. Esta ecuación entonces será la que usemos para probar correlación.

### Casos de resolución: 

En todos los casos vamos a plantear 

$H_{0}=\rho=o$

y lo que variara será nuestra H1

Si 

$H_{1}:/\rho>0$

entonces 

Rechazar $H_{0}$ si 

$$
\frac{r\sqrt{ (n-2) }}{\sqrt{ (1-r{{^2}}) }}>t

$$
Si 

$H_{1}:/\rho<0$

entonces 

Rechazar $H_{0}$ si 

$$
\frac{r\sqrt{ (n-2) }}{\sqrt{ (1-r{{^2}}) }}<-t

$$
Si 

$H_{1}:/\rho≠0$

Entonces se puede usar cualquiera de los 2, aunque el t usado debe ser con el a/2

Ejemplo:

Un equipo de investigaci6n estaba intentando averiguar si el riesgo político existente en
los paises esta relacionado con su inflaci6n. En esta investigaci6n, se realiz6 una en-
cuesta a analistas del riesgo político que permiti6 elaborar una puntuaci6n media del
riesgo político de 49 paises (los datos proceden del estudio mencionado en la referencia
bibliografica 2).

Solución
Cuanto mas alta es la puntuacion, mayor es el riesgo politico. La correlacion muestral
entre la puntuaci6n del riesgo político y la inflación de estos paises era de 0,43.

Tenemos una estructura (la da ya planteada la consigna)

$H_{0}:\rho=o$
$H_{1}:/\rho>0$

Por lo cual para verificar la correlacion deberemos ver si 

$$
\frac{r\sqrt{ (n-2) }}{\sqrt{ (1-r{{^2}}) }}>t
$$
con n=49 y r=0.43

Ahora entonces calculamos 

$$
\frac{0.43\sqrt{ (47) }}{\sqrt{ (1-0.43{{^2}}) }}>t_{47gl,0.05}
$$
Lo que queda:

$$
3,265>1,67793
$$
Como vemos la desigualdad se verifica, por lo cual tenemos pruebas para decir que a 5% de significación, $H_{0}$ no se verifica, por lo que hay un grado de correlación lineal entre las variables.

Ahora para resolver mejor cualquier ejercicio acá dejo lista de todas las formulas que serian necesarias:


$$
r=\frac{Cov(xy)}{\sigma_{x}\sigma_{y}}
$$

donde 

$Var(x)=E(X{^2})-E(X){^2}$
$Cov(xy)=E(xy)-E(X).E(Y)$
y obviamente $E(X)=\frac{Suma_{x}}{n}$


# Rectas de regresión 

La ecuación de la recta de regresión de  y sobre x es 

$$
Y=A+Bx 
$$
y esta es una ecuación que representa la relación lineal entre la variable Y y la variable x, siempre y cuando haya una relación lineal entre las 2 funciones en primer lugar lógicamente. Esta función nos dará el valor esperado de Y para un x dado. Para calcular A y B se usa el criterio de mínimos cuadrados (SCE), e el cual se minimizan los cuadrados de la sumatoria de la función original (no pregunten) hasta llegar ==al sistema de ecuaciones normales== , que consiste en:

$$
\sum Y=nA+B/\sum x
$$
$$
\sum xy=A/\sum x+B/\sum X{{^2}}
$$

Entonces una vez establecido este sistema podemos despejar A y B por sustitución y con eso armar la función de regresión. Obvio que esto puede ser tremendo lio, así que también hay formas alternativas de calcular A y B, estas siendo:

$$
B=\frac{Cov(xy)}{var(x)}=r{\frac{\sigma_{y}}{\sigma_{x}}}
$$
**Nota: Esta fracción también se conoce como el coeficiente de regresión.** 
y 


$$
A=E(Y)-B.E(X)
$$
Alternativamente, gracias al criterio de mínimos cuadrados,  la ecuación de la recta de regresión también se puede re-expresar con la forma 

$$
Y= E(Y)-B(X-E(X))
$$
# Resumen:

Si en el examen toman un ejercicio de regresión lineal, entonces (a menos que ya lo aclare la consiga) hay que empezar con la prueba de hipótesis para fijarse si hay una relación lineal entre las variables, y si hay entonces ahí se puede pasar al planteo de las ecuaciones de regresión. 

# Métodos y supuestos de mínimos cuadrados (solo en caso que lo tome en el teórico)

![Pasted image 20241113015722.png](/img/user/0-Imagenes/Pasted%20image%2020241113015722.png)
![Pasted image 20241113020005.png](/img/user/0-Imagenes/Pasted%20image%2020241113020005.png)

# Fuentes:

Yo
El apunte de Regresión lineal del campus: https://economicasuba.sharepoint.com/sites/Matematica/AULA-199153/Material%20teoria/Apunte%20de%20correlaci%C3%B3ny%20regresi%C3%B3n%20.pdf
