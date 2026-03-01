Role Name
=========
config-printer

Setup Printing for RHEL and FreeBSD hosts

Requirements
------------
RHEL and FreeBSD OSs

Role Variables
--------------

# contents of defaults/main

# printer declaration variable
# Currently I am only supporting ipv4
config_printer_printers:
  - printer_name: 
    driver_filepath:
    printer_path:

# user list to be used to check and if necessary add user to cups group
config_printer_users:
  -

# The following variables are used for the defaults/RedHat and defaults/FreeBSD files
# The values will be different based on OS specifics

# path and name to the config file
config_printer_config_file_path: 

# contents of RedHat_variables.yml under vars

# packages to install
config_printer_pkgs:
  - name:

# name of the printer service
config_printer_printer_svc:


Dependencies
------------

None.

Example of Playbook
-------------------

- hosts: linux_workstations

  vars:
    
    my_default_printer_name: home_printer
    my_default_printer_ip: 10.0.0.200

    config_printer_printers:
      - printer_name: "{{ my_default_printer_name }}"
        driver_filepath: "///sample.drv/laserjet.ppd"
        printer_path: "socket://{{ my_default_printer_ip }}:9100"

  roles:

    - name: config_printer

License
-------

BSD

Author Information
------------------

Rich O'Hara

