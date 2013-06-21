ome-vagrant
===========

vagrant / ansible bootstrap for OME

Quickstart
==========

* Clone this repository
* copy/unzip an omero 4.4.x-ice34 installation into cloned directory
* symlink omero directory to OMERO-CURRENT
* create/symlink a data repository directory called OMERO
* adjust box name in Vagrantfile to reflect your proper centos 6.x box
* vagrant up

Issues
======

* if omero.server or omero.web are not shutdown gracefully they will fail to start b/c of the existing pid files
* cannot use a symlink outside of vagrant dir as the export in the vm dereferences and becomes broken
* schema population is touchy due to presense of .omero-schema-created file so can fail easily
  * needs a better check for successful schema run
