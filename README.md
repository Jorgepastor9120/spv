#Supermercado Virtual para el Comercio Local 
 
##Objetivo 
Ofrecer una plataforma web sencilla y directa que conecte de manera efectiva los comercios de alimentación locales con el pequeño consumidor, fijando como principal usuario objetivo a la propia población del barrio o ciudad. 
 
##Alcance 
Se trata de un modelo B2C que abarcará el ámbito de los productos de alimentación: 
* Carnicería y charcutería 
* Pescadería 
* Frutería (fruta y verduras) 
* Panadería, confitería y bollería 
La razón de elegir este ámbito tan concreto es porque se busca facilitar al cliente final la búsqueda y acceso a una gran variedad de productos alimenticios de alta calidad que por lo general no se encuentran en grandes o medianas superficies, y son los pequeños comercios especializados los que suelen ofrecerlos. 
En la plataforma no se incluirá ningún producto que contenga alcohol (cerveza, vino, destilados…) ¿Por qué? Me desmarcaría de la comida no sana (alcohol, productos "prefabricados", bollería industrial...), me centraría en la venta de productos de comercio tradicional (descritos arriba). Y no solo buscamos beneficiar al usuario final (que también). Sobre todo buscamos beneficiar al comercio local, dándole la opción de subirse al carro del comercio electrónico por un precio muy asequible y no quedarse atrás. 
Tiraría mucho también de productos artesanos (muchos comercios pequeños lanzan sus propios productos como pueden quesos, algunos dulces, postres, etc.) 
 
##Contexto 
Cada año el comercio electrónico cobra más importancia en el día a día del consumidor, y por supuesto así debe serlo también para los comercios, que deben adaptarse a las numerosas ventajas que ofrece, ya que de lo contrario puede suponer un lastre de consecuencias irreversibles, como ya se ha visto a lo largo de los últimos años por ejemplo con el sector de los productos multimedia. 
Pero quizás el sector donde más haya que centrarse para situarnos y poder ver la perspectiva a medio-largo plazo del modelo que se plantea es el de los comercios de comida rápida. Con plataformas como Just-Eat, que han logrado unificar la manera de pedir comida por Internet entre una gran variedad de pequeños y medianos comercios cercanos, multiplicando así el alcance a posibles clientes de cualquier comercio de este tipo, por pequeño que sea y esté donde esté. Como he dicho antes, también me desmarcaría de los comercios de comida rápida. 
Es también este último punto el que queremos resaltar como parte del contexto, debido a que las medianas y grandes superficies, respaldadas por grandes empresas están desplazando al pequeño comercio de la vida cotidiana, al punto que hoy en día cuesta encontrar este tipo de locales en barrios de nueva construcción, y cada vez más también en barrios donde antes era común que estuvieran. Pensamos que una de las principales razones es la dispersión geográfica y la falta de conocimiento de los consumidores sobre estos locales. Mediante esta idea se trata de solucionar ambos problemas. 
 
##Monetización 
Se plantean varios modelos diferentes de monetización: 
* Cobrar una cantidad mensual fija por cada producto que se suba. Podrá variar según el precio del producto, el tipo o incluso hacer descuentos por conjuntos grandes de productos. No variaría el precio según coste de producto. Una de las claves de esta plataforma es su sencillez y limpieza, sin letras pequeñas. De esa manera ya tendrías que estar explicando que si subes un producto determinado te puede costar más que subir otro. Esto es negativo. Me limitaría a 1 producto, 0,60€, sin más ni más. Muy fácil de entender para el típico charcutero de barrio que no entiende mucho de estas cosas. 
* Cobrar un porcentaje del precio de cada producto vendido a través de la plataforma. Esta opción se puede contemplar para casos donde se busque principalmente promocionar un catálogo de productos, y la venta se realice en la tienda física. Casi que descarto por completo los pagos en base a porcentaje, dan sensación de inseguridad, a mi personalmente las plataformas que cobran por % no me gustan nada. 
* Combinar ambas modalidades, reduciendo el coste de cada una. 
 
##Implementación 
Por un lado tendremos la plataforma web, donde el usuario final podrá mirar, comprar o reservar los productos (productos del día o frescos) de la ciudad o población en la que se encuentre. El cliente podrá recogerlos en tienda física o solicitar su transporte. 
El comercio tendrá el control en todo momento de los productos que tiene subidos, estadísticas, ventas, etc. (mediante la correspondiente sección privada en la web). 
Por otro lado, tendremos la aplicación móvil, con el mismo contenido que la tienda online, pero añadiendo notificaciones personalizadas para cada usuario con productos recomendados según unos parámetros previamente configurados por éste.  
El comerciante tendrá también la opción de añadir o eliminar productos él mismo desde esta aplicación de forma rápida y sencilla. 
Adicionalmente, otra versión web más ligera donde el usuario con poco acceso a internet puede mediante un formulario, solicitar una cesta recomendada a su correo electrónico (con la orden de pago). 
 
##PLATAFORMA WEB 
 
Previamente, hay que estudiar en que formato crear la web, con Bootstrap/php/js o con Web Components. En cualquier caso deberá ser una web muy rápida tanto en todo tipo de dispositivos, y especialmente orientada a móvil. Definitivamente me decantaría por Bootstrap/php/js, es algo que conocemos casi a la perfección y es perfectamente válido. 
 
Partes: 
 
* BackOffice general (para nosotros). Donde nosotros podremos controlar todo en general. Ventas, comercios registrados, productos… Podría ser un panel basado en Prestashop pero añadiendo y quitando cosas para crearlo a medida. 
 
	* BackOffice del comercio. Cada comercio tendrá su backOffice donde podrá gestionar sus: 
	* Productos: Subirlos, eliminarlos, desactivarlos, programar los días de publicación y ofertas. Esto como mínimo. 
	* Ventas: Un panel donde pueda ver todas sus ventas y gestionarlas. 
	* Reservas: Un panel donde pueda ver todas las reservas del día y gestionarlas. 
	* Estadísticas: Productos más visitados, productos más vendidos, etc. 
 
* Tienda online. Que debería tener al menos las siguientes funciones: 
	* Una pestaña por cada comercio, con un listado de los productos que vende (en la plataforma, se entiende). 
	* Mapas interactivos donde la gente pueda seleccionar de manera visual donde comprar. 
	* En la pagina de producto, un botón de reserva, otro de compra. 
	* Area privada, para que cada usuario privado tenga su cuenta con pedidos, reservas, etc. 
 
##APP 
 
Lo mismo que la plataforma más lo visto anteriormente. 
 
Puntos que habría que resolver: 

* Transporte, ¿si un cliente compra dos productos de dos tiendas que están lejos entre si, como hacer para que pague lo mínimo por el transporte? ¿cómo optimizar el transporte para comercios pequeños que ya de por si cuentan con poco margen de beneficio? 
* Pago. Lógicamente los pagos online irían a una cuenta bancaria (la nuestra). ¿Cómo hacemos que el dinero vaya después a cada comerciante según lo que hayan vendido ese mes? Hacer transferencias a mano es casi inviable si hablamos de tener más de 1000 clientes de largo. 
* Elegir tipo de código para hacer la plataforma web. 
* ¿En que punto lanzaríamos la app? ¿Quien la hace? ¿Como? 
* ¿Vamos a incluir un sistema de posicionamiento de productos? Por ejemplo, si hay dos productos iguales en una misma ciudad, si uno paga más, se le posiciona más arriba. Ordenación por criterios objetivos, como en toda las webs: Precio, cercanía, relevancia, opiniones, etc. Sistemas de recomendación como el de Amazon, con técnicas de machine learning se hace fácil, aunque suele dar resultados inesperados. Me refiero a algo muy simple. Si tu buscas 1kg de pechuga pavo y hay dos comercios que tienen 1kg de pechuga de pavo. Pues si uno tiene el sistema "premium" (por llamarlo de alguna manera) activo, pues saldrá antes en los resultados, no es más. De todas formas no estoy seguro esta idea se desmarca un poco de la filosofía de simpleza y claridad. 