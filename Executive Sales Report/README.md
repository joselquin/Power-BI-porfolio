# Executive Sales Report

Este trabajo corresponde a mi propuesta para el Challenge 1 de la web Enterprise DNA, prestigiosa web de formación y foro de Power BI. Cada 2 semanas, se lanza un reto con una base de datos para la que hay que proponer una solución que muestre los aspectos indicados en cada uno.

En este caso, se trata de una base de datos de ventas de una empresa durante varios meses. Se trata de elaborar un informe ejecutivo para el Comité de Dirección que muestre la evolución de ventas y otros aspectos que puedan interesar a los directivos.

La base de datos tiene varias fact-tables:

* Apuntes de Ventas
* Localizaciones de las tiendas
* Productos
* Equipo de Ventas 

He creado un informe con 4 páginas:

1.- General
	- Se muestra una información global de las ventas, costes, márgenes y % de margen. 
	- Se puede seleccionar el periodo de tiempo a considerar. 
	- También se muestra una evolución de cada concepto a través de los meses.
	- Se muestra un top 3 de los productos vendidos, el equipo de ventas y la localidad.
	- Para cada uno de estos últimos conceptos, se puede seleccionar el mostrar el dato de ventas, el de costes o el de margen. 
	- Por último, aparece un selector para navegar cómodamente entre las 4 páginas (se repetirá el mismo selector en las otras tres).

2.- Productos.
	- Para todas las visualizaciones de esta página, se puede elegir el mostrar la cifra de ventas, la de costes o la de margen a través de un selector. Esto permite mostrar un panel muy limpio, pero disponer de mucha información.
	- Se muestra una gráfica de evolución a través de las semanas, con una línea de tendencia y un forecast para las próximas 3 semanas.
	- Se muestra un mapa con la distribución de estados y su nivel de ventas, costes o márgenes en el perido considerado. Si se hace click en cualquiera de los estados, los demás paneles mostrar´´an los datos correspondientes a ese estado. Si se pasa el cursor por encima de un estado, se muestran los valores en una ventana flotante.
	- Por último, se muestran los 5 productos con mejores ventas y los 5 con peores ventas. Se da la circunstancia de que los rankings proceden todos de las mismas medidas de Power BI. El número de valores mostrados (3 en la principal, 5 aquí, 10 en la página de Equipo de Ventas o 7 en la de Localizaciones) se elije a través de un selector oculto en cada página.

3.- Equipo de Ventas. 
	- Aquí mostramos igualmente una evolución semanal con una línea de tendencia y un forecast a 3 semanas (calculado mediante regresión lineal).
	-  En el mapa tenemos las 4 regiones de EEUU, aunque podemos seleccionar también cada estado y ver sus valores de ventas, costes, margen y % de margen si pasamos el cursor por encima de cada uno.
	- También se muestran los 5 mejores equipos por ventas y los 5 peores.
	- Pero en este panel, tenemos un menú que se abre pulsando sobre el icono disponible a la izquierda, con el que se permite filtrar todo los datos anteriores por uno o más productos, equipo de ventas o estado, lo que da muchísima versatilidad a esta página.

4.- Localizaciones.
	- Aquí tenemos una medida del nivel de ventas por cada $ de ingreso de la zona considerada. Nos permite hacernos una idea de cómo estamos aprovechando el mayor o menor nivel de ingresos de la zona considerada.
	- Se hace una segmentación de las distintas poblaciones en tres zonas consideradas como de bajo, medio y alto nivel por sus datos de rentabilidad y se muestra el nivel de ventas en cada una. Si pulsamos sobre el icono "i", aparece una ventana emergente con las 7 localidades con menor nivel de rentabilidad.
	- También se muestran sendos gráficos de barras con las 7 localidades con mejor nivel de ventas y las 7 copn peor nivel.
	- También se muestra un gráfico de sectores con el top 7 por estados y el de regiones de EEUU.
	- Mostramos igualmente los datos globales de ventas, costes, margen y % de margen según los filtros seleccionados.
	- Estos filtros, igual que en la página de Equipo de Ventas, pueden seleccionarse en la ventana emergente que aparece al pulsar sobre el icono disponible en la izquierda del panel. En este caso, se puede filtrar por productos, ciudades, regiones y estados.


Por tanto, hay varias formas de llegar a la misma información, pero desde un punto de vista diferente, lo que permite mostrar diferentes historias o que la dirección navegue por los paneles viendo las distintas perspectivas de los datos.

En el caso de un analista, la idea sería no meter ningún filtro, describir la historia que cada panel muestra, centrándose en los puntos globales de mejora (peores productos, peores equipos de venta y peores localidades). Para ahondar más en cada uno de estos aspectos mejorables, ya si podríamos valernos de los filtros.
