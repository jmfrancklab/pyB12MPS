===============
pyB12MPS Module
===============

In this section the functions of the pyB12MPS module are explained. In general, most functions can be used to query a parameter, while some functions can query and set (send) a value to the MPS.

For example the command::

   B12MPS.freq()

will return the current microwave frequency of the MPS, while::

   B12MPS.freq(9.554)

will set the microwave frequency to 9.554 GHz.


pyB12MPS Functions
------------------

.. automodule:: pyB12MPS.pyB12MPS
   :members:

Example - pyB12MPS Module
-------------------------

::

    import pyB12MPS as mps

    if mps.test(): # if server is not running, start server
        mps.start(debug = True)

    mps.freq(9.6) # Set microwave frequency to 9.6 GHz

    mps.power(10) # Set microwave power to 10 dBm

    mps.stop() # Stop the server

