# Estilo para jupyter slides

**Resumen**
Para poder crear slides y hacerlo con estilos predeterminados realizaremos los siguientes pasos:
1. crearemos un entorno en python
2. crearemos las slides en una notebook con extensión ipynb
3. crearemos un archivo .css que contenga el estilo deseado para las slides
4. renderizaremos la notebook y listo!
Para que esto sea posible utilizaremos la biblioteca [RISE](https://github.com/jupyterlab-contrib/rise/tree/main).

Algunos puntos a tener en cuenta:
* de acuerdo a la version de jupyter notebook o lab con la que estes trabajand, tendras que usar una versión distinta de la librería. Esto se especificará en la sección siguiente.
* crearemos un template.css en los cuales se podrán cambiar:
    a. tamaño de font
    b. estilo de font
    c. color de font
    d. color de fondo
    para headers 1, 2 y 3 y para el cuerpo del texto.

Completar Además IMAGENES Ver opciones: [css para imagenes](https://www.w3schools.com/css/css3_images.asp)

## Pasos para crear una jupyter slide con estilos predefinidos

0. Creamos un entorno virtual, en este caso lo estamos nombrando como "slides" y lo inicializamos:

```
conda create -n slides
conda activate slides
```

1. Buscamos la versión de notebook instalada en el environment:
```
jupyter --version
```

Si no tienes instalado jupyter lab puedes hacerlo con el siguiente comando:
```
conda install -c conda-forge jupyterlab
```

2. A continuacion instalaremos la version de RISE correpondiente a nuestra version de jupyterlab. Si la versión de jupyterlab es >= 4.0, utilizaremos la biblioteca [RISE](https://github.com/jupyterlab-contrib/rise/tree/main) sino utilizaremos [esta version de RISE](https://rise.readthedocs.io/).

Continuare describiendo el caso en el que jupyterlab>=4.0
[Describo el otro caso? es muy sencillo, creo]

```
pip install jupyterlab_rise
```

3. Para crear las slides primero debemos crear el contenido en una notebook. Las celdas que se pueden utilizar en las slides son de tipo markdown o codigo. Para poder generar las slides, a cada celda le tendremos que asignar un tipo dentro de la siguientes opciones: -, slide, subslide, fragment, skip, notes.
Para asignarle el tipo seleccionar el Property inspector en la barra de herramientas lateral derecha (dos tuequitas). Luego, pararse en la celda de interes y asignarle el "Slide type" deseado.

4. Crear el archivo de estilos con extension .css. Ponerle el mismo nombre que el de la notebook del punto anterior y guardarlos en la misma carpeta.

6. Una vez que tenemos los dos archivos: el .ipynb que contiene a las slides y el .css que contiene los estilos, vamos a crear las slides. Para eso, vamos View> Render as Reveal Slidehow (o Alt+R). De esa manera se podra ver las slides y si quiere hacer una presenacion puede elegir la opcion Open de slideshow in full screen.
