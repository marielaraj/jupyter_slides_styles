# Jupyter slides style

**Summary**
To create slides with predefined styles, we will follow these steps:
1. Create a Python environment.
2. Create the slides in a notebook with the .ipynb extension.
3. Create a .css file that contains the desired style for the slides.
4. Render the notebook, and you're done!

We will use the library [RISE](https://github.com/jupyterlab-contrib/rise/tree/main) to make this possible.

Some points to consider:
* Depending on the version of Jupyter Notebook or JupyterLab you are using, you may need to use a different version of the library. This will be specified in the following section.
* We will create a template.css where you can customize:
    a. Font size
    b. Font style
    c. Font color
    d. Background color
    for headers 1, 2, and 3 and for the body of the text.



## Creating the environment

0. Create a virtual environment, in this case named "slides," and activate it:

```
conda create -n slides
conda activate slides
```

1. Check the version of Jupyter Notebook installed in the environment:
```
jupyter --version
```

If you don't have JupyterLab installed, you can do so with the following command:
```
conda install -c conda-forge jupyterlab
```

2. Next, install the RISE version corresponding to your JupyterLab version. If your JupyterLab version is >= 4.0, use the [RISE library](https://github.com/jupyterlab-contrib/rise/tree/main); otherwise, use [this version of RISE](https://rise.readthedocs.io/).

I will describe the case when JupyterLab >= 4.0
[Do you want me to describe the other case? It's straightforward, I think]

```
pip install jupyterlab_rise
```

3. To create the slides, first, generate the content in a notebook. The cells that can be used in the slides are of markdown or code type. To generate the slides, you need to assign a type to each cell from the following options: -, slide, subslide, fragment, skip, notes.
To assign the type, select the "Slide type" in the Property inspector on the right-hand toolbar. Then, choose the desired type for the cell.

4. Create the styles file with a .css extension. Name it the same as the notebook from the previous step and save them in the same folder.

5. Once you have both files (the .ipynb containing the slides and the .css file containing the styles), go to View > Render as Reveal Slideshow (or Alt+R). This way, you can view the slides, and if you want to present, you can choose the Open slideshow in full screen option.
