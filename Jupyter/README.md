# Klampt-jupyter-extension

This folder contains the [Jupyter notebook](http://jupyter.org) extension for [Klamp't](https://github.com/krishauser/Klampt).

## Installation

To make any use of this extension, you will need to install:

- [Jupyter notebook](http://jupyter.org) 
- Klamp't Python API (try `pip install klampt`)

To install the extension, you can simply enter

`sudo make install`

in this directory.

For more control, you can use the following Makefile targets:

- `install-user`: Installs this in the Jupyter user prefix
- `install-wurlitzer`: The wurlitzer library for capturing C++ output in Python.  This is not strictly needed, but is nice to have

## Usage

The best way to learn how to use this extension is to study the example notebooks in the Jupyter subdirectory of the [Klamp't examples](https://github.com/krishauser/Klampt-examples) package.
Run:

> git clone https://github.com/krishauser/Klampt-examples

And then launch Jupyter:

> cd Klampt-examples/Jupyter
> jupyter notebook

The Jupyter frontend widget can be created by a `KlamptWidget`, which is defined in the `klampt.vis.ipython` module. 
Try typing `help(klampt.vis.ipython.KlamptWidget)` for more help.  The `klampt.vis.ipython` module also contains useful helper widgets for editing robot configurations and points.

Auto-generated [documentation for the klampt.vis.ipython module can be found here](http://motion.pratt.duke.edu/klampt/pyklampt_docs/ipython_8py.html).

## Version history

0.1.0: first release


## Wish list

- Saving widget state to HTML.
- Saving standalone animations in HTML.
- Camera resetting in the GUI.
- More control over background color, lighting, textures.
- Live editing in the visualization.
- Closer interface to the klampt.vis module.

## Contact

Author: Kris Hauser

Duke University

kris.hauser@duke.edu