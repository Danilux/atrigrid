
# Atrigrid

Version 1.0

#### English

This is a very simple substring attribute selector based reponsive grid *( Ok, that didn't sound simple )*, also mobile first ready, the whole grid has 6 units available for building column combinations, just remember they must add up to 6.

Choose a combination of column numbers to build the layout you need:

		6 creates 1 column spanning 6 units   |1|1|1|1|1|1|
		5 creates 1 column spanning 5 units   |1|1|1|1|1| |
		4 creates 1 column spanning 4 units   |1|1|1|1| | |
		3 creates 1 column spanning 3 units   |1|1|1| | | |
		2 creates 1 column spanning 2 units   |1|1| | | | |
		1 creates 1 column spanning 1 unit	  |1| | | | | | 

Atrigrid responds to three breakpoints ( mobile, tablet, desktop ), this allows you to build 3 layouts, one for each breakpoint, the measures set by default are:

	0 to 499px 	=  m for mobile
	500px to 991px = t for tablet
	992px to 1100px = d for desktop

So all you have to do is decide the number of columns combination you want for each layout at different breakpoint steps, and prefix those number with the breakpoint letter, finally suffix "cols":

So for example:

		// This will make a 1 column layout (boring) for mobile, tablet and desktop.
		<div class=m6-t6-d6-cols></div>

		// This will make a two column design, on mobile both columns will span the whole width, on tablet they will devide the space building 2 columns of 3 units each, and on desktop the first column spans 2 units and the second spans 4 units.
		<div class=m6-t3-d2-cols></div>
		<div class=m6-t3-d4-cols></div>


If you need your layout to adapt to the whole available viewport width instead of the 1100px max-width limit, just remove the `.grid-wrapper` class from your HTML.


  
  
 ***
  
  


#### Español

Esta es una simple retícula 'responsive' basada en selectores de atributo substring *( Ok, eso no sono simple)*, además utiliza la metodología mobile first, la retícula completa tiene 6 unidades disponibles para construir combinaciones de columnas, solo recuerda que deben sumar hasta 6.

Elige una combinacion de numero de columnas para construir la composición que necesites:

		6 crea 1 columna ocupando 6 unidades  |1|1|1|1|1|1|
		5 crea 1 columna ocupando 5 unidades  |1|1|1|1|1| |
		4 crea 1 columna ocupando 4 unidades  |1|1|1|1| | |
		3 crea 1 columna ocupando 3 unidades  |1|1|1| | | |
		2 crea 1 columna ocupando 2 unidades  |1|1| | | | |
		1 crea 1 columna ocupando 1 unidades  |1| | | | | |

Atrigrid responde a tres breakpoints ( Móvil, Tablet, Escritorio ), esto permite que construyas tres composiciones, una para cada breakpoint, las medidas fijadas por defecto son:

		0 a 499px  = m para movil
		500px a 991px = t para tablet
		992px a 1100px = d para escritorio

Así todo lo que tienes que hacer es decidir el numero de combinaciones de columnas que quieres para cada composición en los diferentes breakpoints, y prefijar esos números con la letra de breakpoint, finalmente sufija "cols":

Asi por ejemplo:

		// Esto creara 1 composición de 1 columna (aburrido) para móvil, tablet y escritorio
		<div class=m6-t6-d6-cols></div>

		// Esto creara un diseño de 2 columnas, en móvil ambas columnas ocuparan todo el ancho, en tablet se dividiran el espacio construyendo 2 columnas de 3 unidades cada una, y en escritorio la primera columna ocupara 2 unidades y la segunda ocupara 4 unidades.
		<div class=m6-t3-d2-cols></div>
		<div class=m6-t3-d4-cols></div>


Si necesitas que tu composición se adapte a todo el espacio de ancho disponible de la ventana del navegador en lugar de limitar a 1100px como ancho máximo, solo quita la clase `.grid-wrapper` de tu HTML.

