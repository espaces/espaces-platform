eSpaces Platform Buildout
=========================

This Buildout configuration creates a Plone-based environment for operating
eSpaces, an environment for collaboration in research communities.  This
specific configuration works for Australian and New Zealand research
communities, though the concept can easily be extended.

Quick start
-----------

Bootstrap your environment with the automated deployment configuration
(powered by Vagrant for development and Salt for provisioning) located at
https://github.com/espaces/espaces-deployment. 

Otherwise, you can manually configure Plone itself. Install the relevant
dependency packages for a default Plone 4.3.x installation on your favourite
OS and run Buildout accordingly on the code in this repository::

    python bootstrap.py
    ./bin/buildout
    #Start resulting Plone installation
    ./bin/instance1 fg

Requirements
------------

* For default installation, ``mail.espaces.edu.au`` must point to a 
  valid SMTP mail service. At the time of writing, this is a ``CNAME``
  record in DNS that points to a relevant SMTP service for cloud operation.
