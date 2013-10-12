eSpaces Platform Buildout
=========================

This Buildout configuration creates a Plone-based environment for operating
eSpaces, an environment for collaboration in Australian research communities.

Quick start
-----------

Bootstrap your environment with the automated deployment configuration
(powered by Vagrant for development, and Salt for provisioning located at
https://github.com/espaces/espaces-deployment. 

Otherwise, install relevant packages for a default Plone 4.3.x installation on
your favourite OS and run Buildout accordingly::

    python bootstrap.py
    ./bin/buildout
    #Start resulting Plone installation
    ./bin/instance1 fg
