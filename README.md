RESTIC
=========

This role installs and configures restic & auto-restic.

Requirements
------------

No previous requirements are required

Role Variables
--------------

There are 3 types of vars:
- Install vars
- Config vars 
- Trigger vars

Only install vars are viable on it's default value. To configure restic_locations and backends, just follow yaml guidelines and autorestic docs. 

The trigger to launch a "autorestic check" needs the autorestic_generated_conf_path to be defined! This var is used to fetch the generated configuration file with the key to a local path where ansible is being executed. 

Dependencies
------------

No dependencies to other roles

Example Playbook
----------------

Just add it to the playbook as restic.role :)

If you want to run tests, the "tests" dir have a vagrant env configured. 

License
-------

BSD

Author Information
------------------

AdSanz A.K.A Null0ps