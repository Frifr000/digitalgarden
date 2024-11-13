---
{"dg-publish":true,"permalink":"/4-Notas principales/Propiedad de indicadores/"}
---

Parte de la serie:[[3-Links o indices/Estadística\|Estadística]]
Las principales propiedades de los indicadores son :

1  Los estimadores deben ser Insesgados 

El estimador x̅ es un estimador insesgado de Mu si toda vez $E(x̅ )=\mu$ .

Ejemplo: Consideremos una muestra aleatoria simple $X_{1},X_{2},X_{3}\dots Xn$ en la cual todos los ítems de la muestra son independientes entre si e idénticamente distribuidos. 

Entonces x̅ de la muestra será: 

$$
x{{^{-}}=} \\\sum_{i=1} ^{+\infty} \frac{x_{i}}{n}
$$

Por lo cual el valor esperado de x̅ será:

$$
E(x{{^{-}}})=E( \\\sum \frac{x_{i}}{n})
$$
y simplificando

$$
\frac{1}{n}\\\sum_{i=1} ^{+\infty} E(X_{i}) 
$$

Ya que los elementos de la muestra son independientes e idénticamente distribuidos el valor esperado de cada ítems va a ser Mu (yo tampoco lo entiendo mucho pero Wilson ni se molesto en explicarlo).

Así que queda:


$$
\frac{1}{n}\\\sum_{i=1} ^{+\infty} \mu ----\to \frac{1}{n}n.u---\to\mu 
$$
Entonces el valor esperado de x̅ es mu, por lo cual el indicador es insesgado.

Propiedad 2: Eficiencia relativa de un estimador

Considerando que tengamos los estimadores $x{{^a}}$ y $x{{^b}}$ , el mejor estimador será el que posea la menor varianza.

Esta propiedad se relaciona con el error cuadrático medio , el cual consiste en la separación entre un estimador y su parámetro, escribiéndose como

$$
ECM=E(x̅-\mu){{^2}}
$$

distribuyendo el valor esperado y multiplicando el cuadrado queda

$$
ECM=E(x̅{{^{2}})-2\mu E(x̅)}+E(\mu{{^2}})
$$
y ya que es insesgado E(x̅)=Mu , que queda como

$$
ECM=E(x̅{{^{2}})-\mu{{^2}}}
$$
Que otra vez se re escribe como:

$$
ECM=E(x̅{{^{2}})-E(x̅){{^{2}}}=VAR}(x̅)
$$

Por este desarrollo entonces nos queda que el ECM es lo mismo que la varianza cuando el estimador es insesgado , si no es insesgado entonces quedara como:

$$
ECM=VAR(x̅)+Sesgo{{^2}}
$$
2 mini propiedades:

- Suficiencia: Mientras mas elementos de la muestras emplee un indicador mejor
- Consistencia: Cuando mayor tamaño de la muestra, mas se acerca el indicador al parámetro 


# Fuentes y referencias 

Literalmente solo yo, esto esta copiado de mi carpeta