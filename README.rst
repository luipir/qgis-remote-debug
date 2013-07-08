=================
qgis-remote-debug
=================

Start Python remote debugger from QGIS plugin

QGis: Plugin manual installation outside the QGIS plugin manager
----------------------------------------------------------------

follow these steps:

 - clone this repositoy in a <path>
 - copy or link <path>/qgis-remote-debug/RemoteDebug in $HOME/.qgis2/python/plugins/remotedebug (!!! lower case !!!)
 - explicitly add $HOME/.qgis2/python/plugins in PYTHONPATH for the qgis session e.g setting in a shell script that launch qgis
 - then follow reading this document


PyDev Debugging (Eclipse)
-------------------------

`PyDev`_ is a Python IDE for Eclipse with `remote debugger`_ support.

The steps to debug an external program are:

- Go to the debug perspective
- Configure remote debugging of exceptions (PyDev > Manage Exception Breakpoints)
- Start the debug server (PyDev > Start Debug Server)
- Press the QGIS toolbar icon to activate remote debugging
- The debugger is activated when a breakpoint is reached or an expception is raised (configureable) 

.. _PyDev: http://pydev.org/
.. _remote debugger: http://pydev.org/manual_adv_remote_debugger.html

ERIC4 Passive Debugging 
-------------------------

The Steps to activate passive debuging with ERIC4 are:

- open Settings->Preferences->Debugging General
- activate the option "Passive Debugger Enabled"
- Restart the ERIC4 IDE
- Load the Plugin-Project
- Press the QGIS toolbar icon to activate passive debugging with eric4

