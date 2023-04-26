# ESta es la documentación y apuntes del Curso Practico de Introducción a Unity

Presentado por : MIGUEL ANGEL MORA ORTIZ
Programa: DESARROLLO DE VIDEOJUEGOS Y ENTORNOS INTERACTIVOS
SENA    
Ibagué, Tolima
Colombia

Introducción a Unity

clase - 1

Ruth Margarita García - Desarrolladora de Videojuegos

* Interfaz de Unity
	Es fundamental tener establecida la escena, antes de entrar a programar
	
Clase - 2

	Quiero programar videojuegos? 
	Por donde empiezo?
	Cómo lo hago?

¿Qué es Unity?

Es un Game Engine
	*Nos permite: Crear experiencias interactivas
		      Renderizar en tiempo real
		      Manipular asset

-Renderizado en tiempo real 	- Frames por segundo
-Interactividad 		- Cómo el jugador de "habla" al juego

	Assets = Archivod que el juego puede usar para mostrar la experiencia.


¿Qué no es Unity?

Unity no es un editor de Assets

	*Archivos 3D		- Blender, Maya, Sketchup	
	*Archivos 2D		- Krita, Inkscape, Photoshop, Illustrator
	*Música y sonidos	- Audacity, Adobe Audition
	*Archivos de código	- Visual Studio, Sublime, Emacs, Vim


*Puede serlo, pero no lo es:
-ProBuilder = Creación de assets 3D
-UnityAnimations (antes Anima 2D) = Animación de assets 2D


Clase - 3

Instalación de Unity

	Unity Hub > Unity Editor > Módulos

*Unity Hub 	= Es el programa que nos permite descargar cosas
*Unity Editor 	= Programa de realización de Videojuegos
*Módulos 	= Son herramientas que nos permite compilar los videojuegos para usarlos en diferentes consolas



Clase - 4 

Repaso y uso de la interfaz de Unity 

Es primordial mantener un orden en nuestra interfas, para agilizar y facilitar el trabajo en la plataforma


Clase - 5

Paneles:
Escena - Inspector

Qué es una escena?
	*Es un asset
	*Son niveles (El menú del juego es un nivel) Agrupación de elementos

	En esta ventana, podremos ver el desarrollo de nuestro proyecto desde cualquier ángulo, incluso si es movimiento.


Asset= archivo sin función en especifico
Instancia de asset = archivos con funciones, animaciones, (mas divertido)


*Inspector 

*GameObject = Cada cosa en escena


Los cambios que realicemos en el inspector, se harán así mismo en la escena

Componente: Función que le dice al objeto como comportarse


Cuando creamos un nuevo object, podemos agregarle todas las funciones y caracteristicas que queramos

En el inspector, no solo vemos los objects seleccionados, sino también asset y sus caracteristcias

Debemos tener precaución cuando aplicamos un asset o object en la escena, para que se cargue siendo el archivo que es y aplicando la función que hará



Para que sirve cada panel =
	*Inspector: Ver/editar propiedades
	*Project:	Explorador de assets	
	*Escena:	Ver/editar escenas
	*Jerarquía:	Lista de GameObjects en escena



	*GameObject:	Todo elemento en una escena
	*Componente: 	Comportamiento de un GameObject
	*Escena:		Un asset que engloba varios GameObjects y configuraciones




Clase - 6

Como compartir tus proyectos?
Importar y exportar Unity Packages


Podemos usar Unity Packages, para optimizar la exportación de nuestros archivos

Click derecho en la escena > Exportar Package > Seleccionamos los archivos > Genera el paquete

Optimizando el peso del archivo y facilidad de obtención




Clase - 7

Git > Sistema de versionamiento

	Repositorio > Es un proyecto, junto con todas sus versiones
		*Remote
		*Branches
			-main
		*Commits
		*HEAD


Git desde la línea de comando =
	cmd > GUI

Creamos el repositorio desde github y lo clonamos en gitbash

No es recomendable usar versiones distintas con cada programa que usemos
(usar una versión antigua de un archivo creado en unity 2020 y abrirlo en una versión de 2022-2023 de unity)
	*Pueden haber fallos en las funciones

 


Clase - 8


El uso de https, depende de tu usuario y contraseña de la cuenta de github, para el uso de remoto y local en gitbash

Llaves SSH, encriptación. Para el uso de 

Para generar una llabe SSH, seguimos los siguientes pasos:
*Entramos a gitbash, e introducimos el siguiente código:
	ssh-keygen
		(acá podemos seguir por defecto, pero podemos elegir en qué archivo y carpeta queremos generar esta llave))
	continuamos sin ingresar clave, si nuestra pc es privada y propia.

Para ver la llave generada, ingresamos el cógido:
	
	cat (nombre de archivo, carpeta donde destinamos)
La llave generada con (.pub) es la que podemos compartir, la otra es personal y propia.


Copiamos esta llave publica y la ingresamos en github.





Clase - 9

Como volver un repositorio mi proyecto?

Para sincronizar un repositorio remoto, con un repositorio local nuevo, usamos el código:
* git remote add +nombre del repositorio+ "link https o clave ssh"



Ramas:
	*git checkout (rama)
	*git checkout -b (rama)
	*git merge (otra-rama)
	*git diff (archivo)
	*git diff (hash) (archivo)
	*git branch -v






Clase - 10

Navegar a través de la escena:

Pivote: Es el punto al rededor de un objeto
Click derecho: mover hacia los lados
q : subir. e: bajar
wasd : movernos a través de la escena
click derecho + rodillo del mouse: aumentar o disminuir la velocidad de movimiento
alt + click normal: mover vista al rededor de un pivote

Si nos salimos de la visión de nuestro mapa en la escena, podemos dirigirnos a la jerarquía, seleccionamos el elemento que deseamos volver y presinamos la tecla "F".

Como encontramos un objeto en nuestra escena?
Nos dirigmos a Jerarquía y buscamos ese objeto por su nombre, automaticamente en la escena se mostrará ese objeto y además se distinguirá de los otros.



HUEVO DE DIAMANTE: Este se encuentra en el laberinto gigante
HUEVO DE ORO:	 Se encuentra en una armario azul dentro de la habitación 1








Clase - 11

Como manipular el Transform


*Grayboxing
*Armar el nivel
*Hacer pruebas

Mover objetos depende del componente Transform, todos los objetos tienen uno
	-Position
	-Rotation
	-Scale


Atajos:
Ctrl + Shift = Poner un objeto sobre cualquier superficie de otro
Z = cambia entre el pivote o el centro de un objeto
V = selecciona el vertice de un objeto para moverlo en la escena
Ctrl + shift + F = Para poner un objeto en la cabeza de la cámara
ctrl + alt + f = traer un objeto seleccionado a donde estés





Clase - 12

Materiales = Colores, shaders y reflection probes

¿Cómo le pongo color  a un objeto 3D?
*Meshes
*Mapas UV
*Texturas
*Materiales
*Shaders


Mesh
Es una cantidad de puntos recopilados, unidos, haciendo una forma y superficie
Estas superficies están hechas por poligonos, y estas se pueden volver triangulos



Materiales - Shaders - Texturas

Shaders = Es un programa que nos dice a nuestra tarjeta gráfica como interpretar o renderizar cada pixel
Material = Es una interpretación del shader, esta puede tener propiedades, color, números, entre otras características



 Para crear un color, debemos crear un Material dentro de la carpeta de Assets
	Para tener un mejor orden en nuestra mesa de trabajo, ponemos el nombre al objeto que le aplicaremos.
	Para colocar este material a un objeto, simplemente arrastramos el archivo y lo dirigimos al objeto deseado, dentro de la escena
	Si queremos cambiar las caracteristicas del material, seleccionamos el material y desde ahí cambiamos lo que deseemos. pero este cambio afeectará todos los objetos que tengan designada este material

Si queremos añadir una función de reflejo en nuestros objetos, debemos agregar Reflection Pro en nuestra Jerarquía







Clase - 13

Espacio global 	- Es el espacio en general de un mapa/mundo real (latitud, longitud, coordenadas) )
Espacio local 	- Es la dirección o espacio de un objeto en especifico (arriba, izquierda, derecha)

Jerarquía
	Los hijos de un objeto se transforman junto a su padre


Centro - Pivote

Centro = centro de gravedad de un objeto
Pivote = punto de al rededor el cual gira



Clase - 14

Fuentes de sonido y escucha

*AudioSource > componente >Bocina del sonido en el juego
*AudioListener > Orejas que captan el sonido 
*AudioMixer

-Debugear sonido



Clase - 15

Luces y Efectos

Luz > Componente = Luz direccional, luz de punto

Efectos: 
	*Trail
	*Partículas
	*Líneas






Clase - 16

Prefab = Es un asset, pero en escena se vuelve una instancia de un template, y cuando lo modificas, también se cambian todas las instancias que están en la escena

Hay formas correctas de duplicar y esta es usando prefabs.

Tipos de prefab:

Simples: Template de forma de asset. 
Anidados: Prefabs dentro de prefabs.
Variantes: Modificaciones que son prefabs. > Debe tener un prefans principal, para que apartir de este se le hagan 							   las modificaciones que queramos.


Para crear un template de prefab, primero se crea un GameObject 

Clase - 17

Por qué usar Prefabs?

El uso de prefabs en nuestro proyecto y desarrollo, nos facilitará el proceso de este. Siendo capaces de trabajar desde diferentes ramas haciendo uso de Git, para un desarrollo más efectivo y práctico. 

Usando Prefabs, nos será de mucha utilidad, cuando queremos generar elementos dentro de nuestro juego, que sean similares, sin necesidad de hacerlo uno por uno. Le hacemos los cambio al elemento raíz y los otros tomarán los mismos detalles. Si ya queremos hacer un cambio en especifico, simplemente hacemos uso de un elemento en especial que le queramos hacer este mismo cambio.

No sería buena practica, hacer un elemento y este mismo copiarlo y pegarlo. Este sería el uso que le damos al Prefabs, facilitarnos este trabajo.


Clase - 18

Vistazo al 2D - Sprites

Cuando manejamos un 2D, es necesario si importamos el archivo desde un programa ajeno, es primordial hacerlo con estilo PNG, para que se vea el personaje y no una imagen con fondo. 

Cuando usamos 2D en unity tenemos la opción de ver la cámara explicitamente en un solo plano

Para no estar configurando cada GameObject como un Sprite para usarlo en 2D, podemos configurar desde el inicio el editor, para proyectos 2D.

Si ya creamos el proyecto en un editor 3D, podemos facilmente cambiar la configuración desde =
	Settings > Project Settings > Editor > Default Behavior Mode > 2D

Cuando ubicamos nuestro sprite en escena, debemos tener en cuenta las posiciones de cada instancia. Que una esté por delante o detrás de otra. Para eso usamos el 'Order in Layer', mayor sea el numero, mas propiedad tendrá de suporponerse sobre otros.

También podemos hacer uso de 'Sorting in Layer', para darle una palabra clave a cada elemento y así tener un area de trabajo más comoda y optimizada

En unity también podemos editar sprites, en caso de que nuestro png, venga una imagen por partes. Este paquete debemos descargarlo, en caso de que la versión del editor no la tenga

Sorting Group -> Nos sirve para decir a nuestro elemento hecho con varias partes se identifique como uno solo.



Clase -19

¿Cómo pedirle a un objeto que obedezca las leyes de la física?

Con Componentes


Un joint es una articulación, une 3 rigidbodies. Simulación física, que puede romperse

"Fixed Joint" = Es como pegamento, 
"Spring Joint" = Articulación de resorte
Hinge + Spring = Efecto trampolín o bisagra de va y ven
Hinge + Motor = Efecto de molino de viento, gira sobre un eje según una fuerza

Cuando agregamos un joint a un GameObject, automaticamente agrega el rigidbody, ya que sin este no es posible su uso

Rigidbodie 	> Simula física mediante el transform
Collider	> Cómo colisiona con su entorno

Jerarquía y Rigidbodies 

	Los colliders que son hijos de un Rigidbody están 'sujetos' a su padre.

Rigidbody kinemático

	+ Pueden afectar a otros bodies
	+ Otros bodies no le afectan a él
	+ La simulación no afecta a su transform


Clase - 20

Joints - Clavos, resortes, bisagras y motores.





