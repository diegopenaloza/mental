- Frontera de Producción
  id:: 61ee2013-ba01-4b4c-ba53-dc30f15e62e5
  collapsed:: true
	- La frontera de producción parte de la siguiente expresión
		- $$
		  \ln \left(q_{i}\right)=\beta_{0}+\sum_{j=1}^{k} \beta_{j} \ln \left(z_{j i}\right)+\left(v_{i}\right)-u_{i}
		  $$
		- Donde:
			- $ln(q_i)$: Es el logaritmo del numero de unidades producidas por la empresa , medido en unidades
			- $ln(z_{ji})$_: Es el logaritmo del nivel de uso de los insumos, es decir cuanto se ha usado de capital, cuanto se ha usado de trabajo y ase sucesivamente con los demás [[Factores de Producción]] que se tomen en cuenta, por lo general que construyen índices de cantidades para estimar estas variables.
- Frontera de Costos
  id:: 61edfb56-65bd-400b-b36f-3815b0c8f671
	- Teoría
	  collapsed:: true
		- Expresión Matematica
			- La frontera de costo parte de la siguiente expresión
			  id:: 61ee1ef1-069d-4085-a8d8-5d61c255b089
			- $$
			  \ln \left(c_{i}\right)=\beta_{0}+\beta_{q} \ln \left(q_{i}\right)+\sum_{j=1}^{k} \beta_{j} \ln \left(p_{j i}\right) \text { 㐲 } v_{i}+u_{i}
			  $$
			- Donde
				- $ln(c_i)$ : es el logaritmo del costo de la empresa medido en dólares
				- $ln(q_i)$: Es el logaritmo del numero de unidades producidas por la empresa , medido en unidades
				- $ln(p_{ji})$ : Es el logaritmo del precio de los insumos Capital, Trabajo, etc, medido en dólares a diferencia de la estimación de la ((61ee2013-ba01-4b4c-ba53-dc30f15e62e5))
		- Estimación
			- Interpretación de resultados
				- $$
				  \lambda=\sigma_{u} / \sigma_{v}
				  $$
				- Si $\lambda$ es mayor a uno , esto quiere decir que la desviación estándar debido a la ineficiencia es mayor que la desviación estándar debido a un componente idiosincrático o aleatorio, es decir la ineficiencia se debe mas a términos internos de la empresa
				- Si $\lambda$ es menor a uno la ineficiencia de la empresa esta dada por un componente aleatorio
				- ![image.png](../assets/image_1643001183951_0.png)
				- el sigma mu no mide directamente el parámetro de eficiencia, sino que tanto de costo mas esta añadiendo cada una de las empresas en su forma de producir
				- Cuando se estima la función de costo, no solamente tengo la eficiencia técnica sino también  tengo la eficiencia productiva, es decir la eficiencia técnica mas la asignativa
				- Mientras mayor sea el costo de eficiencia mas ineficiente soy, esto se da por que la empresa estaría produciendo de forma mas ineficiente , por lo tanto mas costosa, no lo esta haciendo al mínimo costo
	- Videos
		- [:video {:controls true :src "C:/Users/Diego/Documents/Apowersoft/Apowersoft Online Screen Recorder/20220117_131014.mp4" }]
	- Aplicación
		- Estimación de la Frontera de costos para el sector manufacturero de Ecuador
		  collapsed:: true
			- # 1. Datos
				- Los datos se obtuvieron de superintendencia de compañías, mismo que pertenece al sector manufacturero de Ecuador para el año 2017, los datos a utilizar son:
					- Costos: Como el total de costo de las empresas en el año
					- Ventas: El total de ventas que se genero en dólares en el año
					- Precio Laboral: Se tomo el sueldo junto con los salarios y demás remuneraciones
					- Precio del Capital: Se tomo el total de Activos fijos
				- # 2. Descripción de los datos
				- La base de datos contaba inicialmente con un tota de 49829 empresas, misma de la cual se eliminaron aquellas empresas que no contaran con registro de las variables utilizadas para la estimación, quedando así un total 1202  observaciones,  de las cuales se filtro el sector manufacturero. Dentro de este sector se busco aquellas empresas que cuenten con un activo fijo similar, por lo cual se generaron 4 bloques de empresas según su valor de activo fijo, esto ya que en la industria manufacturera uno de los principales aspectos es su alta inversión en activos fijos necesarios para la generación de productos. Al realizar la división menciona se seleccionamos  aquellas empresas que consten con  el segundo 25% de empresas  según sus Activos fijos, esto ya que el primer bloque presenta empresas que tiene como activos fijos valores de  $30 o similares, haciendo poco valido este primer bloque. En las graficas 1 y 2 se puede observar el principal motivo de la generación de bloques, la gran diferenciación de activos fijos de las empresas.
				- ![image.png](../assets/image_1643159885800_0.png){:height 330, :width 435}
				- ![image.png](../assets/image_1643165569826_0.png){:height 282, :width 427}
				- Una vez definido el conjunto de datos, se puede comenzar a obtener simples estadísticas exploratorias del mismo, en la tabla 1 se evidencia esto. Los datos para el sector manufacturero del bloque 2 generado  cuenta con un numero de 30 empresas. Mismas que en su conjunto tienen un promedio de Activos fijos de 208 mil dólares dólares
				- ![image.png](../assets/image_1643165534065_0.png){:height 74, :width 656}
				- Siendo la empresas con menor activos fijos  LOA Corporación y la de mayor valor de activo fijo Heladerías Confrunat, Como se puede apreciar, aquella de mayor activo fijo es una empresa que vende productos que requieren una gran cantidad de los mismo.
				- Procedemos a logaritmizar las variables que se usaran parar estimar la frontera de costos, permitiéndonos  esto una breve descripción de las relaciones entre las variables.
				- ![image.png](../assets/image_1643168342536_0.png){:height 474, :width 654}
				- Tratando de diferenciar y dar relevancia al bloque de empresas seleccionadas, comparamos el total de ingresos por ventas de todo el sector, en el que se puede observar en la grafica anterior  existe en general una relación directa entre el activo y las ventas, echo que se esperaba, sin embargo  como se puede observar en el grafico,  el valor de netas no siempre incrementa con mayores activos fijos, lo que nos podría dar leve indicio de que empresas en el mismo sector por mas activos fijos tengan, no se genera mayor valor de venta,, es preciso recordar que se esta usando los ingresos generados por ventas, tratando de excluir así ingresos de otra índole, como los financieros. Sin embargo en la siguiente grafica observamos la misma relación, pero en esta ocasión con los datos seccionados.
				- ![image.png](../assets/image_1643169427172_0.png){:height 487, :width 654}
				- La relación muestra un comportamiento casi lineal, por lo cual con las empresas seleccionadas se podría mencionar que un nivel de activos fijos no genera un nivel de ventas  mayor, siendo esto ineficiente, echo que en un  principio, nuevamente, no se podría generalizar por el numero de empresas observadas, pero es un punto de partida.
				- Por el lado de la varíale trabajo, se eligió como proxy los costos de sueldos y salarios, mismo que se establecen con intervención directa o indirecta en la producción.
				- ![image.png](../assets/image_1643171333536_0.png){:height 76, :width 656}
				- Es de interés mencionar  que existe una gran variación de los sueldos en los datos, ya que mientras  existen empresas que llegan al millón de dólares en estos costos de salarios, otras no superan los $ 1500.
				- Por ultimo revisamos la variable de mayor  relevancia en esta estimación, el costo, esta variable recoge los costos totales de producción de una empresa
				- ![image.png](../assets/image_1643171777200_0.png)
				- Como se observa en la tabla anterior, los costos pueden llegar a ser extremadamente altos  de hasta 12 millones de dólares. Sin embargo a diferencia de los Activos fijos, el costo total, muestra una relación  positiva con el numero de ingresos por ventas:
				- ![image.png](../assets/image_1643172015732_0.png){:height 473, :width 656}
			-
			- # 1. Obtención de Datos
				- Los datos se obtuvieron de superintendencia de compañías para el año 2017, las cuentas que se seleccionaron con sus respectivos códigos fueron ; Costos con el código 7991
			- # 3. Estimación de Frontera de Costos
				- Escogemos la estimación de modelo de función de costos, para esta estimación se seleccionó una distribución de tipo half-normal para el termino de eficiencia.
				- ![image.png](../assets/image_1643172949519_0.png){:height 337, :width 654}
				- Tras corree el modelo podemos decir que se rechaza la hipótesis nula que valora la  ineficiencia interna, esto es, existe una ineficiencia interna mayor que la ineficiencia externa y es estadísticamente significativa.
				- Analizamos ahora el total de las empresas estudiadas y como se comporta su ineficiencia mediante un histograma
				- ![image.png](../assets/image_1643236224353_0.png)
				- Como se puede aprecias un gran numero de empresas  muestra una ineficiencia, o mayor costo , de no gran tamaño, sin embargo existe una parte de estas que presenta ineficiencia de gran valor.
				- ![image.png](../assets/image_1643236372624_0.png)
				- La tabla anterior denota que existe una ineficiencia máxima de 51.475, valor que pertenece a la empresa PRODAL Procesadora de Alimentos. por otro lado la empresa que muestra menos ineficiencia es  DECOMUEBLES, con una ineficiencia baja de 1.081.
				- Sin embargo la ineficiencia se presenta algunos valores atípicos
				- ![image.png](../assets/image_1643237015967_0.png)
				- Analizando los datos se encontró que son 60 las empresas que tienen una ineficiencia realmente alta comparada con el resto.
				- ![image.png](../assets/image_1643237263391_0.png)
				- Como se muestra en la tabla anterior, de eliminarse estas 60 empresas,  muestran valores mas homogéneos en su ineficiencia, esto se realizo con el fin de poder establecer una media coherente de ineficiencia en el bloque manufacturero seleccionado, obteniendo así una ineficiencia promedio de  1,799  de las empresas en el sector manufacturero que  poseen activos fijos de entre 86 mil y  380 mil dólares .
			-
			-
-