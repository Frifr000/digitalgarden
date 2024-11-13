---
{"dg-publish":true,"permalink":"/4-Notas principales/Poisson y otras variables/"}
---

-Parte de : [[3-Links o indices/Estadística\|Estadística]]
# **Variable Geométrica** 

![unnamed-chunk-46-1-1.png|600](/img/user/0-Imagenes/unnamed-chunk-46-1-1.png)
Estudia la probabilidad de la cantidad de veces que hay que observar un fenómeno hasta que aparezca un primer éxito, donde se define a la variable X como el numero de fracasos observados hasta que se obtiene el primer éxito.

Ejemplo: Se tira un dado de 6 caras tantas veces como sea necesario hasta que caiga en la cara de 1. ¿Cuál es la probabilidad de que esto se de por primera vez en la decima tirada? 

La geométrica tiene una chance p (probabilidad de éxito) y q(probabilidad de fracaso) que lógicamente es q=1-p. 

Las probabilidades en esta función se calculan con la formula 

$(q^{x-1}).p$

Entonces en este ejemplo la probabilidad se calcula como 

$P=1/6$ $Q=5/6$   $X=10$

$P(x)=(5/6)^{9}.1/6$  =0.03230

*Nota: Hay 2 maneras de calcular distribuciones geométricas, la forma que esta escrita acá la segunda forma, en la app aparece como Geométrica (II)*

Propiedades: 

Función de distribución: 
$$
\sum_{k=1}^{x}p(1-p)^{x}
$$
La cual converge y simplifica en :

$$
1-(1-p)^{x}
$$

Media: 
$$
E(X)=\frac{1}{p}
$$
Varianza:
$$
Var=\frac{1-p}{p^2}
$$
# Variable de Pascal (O Binomial negativa)


![binomial-negativa-Rstudio-3-1.png|750](/img/user/0-Imagenes/binomial-negativa-Rstudio-3-1.png)
<font size=0.5>jajajaj el grafico esta en brazuca</font>

Es otra variable Bernoulli, donde en este caso se estudia el numero de observaciones independientes (X) hasta lograr una r cantidad de éxitos donde r>1. Entonces la distribución se calcula como :

$$
BN={x-1\choose r-1}p^{r}(1-p)^{x-r}
$$
Media:

$$
E(X)=\frac{r(1-p)}{p}
$$
Varianza:

$$
E(X)=\frac{r(1-p)}{p^2}
$$

*nota: Como con la anterior distribución, en la app hay 2 formas de calcular estas distribuciones, lo usa la bibliografía (y como esta escrito acá) es la primera (NB(1)).

Aca no puse ejemplo porque la verdad lo hace todo la app y me da paja. 

# Distribución Hipergeométrica: 

Estas variables son para poblaciones que están divididas en 2 grupos excluyentes, en las cuales se toma una muestras sin reposición de n (no se debe confundir con N, el cual representa a la población total) elementos y se estudian las cantidades de estos que pertenecen a una de las clases(la cantidad de elementos que estemos buscando en la toda la población será M).

Entonces resumiendo, tenemos una población (N) , en la cual tenemos una cantidad de éxitos (M) y fracasos (N-M). De todas esa población , vamos a estudiar una muestra (n) ==**sin reposición**==
y calcular la probabilidad de encontrarnos con una X cantidad de éxitos (M) en la muestra.
![Pasted image 20241111190610.png|450](/img/user/0-Imagenes/Pasted%20image%2020241111190610.png)
<font size=0.5>Fuente de la imagen: Yo</font>
Una vez entendido esto podemos ir a la función de probabilidad que tiene la estructura 

$$
P(X)=\frac{{M\choose X}{N-M\choose n-X}}{N\choose n}
$$


Ejemplo:

En una caja hay 5 pelotas blancas y 7 negras. Se toma un puñado de 3 bolillas (sin reposición). ¿Cuál es la probabilidad de que 2 sean blancas?  

N=12   n=3  M=5 X=2

$$
P(X)=\frac{{5\choose 2}{12-5\choose 3-2}}{12\choose 3}

$$
Que simplificado pasa a ser :


$$
P(X)=\frac{{10}{.7}}{220} = \frac{70}{220} = 0,31818
$$

Media: 

$$
E(X)=n\left( \frac{M}{N} \right)
$$
Varianza:

$$
E(X)=n\left( \frac{M}{N} \right).\left( 1-\frac{M}{N} \right).\left( \frac{N-n}{N-1} \right)
$$

# Variable Exponencial: 

![Exponential_pdf.svg.png](/img/user/0-Imagenes/Exponential_pdf.svg.png)

La distribución exponencial es una distribución que depende del proceso de Poisson , que consiste en un compuesto de eventos discretos que son independientes en el espacio-tiempo. El proceso de Poisson se puede dividir en n subintervalos , dentro de los cuales a lo sumo se puede producir 1 evento. Es decir, que en cada subintervalo n se pueden dar 1 o 0 eventos. 
Entonces, ahora asumamos que en promedio se producirán $\lambda t$ eventos en el intervalo de tiempo t, siendo Lambda la tasa unitaria de ocurrencia del proceso de Poisson. 

Con todo esto, pasamos a la distribución exponencial , la cual mide la probabilidad de que pasen una X cantidad de  intervalos de tiempo (X remplaza acá a la t en la formula $\lambda t$) para que ocurra el próximo éxito de Poisson.

Su función de densidad tiene la forma:

$$
f(x)=\lambda e^{-\lambda x}
$$

donde lambda y x >0.

Media:

$$
E(X)=\frac{1}{\lambda}
$$
Varianza:

$$
Var(X)=\frac{1}{\lambda^2}
$$

Ejemplo:

 La duración de un cierto componente eléctrico es una variable aleatoria exponencial de media
1000hrs.
a- ¿Cuál es la probabilidad de que dicho componente dure más de 200 hora?

En este ej dicen que E(X)=1000, lo cual al despejar Lambda nos da que  $\lambda=\frac{1}{1000}$ . Si metemos esto en la app junto a  x=200, nos da que la probabilidad de X>200 es 0.81873.

# Variable de Poisson:
![Poisson_pmf.svg 1.png|450](/img/user/0-Imagenes/Poisson_pmf.svg%201.png)

La variable de Poisson funciona un poco como una exponencial a la inversa donde en vez de medir cuanto tiempo/longitud se tiene que recorrer para que suceda x, en estas variables de mide cuantas veces puede darse x en una cantidad determinada de tiempo/longitud.

Su función de distribución es :

$$
f(x)=\frac{e{^\lambda}\lambda{{^x}}}{x!}
$$

Media:

$$
E(X)=\lambda
$$
Varianza:

$$
Var(X)=\lambda
$$

Ejemplo:

En un proceso de fabricación de película fotográfica aparecen por término medio
1 defecto de cada 20 metros de película. Si la distribución de defectos es Poisson,
calcular la probabilidad de 6 defectos en un rollo de 200 metros de película.

Acá nos dicen que nuestro parámetro ($\lambda$) es 1 por cada 20 metros, pero ya que nos piden calcular sobre 200 metros de película, entonces el valor de lambda sobre todo el recorrido es 10. Si ponemos eso en la app junto a x=6, entonces nos dará que la probabilidad es 0,6306.



Fuentes/Referencias:

<font size=6>Yo</font>

Distribución geométrica : https://es.wikipedia.org/wiki/Distribuci%C3%B3n_geom%C3%A9trica

Distribución de Pascal: https://es.wikipedia.org/wiki/Distribuci%C3%B3n_binomial_negativa

Distribución Hipergeométrica: https://es.wikipedia.org/wiki/Distribuci%C3%B3n_hipergeom%C3%A9trica

Distribución Exponencial: https://es.wikipedia.org/wiki/Distribuci%C3%B3n_exponencial#Ejemplo

Distribución de Poisson: https://es.wikipedia.org/wiki/Distribuci%C3%B3n_de_Poisson

Lo que pude reconstruir del ppt del orto que hizo Wilson 

Todas las imágenes salvo la de hipergeométrica afanadas de Wikipedia o google imagenes.  