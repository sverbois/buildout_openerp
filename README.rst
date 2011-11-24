Usage
=====

Install PostgreSQL and OpenERP 6.0.3::

    git clone git://github.com/sverbois/buildout_openerp.git
    cd buildout_openerp
    python bootstrap.py --version 1.5.2 --distribute -c 603.cfg
    ./bin/buildout -c 603.cfg
    
Install PostgreSQL and OpenERP trunk::

    git clone git://github.com/sverbois/buildout_openerp.git
    cd buildout_openerp
    python bootstrap.py --version 1.5.2 --distribute -c trunk.cfg
    ./bin/buildout -c trunk.cfg
    
Start PostgreSQL/OpenERP::

    ./bin/start-postgresql
    ./bin/start-openerp-server
    ./bin/start-openerp-web
    
**Options**

To skip PostgreSQL and/or lxml static installation,
remove the lines *staticlxml.cfg* and/or *postgres905.cfg*
in the *extends* section of the configuration file. 

Credits
=======

This buildout is inspired by the work of Antonio SAGLIOCCO aca kalymero.

Author
------

Sébastien VERBOIS - sebastien.verbois@gmail.com
