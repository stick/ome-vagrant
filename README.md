ome-vagrant
===========

vagrant / ansible bootstrap for OME

Quickstart
==========

* Clone this repository
* copy/symlink/unzip an omero 4.4.x-ice34 installation into cloned directory
* symlink omero directory to OMERO-CURRENT
* create/symlink a data repository directory called OMERO
* adjust box name in Vagrantfile to reflect your proper centos 6.x box
* vagrant up

Issues
======

* if omero.server or omero.web are not shutdown gracefully they will fail to start b/c of the existing pid files
