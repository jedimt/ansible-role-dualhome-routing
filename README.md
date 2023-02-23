Ansible Role: Dualhome Routing
=========

This role sets up routing for a Ubuntu Linux host when using two highspeed NICs on the same L2 segment.

Requirements
------------

None

Role Variables
--------------

There are eight variables for this role. Examples:

        # These variables are highly host specific. I have them defined in a
        # host_vars file for each inventory host
        data_ip: 10.100.25.35
        mgt_ip: 10.100.25.34
        mgt_int: eno1
        data_int: ens6f0np0

        # These are defined as role defaults
        route: 10.100.24.0/22
        gateway4: 10.100.24.1
        mgt_route_table: 100
        data_route_table: 101


Dependencies
------------

None.

License
-------

MIT

Author Information
------------------

Aaron Patten
aaronpatten@gmail.com
