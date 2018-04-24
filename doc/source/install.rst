.. Copyright SAS Institute

Installation
============

DLPy can be installed using ``pip`` as follows::

    pip install sas-dlpy

Releases can also be found on GitHub at https://github.com/sassoftware/python-dlpy/releases.


Prerequisites
-------------

SWAT
****

DLPy does not do any analytic operations itself.  It is a wrapper around the SWAT
package which communicates with a SAS CAS server to do the analytics.  The SWAT
package can be installed from GitHub at the following URL.

https://github.com/sassoftware/python-swat/releases


Graphviz
********

When installing DLPy, the graphviz Python package will automatically be installed.
However, the graphviz Python package will not work without the graphviz command-line
tools from https://www.graphviz.org/download/.  You must install those for your
system, and add the location of the ``bin/`` subdirectory to your systems' path.

To verify that the utilities will work, run the following command::

    dot -V

Keras (Optional)
****************

To enable the Keras model conversion, a Keras package with version 2.1.3 or newer is required.
It can be downloaded from https://github.com/keras-team/keras or installed/updated by 
running the following command in the command line::
    pip install --upgrade keras
    
    
Caffe (Optional)
****************

To enable the Caffe model conversion, a Caffe package with version 1.0.0 or newer is required.
The instruction of Caffe installation is available at http://caffe.berkeleyvision.org/installation.html.
